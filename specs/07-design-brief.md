# Save the Novel — Design Brief

*For visual design in Figma*

---

## Project Overview

**Save the Novel** is a website that collects and publishes long-form personal essays about the experience of reading novels. Contributors — authors, readers, teachers — write letters to the authors of the books that changed their lives. Each essay links to the contributor's favorite independent bookstore.

The site's mission is to demonstrate why we read novels, to give readers a voice, and to support the literary ecosystem.

**This is a reading-first website.** The essays are the product. Every design decision should serve the experience of reading a 2,000-word personal essay on a screen.

---

## Brand Personality

| Attribute | Not This | This |
|-----------|----------|------|
| Tone | Corporate, slick | Warm, personal, earnest |
| Feel | Tech startup | Independent bookstore |
| Pace | Fast, scannable | Unhurried, immersive |
| Energy | Loud, promotional | Quiet confidence |
| Aesthetic | Minimalist-cold | Minimalist-warm |

**Key words:** Literary. Intimate. Inviting. Grounded. Human. Timeless.

**The feeling we want:** You've walked into a beautiful independent bookstore on a rainy afternoon. There's good lighting. Someone has made coffee. You're in no rush. You pick up something to read.

---

## Typography

Typography is the single most important design decision for this project.

### Body Text (Essays)
- **Serif font required.** This is a site about novels — serif typography signals "this is meant to be read."
- Suggested directions: Literata, Lora, Freight Text, Crimson Pro, Source Serif Pro, or Iowan Old Style
- Line height: 1.6–1.75 (generous)
- Measure (line length): 60–70 characters max
- Font size: 18–20px on desktop, 17–18px on mobile
- Comfortable paragraph spacing

### Headings
- Can be serif or a complementary sans-serif
- If sans: something warm, not geometric — e.g., Outfit, DM Sans, Source Sans
- Clear hierarchy: H1 for essay title (large, confident), H2 for sections (if essays have them)

### UI / Navigation
- Clean sans-serif for navigation, buttons, metadata, labels
- Small caps or letter-spacing for labels and taxonomy markers
- Monospace accent for dates, reading time, and other metadata (optional)

### Type Scale Reference
| Element | Size (desktop) | Weight |
|---------|---------------|--------|
| Essay body | 18-20px | Regular (400) |
| Essay title | 32-40px | Bold (700) |
| Page headings | 28-36px | Bold (700) |
| Navigation | 14-16px | Medium (500) |
| Metadata (date, reading time) | 12-14px | Regular (400) |
| Cards excerpt | 14-16px | Regular (400) |

---

## Color Palette

### Direction: Warm Literary Neutrals

The palette should feel like the inside of a good bookstore or the endpapers of a well-made book.

### Suggested Primary Palette

| Role | Suggested Range | Notes |
|------|----------------|-------|
| Background | Warm cream / off-white (`#FAF7F2` range) | Not stark white — that's cold and clinical |
| Text | Deep warm brown or charcoal (`#2C2418` range) | Not pure black — softer on the eyes for long reads |
| Accent | Deep green, muted terracotta, or warm navy | One strong color for links, buttons, highlights |
| Secondary | Muted sage, dusty rose, or warm gray | For borders, cards, secondary elements |
| Highlight | Warm gold or amber | For the featured essay, special callouts |

### Color Principles
- **Warm, not cool.** Cream over white. Brown over black. Sage over teal.
- **High contrast where it matters** (text on background for reading)
- **Low contrast for decoration** (subtle card borders, section backgrounds)
- **Dark mode:** Yes, but it should feel warm too — deep brown/charcoal, not pure black

### Avoid
- Bright/saturated blues (feels corporate)
- Pure black on pure white (feels sterile)
- Gradients (feels tech)
- More than 2-3 accent colors (feels busy)

---

## Layout & Grid

### General Principles
- **Generous whitespace.** Let the content breathe.
- **Single-column for essays.** No sidebar competing for attention during reading.
- **Content width:** 680-720px max for essay text (optimal reading measure)
- **Page width:** Up to 1200px for index pages and navigation

### Key Layouts to Design

#### 1. Homepage
```
┌─────────────────────────────────────┐
│           NAVIGATION                │
├─────────────────────────────────────┤
│                                     │
│     THE MANIFESTO / HERO            │
│     (Set the tone immediately)      │
│                                     │
├─────────────────────────────────────┤
│                                     │
│     FEATURED ESSAY                  │
│     (The monthly spotlight —        │
│      title, book, contributor,      │
│      opening excerpt, bookstore)    │
│                                     │
├─────────────────────────────────────┤
│                                     │
│     RECENT ESSAYS                   │
│     ┌───────┐ ┌───────┐ ┌───────┐  │
│     │ Card  │ │ Card  │ │ Card  │  │
│     └───────┘ └───────┘ └───────┘  │
│                                     │
├─────────────────────────────────────┤
│     CALL TO ACTION                  │
│     Read / Submit / Subscribe       │
├─────────────────────────────────────┤
│           FOOTER                    │
└─────────────────────────────────────┘
```

#### 2. Essay Page (THE most important page)
```
┌─────────────────────────────────────┐
│           NAVIGATION                │
├─────────────────────────────────────┤
│                                     │
│        Essay Title                  │
│        On: Book Title by Author     │
│        By: Contributor Name         │
│        12 min read                  │
│                                     │
│  ─────────────────────────────────  │
│                                     │
│     The full essay text.            │
│     Long-form. Uninterrupted.       │
│     Beautiful typography.           │
│     This is the entire point.       │
│                                     │
│  ─────────────────────────────────  │
│                                     │
│     🏪 Contributor's bookstore:     │
│     [Bookstore Name] — City, ST    │
│                                     │
│     About the contributor           │
│                                     │
│  ─────────────────────────────────  │
│                                     │
│     Related Essays                  │
│     ┌───────┐ ┌───────┐            │
│     │ Card  │ │ Card  │            │
│     └───────┘ └───────┘            │
│                                     │
├─────────────────────────────────────┤
│           FOOTER                    │
└─────────────────────────────────────┘
```

#### 3. Essay Index / Browse
```
┌─────────────────────────────────────┐
│           NAVIGATION                │
├─────────────────────────────────────┤
│                                     │
│     Essays                          │
│     [By Title] [By Author]          │
│     [By Contributor] [All]          │
│                                     │
│     ┌───────────────────────────┐   │
│     │ Essay Card                │   │
│     │ Title / Book / Contributor│   │
│     │ Excerpt... (2-3 lines)   │   │
│     │ 8 min read               │   │
│     └───────────────────────────┘   │
│     ┌───────────────────────────┐   │
│     │ Essay Card                │   │
│     └───────────────────────────┘   │
│     ┌───────────────────────────┐   │
│     │ Essay Card                │   │
│     └───────────────────────────┘   │
│                                     │
├─────────────────────────────────────┤
│           FOOTER                    │
└─────────────────────────────────────┘
```

---

## Essay Card Component

The essay card appears on the homepage, browse pages, and as related essays. It should contain:

- Essay title
- Book title and author
- Contributor name
- Excerpt (2-3 sentences)
- Reading time
- (Optional) Bookstore name

The card should invite clicking without feeling clickbait-y. Warmth over urgency.

---

## Imagery

### Approach: Minimal
- **No stock photography.** Nothing generic.
- Consider: texture, paper grain, or subtle illustrated elements as background accents
- Contributor photos: optional, black & white if used, to maintain visual cohesion
- Book cover images: only if rights allow, and only on book-specific pages (P2)

### If illustrations are used:
- Hand-drawn, literary feel — think bookplates, woodcuts, line drawings
- Used sparingly as accent, never as hero images competing with the text

---

## Components to Design

### Priority 1 (Must Have)
1. **Navigation bar** — simple, warm, not corporate
2. **Essay card** — the primary content unit on browse/home pages
3. **Essay page layout** — the full reading experience
4. **Homepage** — manifesto, featured essay, recent essays, CTA
5. **Footer** — secondary nav, subscribe link, manifesto snippet or tagline
6. **Subscribe form** — email capture, minimal, inline or modal
7. **Submission page** — guidelines + contact method

### Priority 2 (Should Have)
8. **Essay taxonomy browser** — filter tabs or sidebar
9. **Bookstore callout component** — the linked bookstore badge on essay pages
10. **Featured essay treatment** — how it looks differently on the homepage
11. **Mobile layouts** for all of the above

### Priority 3 (Nice to Have)
12. **Events page layout**
13. **Contributor profile page**
14. **Book aggregation page**
15. **404 page** (make it charming)

---

## Responsive Breakpoints

| Breakpoint | Target |
|-----------|--------|
| 320-480px | Mobile (reading on phone — must be excellent) |
| 481-768px | Tablet |
| 769-1024px | Small desktop |
| 1025px+ | Desktop |

Mobile reading experience is critical. Many people read long-form content on their phones. The essay page on mobile must be just as beautiful as on desktop.

---

## Mood & Inspiration

Places to look for design inspiration:

- **The Marginalian** (themarginalian.org) — literary, warm, reading-focused
- **Longreads** (longreads.com) — clean essay presentation
- **The Paris Review** (theparisreview.org) — classic literary design
- **Electric Literature** (electricliterature.com) — modern literary web
- **Independent bookstore websites** — Powell's, Strand, Tattered Cover
- **Print design:** The interior layout of a well-typeset novel. The colophon page. Endpapers.

---

## What This Site Is NOT

- Not a social media platform (no comments, no likes, no engagement metrics visible)
- Not a blog (it's a curated collection, not a chronological feed)
- Not an e-commerce site (the shop is a future add-on, not the focus)
- Not a news site (no urgency, no ticker, no "trending")

The closest analogy is a literary journal — curated, beautiful, meant to be read slowly.

---

## Deliverables Requested

1. **Style tile** — colors, typography, textures, component samples on one board
2. **Homepage** — desktop and mobile
3. **Essay page** — desktop and mobile (the hero deliverable)
4. **Essay browse/index** — desktop and mobile
5. **Submission page** — desktop
6. **Component library** — cards, buttons, nav, footer, forms, bookstore badge
