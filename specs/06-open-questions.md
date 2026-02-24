# Save the Novel — Open Questions & Recommendations

Questions that need to be resolved before or during development. Each includes our recommendation.

---

## 1. Tech Stack / Platform

**Question:** What platform and tech stack should the site be built on?

**Options:**
- **A) Static site generator (Astro, Hugo, Eleventy) + Markdown files** — Essays stored as Markdown in a Git repo, built to static HTML. Simple, fast, free to host.
- **B) Static site generator + Headless CMS (Sanity, Contentful, Decap CMS)** — Same static output, but content is managed through a visual editor rather than Markdown files.
- **C) WordPress** — The default. Huge ecosystem, easy for non-technical editors. Heavier, requires hosting.
- **D) Squarespace / Webflow** — No-code platforms. Fast to launch, limited customization.
- **E) Next.js / Remix + database** — Full-stack framework. Maximum flexibility, most complex.

**Recommendation: B — Static site generator (Astro) + Headless CMS (Decap CMS or Sanity)**

Why: The site's content is essays that change infrequently. Static is the right architecture — fast, secure, cheap to host. But S.E. needs to add essays without touching code. A headless CMS gives her a visual editor while keeping the site static. Decap CMS (formerly Netlify CMS) is free and works with GitHub — essays are still Markdown files in the repo, but edited through a browser UI. Astro is ideal because it's content-focused by design, outputs zero JavaScript by default, and has excellent Markdown support.

If simplicity is paramount, even a basic Eleventy + Decap CMS setup would work beautifully.

**Caveat:** If S.E. or her team has WordPress experience and strong preference, WordPress is perfectly fine. Don't fight familiarity for purity.

---

## 2. ~~Singular vs. Plural~~ — RESOLVED

**Answer:** **Save the Novels** (plural). Domain: **savethenovels.org**

---

## 3. Domain Name

**Question:** What domain should the site live at?

**Options to investigate:**
**RESOLVED:** Domain registered — **savethenovels.org**

This also resolves the singular vs. plural question: it's **Save the Novels** (plural).

---

## 4. Essay Submission Method

**Question:** How should contributors submit their essays?

**Options:**
- **A) Email** — Contributors email their essay to a dedicated address (submit@savethenovels.org). S.E. handles intake manually.
- **B) Web form** — A form on the site where contributors paste or upload their essay text, along with metadata (bio, bookstore, website).
- **C) Google Form** — Quick to set up, familiar to everyone, responses collected in a spreadsheet.
- **D) Submittable / similar platform** — Purpose-built literary submission tool. Some cost.

**Recommendation: A (email) for launch, with B (web form) as a P1 improvement.**

Why: At launch, the volume will be manageable — mostly people S.E. already knows from bookstore events. Email is personal, which matches the project's ethos. A web form can be added once submission volume warrants it. A Google Form is a fine interim solution if she wants more structure than raw email.

---

## 5. Essay Length & Display

**Question:** These are long-form essays. How do we handle length on the site?

**Considerations:**
- Average essay might be 1,500-3,000 words, some could be 5,000+
- The whole point is long-form, deep reading — truncation would be hypocritical

**Recommendation:** Display the full essay on its own page, always. No "read more" truncation — that contradicts the mission. On index/browse pages, show a 2-3 sentence excerpt (manually curated, not auto-truncated).

**No reading time estimates anywhere.** S.E. was explicit: *"We read because it's timeless, not because it's measured."* This is philosophically correct for this project.

For very long essays (5,000+), consider a subtle floating table of contents or progress indicator — but never break the essay across multiple pages.

---

## 6. Mailing List Provider

**Question:** What email service should power the mailing list?

**Options:**
- **A) Buttondown** — Simple, Markdown-native, affordable, indie-spirited. Fits the ethos.
- **B) ConvertKit (now Kit)** — Creator-focused, good automation, free tier up to 10K subscribers.
- **C) Mailchimp** — The default. Free tier exists. More complex than needed.
- **D) Substack directly** — Already has a Substack. Could just use that.

**Recommendation: A (Buttondown) or B (ConvertKit)**

Why: S.E. explicitly said she'd prefer emails to come from the site directly, with Substack as a mirror. Buttondown is beautifully simple and Markdown-native — perfect for sending a literary essay once a month. ConvertKit is more feature-rich if she wants automations or segmentation later.

**Substack relationship:** Cross-post the monthly essay to Substack as a Note manually. Don't try to automate this initially — it's once a month.

---

## 7. Substack Sync

**Question:** S.E. mentioned wanting to check the Substack email list and copy it. How should the Substack and site mailing lists relate?

**Recommendation:** Keep them separate but complementary.

- **Site mailing list** = the primary list, owned by S.E., lives on her email provider
- **Substack** = a secondary distribution channel and discovery platform

Don't try to sync them technically. Instead:
1. On the Substack, link prominently to the main site
2. On the site, offer both: "Subscribe via email" (primary) and "Follow on Substack" (secondary)
3. Monthly featured essay goes to both, but the site email is the canonical send

Trying to automatically sync subscriber lists between platforms is fragile and often violates terms of service.

---

## 8. Rights & Licensing

**Question:** What rights does Save the Novel hold to published essays?

**Things to decide:**
- Does the contributor retain full rights to their essay?
- Is Save the Novel granted a non-exclusive license to publish?
- Can contributors also publish their essay elsewhere (their own blog, a magazine)?
- What about collected editions — could these essays become a book someday?

**Recommendation:** Contributors retain all rights. Save the Novel gets a non-exclusive, perpetual license to publish on the site and in the newsletter. Contributors are free to publish their essay anywhere else. This is the most generous and author-friendly approach, which is on-brand for a project called "Save the Novel."

If there's any future aspiration to compile essays into a book, include language about that possibility in the contributor agreement — even if it's just "we may someday want to publish a collected edition, and we'll reach out to each contributor individually for permission."

**Action item:** Have a lawyer review a simple contributor agreement. This doesn't need to be complex.

---

## 9. Editorial Voice & Tone

**Question:** How much editing will S.E. do on submitted essays?

**Considerations:**
- Too much editing loses the authentic voice
- Too little risks inconsistent quality
- Some contributors will be published authors; others won't

**Recommendation:** Light editorial touch. Fix typos and grammatical errors, suggest structural improvements, but preserve each contributor's voice completely. The raw, personal quality IS the content. Consider having a brief editorial note at the top of the FAQ explaining the editorial philosophy.

---

## 10. Design Aesthetic

**Question:** What should the site look and feel like?

**Direction (confirmed by S.E. in strategy session):**
- **Earth tones, organic feeling** — confirmed directly
- **Not shiny, not high-tech** — no cool-tone gradients, nothing that feels like a tech startup
- Literary, warm, unhurried
- Reading-first design — the essays are the product
- Think: independent bookstore, not Amazon

**S.E. wants to see design samples/options** before committing to a specific palette. Present 2-3 directions.

**Recommendation:** Warm color palette (creams, deep greens, muted earth tones). Serif font for body text (this is a site about novels — serif is correct). Generous whitespace. No visual clutter. The design should feel like opening a book.

---

## 11. Hosting & Deployment

**Question:** Where should the site be hosted?

**Options:**
- **A) GitHub Pages** — Free, simple, works with static sites. This repo is already structured for it.
- **B) Netlify** — Free tier, great DX, built-in form handling, CMS integration.
- **C) Vercel** — Similar to Netlify, more focused on Next.js/React.
- **D) Traditional hosting** — If WordPress is chosen.

**Recommendation: B (Netlify) for production, A (GitHub Pages) for the spec/explainer docs.**

Why: Netlify pairs naturally with Decap CMS (they created it). Free tier is more than sufficient. Automatic deploys from Git. Built-in form handling could replace a dedicated submission form. GitHub Pages is great for the project documentation (this repo).

---

## 12. Social Media Presence

**Question:** Does Save the Novel need social media accounts?

**Recommendation:** Yes, but minimal. One account, probably Instagram — it's where book culture thrives (#bookstagram). Use it to:
- Share pull quotes from essays
- Promote bookstore events
- Share contributor photos and stories
- Announce new essays

Don't spread across every platform. One channel, done well, is plenty. The site and newsletter are the primary channels.

---

## 13. Future Merch Shop

**Question:** When and how to add the "I come from the library" bumper stickers and other merch?

**Recommendation:** Don't build a shop. Use a third-party print-on-demand service (Shopify Lite, Big Cartel, or even Etsy) and link to it from the site. This can happen anytime post-launch and doesn't need to be part of the core site architecture.

---

## 14. Multiple Essays About the Same Book

**Question:** Can more than one person write about the same novel?

**Answer:** Absolutely yes. This should be celebrated, not avoided. If five people write about how *Beloved* changed their lives, that's five different windows into the same masterwork. The site architecture already supports this — the book page aggregation (P2 feature) would beautifully showcase this.

---

## 15. Analytics & Privacy

**Question:** How much do we want to track, and how?

**Recommendation:** Use a privacy-respecting analytics tool (Plausible or Fathom). No cookies, no tracking pixels, no Google Analytics. This audience cares about ethics and privacy. The key metrics are:
- Which essays get read
- Which bookstore links get clicked
- Newsletter signup conversion
- Referral sources (are bookstores driving traffic?)

---

## Decision Priority

| # | Question | Urgency | Blocks |
|---|----------|---------|--------|
| 2 | ~~Singular vs. plural~~ | **RESOLVED** | savethenovels.org (plural) |
| 3 | ~~Domain name~~ | **RESOLVED** | savethenovels.org |
| 1 | Tech stack | **Now** | Everything else |
| 8 | Rights & licensing | **Before outreach** | Contributor agreements |
| 10 | Design aesthetic | Before design (March) — S.E. wants samples | Figma work |
| 4 | Submission method | Before launch | Submission page design |
| 6 | Mailing list provider | Before dev (April) | Newsletter integration |
| 11 | Hosting | Before dev (April) | Deployment pipeline |
| 5 | Essay length | Already decided | No reading time — resolved |
| 7 | Substack sync | Post-launch OK | Nothing critical |
| 9 | Editorial voice | Ongoing | Nothing technical |
| 12 | Social media | Pre-launch | Nothing technical |
| 13 | Merch shop | Post-launch | Nothing |
| 14 | Same-book essays | Already answered | Nothing |
| 15 | Analytics | During dev | Nothing critical |
