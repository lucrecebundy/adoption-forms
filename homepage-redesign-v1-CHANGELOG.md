# Adoption Forms Express — Homepage Redesign — Change Log Archive

**Companion to:** `homepage-redesign-v1.md`
**Purpose:** Historical change-log entries for the homepage spec doc. Split out 2026-05-01 to keep the main doc under the auto-load size threshold. The homepage doc keeps only the most recent ~5 entries; everything older lives here.

**How to use this file:**
- Append-only — never edit past entries.
- When the homepage doc's in-line change log grows past ~5–7 entries, move the older entries here.
- Read this file when you need full homepage history (e.g., "when did the testimonial three-up change?").

---

## Homepage Change Log — Archived Entries

| Date | Change | Author |
|---|---|---|
| 2026-04-28 | v1.0 — Initial homepage redesign spec drafted (full document) | Claude / Tyler |
| 2026-04-28 | v1.1 — Added Executive Summary section near top covering biggest changes vs. current site, layered keyword strategy, and AI search optimization principles | Claude / Tyler |
| 2026-04-28 | v2.0 — Built `homepage.html`: single self-contained HTML file, inline CSS using master design tokens, Fraunces + Manrope typography, JSON-LD schema (LegalService, AggregateRating, FAQPage), CSS-only animations on hero, vanilla JS FAQ accordion. Hero photo: 497A2248-scaled.jpg. Founder spotlight photo: 497A2015-scaled.jpg. WordPress-ready. | Claude / Tyler |
| 2026-04-29 | v2.1 — Cross-doc consistency edits to align with DFY package changes: (1) timeline updated 2–4 months → 4–6 months in How It Works step 4 and FAQ Q2; (2) "Waiver of Notice" removed from Section 5.10 forms list; (3) attorney call line clarified as "scoped to questions about your forms" in Section 5.10 and both pricing cards. **Homepage HTML still needs matching edits — flagged for next build session.** | Claude / Tyler |
| 2026-04-29 | v2.2 — Review count updated 118 → 142 across the doc and homepage HTML (4 places in HTML: schema markup `reviewCount`, hero credibility line, hero image badge, trust strip; 6 places in doc: executive summary, hero copy, trust strip, founder credibility, lead-in to reviews section, AggregateRating schema spec). **Note: review count is currently hardcoded — see new master open decision about live-feed integration.** | Claude / Tyler |
| 2026-04-29 | v2.3 — Visible review count rounded to "140+" in 4 HTML spots and 5 visible doc spots (resolves master open decision #19, option B). Schema markup `reviewCount` retains exact 142 (Google schema requires precise numerics; not visitor-facing). | Claude / Tyler |
| 2026-04-29 | v2.4 — Section 5.11 three-up testimonials swapped from Shawri/Kristin/Halewya to Catherine Day, Kevin Shafer, Sarah Hall. Homepage HTML updated to match. Featured testimonial (Amanda) unchanged. Each new card hits a different angle: Catherine (authority claim — "more knowledgeable than any other family law"), Kevin (post-purchase satisfaction + "would use again"), Sarah ("handled everything for us" — DFY product promise). Catherine's review is truncated; pull full text from Google before final HTML build. | Claude / Tyler |
| 2026-04-29 | v2.5 — Sarah Hall swapped out for Ruby Leonard in three-up. Reason: Ruby's review is the only Google review in the entire 142-review set that explicitly mentions purchasing the DIY adoption documents as a product — strongest single asset for forms-product social proof. New trio: Catherine (authority), Kevin (satisfaction + use again), Ruby (forms-product validation). Sarah Hall's testimonial moved into reserve for future DIY checkout page. Notes section updated to flag Ruby's strategic uniqueness. | Claude / Tyler |
| 2026-04-29 | v2.6 — Catherine Day full review text now in spec and HTML. Used a curated excerpt that includes the strongest line from her review ("she said she handled everything, and boy, she was not lying. In the end, all I had to do essentially, was pay and show up to the court") which is arguably the single most powerful customer-voice line on the entire homepage. Untruncated. | Claude / Tyler |
| 2026-04-29 | v2.7 — Featured testimonial restructured: Kristin's testimonial now serves as the featured pull quote, paired with her circular photo (URL: `/wp-content/uploads/2026/04/Kristin.png`). Amanda's "$10K + 3 lawyers" testimonial moved into the three-up as card 2 (replacing Kevin Shafer). Kevin moves to testimonial reserve. New CSS class `.review-featured-photo` added to homepage HTML for circular photo styling (88px, white border, soft shadow). The featured testimonial is the only one with a photo by design — creates a single visual anchor for the social-proof section. Photo-release note added flagging the need to document Kristin's marketing-use consent. | Claude / Tyler |

---

*End of archived entries — see `homepage-redesign-v1.md` Section 11 for the most recent ~5 entries.*
