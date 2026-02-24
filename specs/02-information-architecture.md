# Save the Novel — Information Architecture

## Sitemap

```
savethenovels.org
├── Home (/)
│   ├── Hero / Manifesto
│   ├── Featured Essay (rotates monthly)
│   ├── News on Reading (curated links to articles about novel reading)
│   └── Call to Action (read, submit, subscribe)
│
├── Essays (/essays)
│   ├── Browse All
│   ├── By Book Title (/essays?by=title)
│   ├── By Book Author (/essays?by=author)
│   ├── By Contributor (/essays?by=contributor)
│   ├── By Publication Date (/essays?by=date)
│   └── Individual Essay (/essays/:slug)
│
├── Featured Archive (/featured)
│   └── Previously featured essays, reverse chronological
│
├── Submit (/submit)
│   ├── Submission Guidelines / FAQ
│   └── Submission Form or Contact Link
│
├── About (/about)
│   └── About S.E. Elkins and the project
│
├── FAQ (/faq)
│   └── Contribution rules, editorial process, rights
│
└── Subscribe (/subscribe)
    └── Mailing list signup
```

### Additional P0 Pages
```
├── News (/news)                 # Curated news and articles about novel reading
└── Resources (/resources)       # For educators and new novel readers
```

### Future Pages
```
├── Shop (/shop)                 # "I come from the library" merch
└── Events (/events)             # "Let the Reader Speak" bookstore events
```

## Navigation

### Primary Navigation (persistent header)
1. **Home**
2. **Essays** (with dropdown: By Title, By Author, By Contributor)
3. **Submit**
4. **About**

### Secondary Navigation (footer)
- FAQ
- Subscribe / Mailing List
- Contact
- Featured Archive

## Content Organization

Essays are the core content unit. They can be discovered through four primary taxonomies:

| Taxonomy | Description | Example |
|----------|-------------|---------|
| **Book Title** | The novel the essay is about | *Beloved*, *One Hundred Years of Solitude* |
| **Book Author** | The author of that novel | Toni Morrison, Gabriel Garcia Marquez |
| **Contributor** | The person who wrote the essay | A local author, a reader, a teacher |
| **Publication Date** | When the essay was published on the site | Newest first, or by month/year |

### Note on Overlapping Roles
Some book authors will also be contributors (writing about a different novel that changed *their* life). The data model must handle this cleanly — a person can exist as both a "Book Author" and a "Contributor" without collision.

### Contributor Profiles
- Name (linked to personal website or Substack, if any)
- Brief bio (optional)
- Favorite independent bookstore (required — each essay links to one)

## Page Hierarchy & Content Priority

### Home Page
1. **The Manifesto** — sets the tone immediately
2. **Featured Essay** — the monthly spotlight, the heart of the site
3. **Recent Essays** — 3-4 cards showing the latest additions
4. **News on Reading** — curated links to articles about novel reading, literacy, and the literary landscape
5. **Call to Action** — subscribe, submit your story, visit a bookstore

### Individual Essay Page
1. **Essay Title** (which is the letter/essay title, not necessarily the book title)
2. **The Book** — title and author of the novel being written about
3. **The Contributor** — name, linked to their site if applicable
4. **The Essay** — full long-form text
5. **The Bookstore** — name and link to the contributor's favorite indie bookstore
6. **Related Essays** — others about the same book, author, or by the same contributor

### Essays Index Page
- Default: reverse chronological (newest first)
- Filter/sort by: Book Title (A-Z), Book Author (A-Z), Contributor (A-Z), Publication Date
- Search (stretch goal)

## URL Structure

| Page | URL Pattern |
|------|-------------|
| Home | `/` |
| All Essays | `/essays` |
| Single Essay | `/essays/[slug]` |
| About | `/about` |
| Submit | `/submit` |
| FAQ | `/faq` |
| Featured Archive | `/featured` |
| Subscribe | `/subscribe` |
| News | `/news` |
| Resources | `/resources` |

Slugs should be human-readable, derived from the essay title or the book title + contributor name.
