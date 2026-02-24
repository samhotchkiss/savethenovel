# Save the Novel — Content Model

## Core Content Type: Essay

An essay is the fundamental unit of content on the site. It is a long-form personal letter or essay addressed to the author of a novel that changed the contributor's life.

### Essay Fields

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `title` | String | Yes | Title of the essay/letter |
| `slug` | String | Yes | URL-safe identifier, auto-generated from title |
| `body` | Rich Text | Yes | The full essay text (long-form) |
| `excerpt` | String | Yes | 2-3 sentence pull quote or summary for cards/previews |
| `book_title` | String | Yes | Title of the novel the essay is about |
| `book_author` | Reference → Person | Yes | Author of the novel |
| `contributor` | Reference → Person | Yes | Person who wrote this essay |
| `bookstore` | Reference → Bookstore | Yes | Contributor's favorite indie bookstore |
| `featured_date` | Date | No | Month this essay was the featured spotlight |
| `published_date` | Date | Yes | When the essay went live |
| `status` | Enum | Yes | `draft`, `in_review`, `published` |
| `cover_image` | Image | No | Optional hero image for the essay |

### Long-Form Content Considerations

These essays are substantial — likely 1,000-5,000+ words. Design and technical considerations:

- **Reading experience** matters: generous line height, comfortable measure (~65 characters), quality typography
- **Estimated reading time** displayed on cards and essay pages
- **Progressive rendering** — the full essay loads on its own page, not truncated with "read more"
- **Print stylesheet** — readers may want to print these; honor that instinct
- **Anchor links** — for particularly long essays, consider section anchoring

## Person

A person can be a **Book Author**, a **Contributor**, or both. This is a single entity to avoid duplication when someone occupies both roles.

### Person Fields

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | String | Yes | Full name |
| `slug` | String | Yes | URL-safe identifier |
| `bio` | String | No | Brief biographical note |
| `website` | URL | No | Personal website, Substack, etc. |
| `roles` | Array of Enum | Yes | `book_author`, `contributor`, or both |

### Linking Logic

- When displayed as a **Book Author**: shows all essays written *about* their books
- When displayed as a **Contributor**: shows all essays they *wrote*, plus links to their website
- Name is hyperlinked to their website/Substack when available

## Bookstore

Each essay links to the contributor's favorite independent bookstore.

### Bookstore Fields

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | String | Yes | Bookstore name |
| `slug` | String | Yes | URL-safe identifier |
| `location` | String | Yes | City, State |
| `website` | URL | Yes | Bookstore website |
| `description` | String | No | Brief description or contributor's note about why this store |

### Bookstore Aggregation

A bookstore page or sidebar feature could show:
- How many essays link to this bookstore
- Which contributors named it as their favorite
- Direct link to the store's website

This creates a natural network effect — bookstores have an incentive to promote the site because it drives traffic to them.

## Taxonomy / Browse Dimensions

| Dimension | Source | Browse URL |
|-----------|--------|------------|
| By Book Title | `essay.book_title` | `/essays?by=title` |
| By Book Author | `essay.book_author.name` | `/essays?by=author` |
| By Contributor | `essay.contributor.name` | `/essays?by=contributor` |
| By Bookstore | `essay.bookstore.name` | (future: `/bookstores`) |

## Featured Essay

One essay per month is selected as the **Featured Essay**:

- Displayed prominently on the homepage
- Sent to the mailing list subscribers
- Added to the Featured Archive after its month ends

### Featured Archive

Reverse-chronological list of all previously featured essays with the month they were spotlighted.

## Newsletter / Mailing List

| Field | Description |
|-------|-------------|
| **Frequency** | Monthly |
| **Content** | The featured essay of the month |
| **Source** | Site's own mailing list (primary), cross-posted to Substack as Notes |
| **Preference** | Emails come from the site directly; Substack is a mirror |

### Mailing List Sync Consideration

S.E. Elkins also maintains a Substack. Ideal workflow:
1. Featured essay is published on the site
2. Email goes out to the site's mailing list
3. A Note or post is cross-published to Substack

Whether to automate the Substack cross-post or handle it manually is a future decision. Priority is the site's own email list.

## Content Workflow

```
Contributor submits essay (via form or email)
        ↓
Editorial review (S.E. Elkins)
        ↓
Request contributor info:
  - Bio, website, favorite indie bookstore
        ↓
Essay published → status: published
        ↓
Optionally selected as Featured Essay for a given month
        ↓
Featured essay sent to mailing list
```

## Content Volume Projections

- **At launch**: 10-20 essays from Southwest bookstore event contributors
- **Ongoing**: New submissions from readers and authors
- **Growth**: East Coast bookstore tour in Fall 2026 will generate a wave of new content
