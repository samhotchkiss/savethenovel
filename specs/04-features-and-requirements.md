# Save the Novel — Features & Requirements

## P0 — Must Have for Launch

### 1. Homepage
- Manifesto / mission statement prominently displayed
- Featured essay of the month with full presentation
- Recent essays grid (3-4 cards with title, book, contributor, excerpt)
- **News on Reading** — curated section with links to articles about novel reading, literacy, the literary landscape
- Call to action: Read, Submit, Subscribe
- Link to mailing list signup

### 2. Essay Pages
- Full long-form essay display with quality typography
- **No reading time estimate.** *"We read because it's timeless, not because it's measured."*
- Book title and author (author name linked if they have a profile)
- Contributor name (linked to their website/Substack if available)
- Contributor's favorite independent bookstore (name + link to store website)
- Related essays (same book, same author, or same contributor)
- Social sharing (minimal — link copy, maybe email)

### 3. Essay Browsing
- Default view: all essays, reverse chronological
- Browse by Book Title (alphabetical grouping)
- Browse by Book Author (alphabetical grouping)
- Browse by Contributor (alphabetical grouping)
- Browse by Publication Date (chronological)
- Essay cards: title, book, contributor, excerpt

### 4. Submission Flow
- Dedicated submission page with clear guidelines
- Contribution FAQ: what we're looking for, length expectations, editorial process, rights/licensing
- Contact method for submissions (form or email — see Open Questions)

### 5. About Page
- About S.E. Elkins
- About the project's origin (Southwest bookstore events)
- The vision and mission

### 6. FAQ Page
- Rules for contribution
- What makes a good essay for this site
- Editorial process and timeline
- Rights and licensing (does the contributor retain rights?)
- Can I write about a book someone else already wrote about? (Yes — that's the point)

### 7. Mailing List
- Email signup form (embedded or linked)
- Monthly featured essay sent to subscribers
- Emails originate from the site (not Substack)
- Substack cross-post handled separately (manual or automated)

### 8. News on Reading
- Curated section (homepage + dedicated page) with links to external articles about novel reading
- Articles about literacy, the state of reading, novel culture, the literary landscape
- Editorially curated by S.E. Elkins — not an automated feed

### 9. Resources for Readers & Educators
- Resources for educators who want to teach novels in their classrooms
- Resources for people who never learned to read long-form in school
- Potential viral content: "How to Read a Book" guide by S.E. Elkins
- Links to curricula, reading guides, and advocacy organizations

### 10. Responsive Design
- Mobile-first reading experience
- Long-form essays must be comfortable to read on phone, tablet, desktop
- Generous typography, appropriate line length, good contrast

## P1 — Should Have (Soon After Launch)

### 11. Featured Archive
- Chronological archive of previously featured essays
- Month/year label for each
- Accessible from footer navigation or a dedicated page

### 12. Bookstore Directory
- Aggregated view of all independent bookstores linked from essays
- Each bookstore shows: name, location, website, number of essays linking to it
- Creates goodwill and incentive for bookstores to promote the site

### 13. Search
- Full-text search across essay titles, book titles, authors, contributors
- Search results show essay cards

### 14. Print Stylesheet
- Clean print layout for essays
- Readers who love novels also love paper — respect that

### 15. RSS Feed
- For readers who still use RSS (and these readers definitely do)

## P2 — Nice to Have (Future)

### 16. Merchandise Shop
- "I come from the library" bumper stickers
- Potentially other literary-themed merchandise
- Could be a simple Shopify embed or external link initially

### 17. Events Page
- Upcoming bookstore reading events
- "Let the Reader Speak" events — Southwest (current), East Coast tour (Fall 2026)
- Past events archive

### 18. Contributor Profiles
- Dedicated page for contributors with multiple essays
- Bio, website link, all their essays, their bookstore picks

### 19. Book Pages
- Aggregated view for books with multiple essays
- All essays about *Beloved*, for example, on a single page
- Book cover image (if rights allow)

### 20. Automated Substack Sync
- Automatic cross-posting of featured essay to Substack Notes
- Or: automated check/copy of Substack email list (as S.E. mentioned)

## Non-Functional Requirements

### Performance
- Fast initial load — readers shouldn't wait to start reading
- Static site generation preferred (essays don't change frequently)
- Images optimized and lazy-loaded

### Accessibility
- WCAG 2.1 AA compliance
- Semantic HTML structure
- Screen reader friendly navigation
- Sufficient color contrast for long reading sessions
- Keyboard navigable

### SEO
- Proper meta tags for each essay (title, description, open graph)
- Structured data for articles (schema.org)
- Clean, crawlable URLs
- Sitemap

### Analytics
- Basic traffic analytics (privacy-respecting: Plausible, Fathom, or similar)
- Track: page views, essay reads, bookstore link clicks, newsletter signups

### Hosting
- GitHub Pages compatible (or similar static hosting)
- Custom domain: savethenovels.org
- SSL/HTTPS

### Content Management
- Whoever manages the site needs a way to add new essays without writing code
- Options: headless CMS, markdown files with a build step, or a simple admin interface
- See Open Questions document for CMS decision
