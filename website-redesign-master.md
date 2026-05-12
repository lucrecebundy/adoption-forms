# Adoption Forms Express — Website Redesign Master Document

**Document type:** Master / index for the entire site redesign
**Owner:** Lucrece H. Bundy / Tyler
**Site:** adoptionformsexpress.com
**Version:** 1.23
**Last updated:** May 12, 2026
**Status:** Active

---

## How This Document Works

This is the **master file** for the Adoption Forms Express redesign. It lives *above* the page-level working documents (homepage, qualifier quiz, pricing, etc.) and holds everything that applies across the whole site:

- Project goals and north star
- Brand voice and UPL guardrails (apply to every page)
- Visual system / design tokens (apply to every page)
- SEO foundation and master keyword list
- Tech stack and integrations
- Site architecture and page-by-page status
- Master roadmap, open decisions, and change log
- An index of every companion document

**Page-level docs** (e.g., `homepage-redesign-v1.md`) hold page-specific copy, layout, and schema. They defer to this master on anything site-wide. If something here conflicts with a page doc, this document wins.

### How to use it in a session

1. **Open this file first** at the start of every Claude Code, Cowork, or chat session.
2. Read the **Master Open Decisions** and **Master Change Log** to see what changed since last session.
3. Open the **page-level doc** for whatever you're working on.
4. At the end of the session, log changes here AND in the page-level doc.

### Naming convention for companion docs

`[page-or-area]-[type]-v[X].md` — e.g., `homepage-redesign-v1.md`, `qualifier-quiz-v1.md`, `county-landing-pages-v1.md`.

---

## 1. Project Goals & North Star

### Business goal

Move Adoption Forms Express from a side product into the **primary business** so Lucrece can phase out active courtroom practice. The website is the customer-acquisition engine — its job is to qualify, convert, and deliver.

### Site goals (in priority order)

1. **Convert qualifying Nebraska families** into form purchases (DIY $299 or Done-For-You $499).
2. **Build search authority** — rank #1 for Nebraska stepparent adoption queries on Google AND surface in AI search (ChatGPT, Claude, Perplexity, Google AI Overviews).
3. **Protect attorney trust** — every page must signal real Nebraska attorney expertise without creating UPL exposure.
4. **Route non-fits cleanly** — visitors who don't qualify get referred to Bundy Law LLC for contested or complex cases (revenue stays in the family of businesses).

### Success metrics (track from launch)

- Conversion rate (visitor → qualifier started)
- Qualifier completion rate (started → qualified)
- Purchase rate (qualified → paid)
- Average order value (DIY mix vs. DFY mix)
- Organic search traffic from Nebraska
- Featured-snippet wins for target queries
- AI search visibility (manual checks: ChatGPT, Perplexity, Google AI Overviews)
- Bundy Law referral conversions from disqualified visitors

---

## 2. Site Architecture & Page Status

Every page on the redesigned site, what it's for, what doc holds its spec, and where it stands.

| Page | URL | Purpose | Doc | Status |
|---|---|---|---|---|
| Homepage | `/` | Top of funnel, qualifier entry | `homepage-redesign-v1.md` + `homepage.html` | 🟢 Built, testimonials locked, ready for review and deploy |
| Qualifier quiz | `/qualify` | 60-second eligibility quiz | `qualifier-quiz-v1.md` | ⚪ Not started |
| Pricing | `/pricing` | Standalone pricing comparison | `pricing-page-v1.md` | ⚪ Not started |
| DFY sales page — minor child | `/dfy-minor-sales-page/` | Post-quiz sales page (gated, noindex). Two CTA buttons link to the checkout page. | `dfy-minor-child-page-v1.md` + `dfy-minor-child.html` | 🔵 Built — ready for WordPress deploy |
| DFY checkout — minor child | `/dfy-child-check-out-page/` | Transactional checkout (gated, noindex, ThriveCart embed). Only place ThriveCart loads. Sibling top-level page to the sales page (not a child page). | `dfy-minor-child-page-v1.md` + `dfy-minor-child-checkout.html` | 🔵 Built — ready for WordPress deploy |
| DFY sales — adult | `/dfy-adult-sales-page/` | Post-quiz sales page (gated, noindex). Two CTA buttons link to the future adult checkout page. | `dfy-adult-page-v1.md` + `dfy-adult.html` | 🔵 Built — ready for WordPress deploy |
| DFY checkout — adult | `/dfy-adult-checkout-page/` | Transactional checkout (gated, noindex, ThriveCart embed — product 8). Only place ThriveCart loads. Sibling top-level page to the sales page. | `dfy-adult-page-v1.md` + `dfy-adult-checkout.html` | 🔵 Built — ready for WordPress deploy |
| DIY sales — minor child | `/diy-minor-sales-page/` | Post-quiz sales page (gated, noindex). Two CTA buttons link to the DIY checkout page. | `diy-minor-child-page-v1.md` + `diy-minor-child.html` | 🔵 Built — ready for WordPress deploy |
| DIY checkout — minor child | `/diy-minor-checkout-page/` | Transactional checkout (gated, noindex, ThriveCart embed — product 4). Only place ThriveCart loads. Sibling top-level page to the sales page. | `diy-minor-child-page-v1.md` + `diy-minor-child-checkout.html` | 🔵 Built — ready for WordPress deploy |
| DIY sales — adult | `/diy-adult-sales-page/` | Post-quiz sales page (gated, noindex). Two CTA buttons link to the DIY adult checkout page. | `diy-adult-page-v1.md` + `diy-adult.html` | 🔵 Built — ready for WordPress deploy |
| DIY checkout — adult | `/diy-adult-check-out-page/` | Transactional checkout (gated, noindex, ThriveCart embed — product 7). Only place ThriveCart loads. Sibling top-level page to the sales page. | `diy-adult-page-v1.md` + `diy-adult-checkout.html` | 🔵 Built — ready for WordPress deploy |
| DFY pillar (public SEO) | `/done-for-you-adoption-forms-nebraska/` | Indexed pillar page funneling to quiz | `dfy-pillar-page-v1.md` | ⚪ Not started |
| Adult adoption pillar (public SEO) | `/adult-stepparent-adoption-nebraska/` | Indexed pillar page targeting underserved adult-adoption keywords | `adult-adoption-pillar-v1.md` | ⚪ Not started |
| About / Founder | `/about` | Lucrece bio, firm story, credentials | `about-page-v1.md` | ⚪ Not started |
| How It Works | `/how-it-works` | Long-form process walkthrough | `how-it-works-v1.md` | ⚪ Not started |
| FAQ (full) | `/faq` | Expanded FAQ standalone page | `faq-page-v1.md` | ⚪ Not started |
| County landing pages | `/counties/[county-slug]` | Local SEO — 1 page per priority county | `county-landing-pages-v1.md` | ⚪ Not started |
| Blog | `/blog` | SEO content engine | `seo-content-calendar-v1.md` | ⚪ Not started |
| Conversational AI intake | TBD | Phase 3 AI flow replacing/augmenting qualifier | `conversational-ai-intake-v1.md` | ⚪ Not started |
| Lead magnet landing | `/starter-guide` | Email capture + free PDF ("Free Nebraska Adoption Guide") | `lead-magnet-v1.md` | ⚪ Not started — but already referenced as the secondary CTA on homepage (hero + final CTA + FAQ footnote) and in the homepage + DFY footer. Currently stubbed to `#` in HTML. |
| Terms of Use | `/terms-of-use/` | Legal — same content as live page, with the old "No Refunds" section replaced by a new "Refunds" section that defers to the Refund Policy page | `legal-pages-v1.md` + `terms-of-use.html` | 🔵 Built — ready for WordPress deploy |
| Privacy Policy | `/privacy-policy/` | Legal — content preserved verbatim from the live page, emails standardized to `info@adoptionformsexpress.com` | `legal-pages-v1.md` + `privacy-policy.html` | 🔵 Built — ready for WordPress deploy |
| Refund Policy | `/refund-policy/` | Legal — brand new page covering 7-day eligibility window, pre/post-delivery distinction, request mechanism, exceptions. NOT linked from site footer per Decision #22 — surface via post-purchase invoice/receipt only. | `legal-pages-v1.md` + `refund-policy.html` | 🔵 Built — ready for WordPress deploy |
| 404 / Disqualified | `/not-a-fit` | Where disqualified visitors land | `disqualified-routing-v1.md` | ⚪ Not started |

**Status legend:** ⚪ Not started · 🟡 In draft · 🟠 In review · 🟢 Locked / build-ready · 🔵 Built · ✅ Live

---

## 3. Brand & Voice (Site-Wide)

### Voice principles

- **Warm but authoritative.** This is an emotional decision (legalizing parenthood) handled by a real attorney. Both notes must be present in every paragraph.
- **Plain English.** No "wherefores" or "heretofores." If a sentence sounds like it came from a contract, rewrite it.
- **Honest about fit.** We say out loud when DIY isn't right. This is the opposite of pressure-selling and it's our biggest differentiator.
- **Confident in the product.** No hedging language ("we hope," "we try," "should work"). The forms work. They've worked 200+ times.

### Words we use

family · blended family · already · finally · officially · attorney-prepared · Nebraska-specific · qualifying families · the parent you already are

### Words we avoid

- "Cheap" (use "affordable" or just price specifics)
- "Loophole" (creates legal red flags)
- "Guaranteed" (UPL risk — never promise legal outcomes)
- "Easy" by itself (sounds like minimization of an emotional process — pair with "straightforward" or "designed to make this less overwhelming")

### UPL guardrails (NON-NEGOTIABLE — apply to every page)

1. **Footer disclaimer must appear on every page:**
   *"Adoption Forms Express provides access to independent attorneys and self-service tools. We are not a law firm and do not provide legal advice. Use of our products and services are governed by our Terms of Use and Privacy Policy. The forms provided are intended for use in uncontested Nebraska stepparent adoption cases. If your case is contested or your situation is unusual, you should consult a licensed attorney."*
2. **No language that promises a specific legal outcome** ("guaranteed adoption," "your case will succeed").
3. **Distinguish the product from the law firm.** Adoption Forms Express ≠ Bundy Law LLC. They share a founder, not a legal entity.
4. **No personalized legal advice on the site.** Educational content is fine. "Here's what your specific case should do" is not.
5. **Contested cases must always route out** to Bundy Law LLC or a general consult — never to the DIY product.
6. **The qualifier quiz is the legal-fitness gate** and must remain conservative: when in doubt, route to consult, not to checkout.

### Compliance review trigger

Any new page or significant copy change requires a 5-minute UPL re-read by Lucrece before publishing. Log it in the page doc's change log.

---

## 4. Visual System (Site-Wide Design Tokens)

These tokens apply to every page. Page docs do not redefine — they reference.

### Color palette (proposed — confirm in Phase B)

| Token | Hex | Use |
|---|---|---|
| `--color-primary` | `#1F3A5F` | Headings, primary brand, navigation |
| `--color-accent` | `#E07856` | CTAs, highlights, the one button color |
| `--color-bg` | `#FAF7F2` | Page background |
| `--color-bg-alt` | `#FFFFFF` | Card / section alternates |
| `--color-text` | `#1A1A1A` | Body copy |
| `--color-text-muted` | `#6B6B6B` | Captions, secondary text |
| `--color-success` | `#7A9E7E` | Checkmarks, qualifier "yes" states |
| `--color-border` | `#E5E1DA` | Section dividers, card outlines |

### Typography

- **Headings:** Lora, Source Serif Pro, or Fraunces (decide in Phase B). Serif communicates warmth + authority.
- **Body:** Inter or Open Sans. Humanist sans for readability.

**Type scale (desktop / mobile):**

| Element | Desktop | Mobile |
|---|---|---|
| H1 | 48px | 32px |
| H2 | 36px | 26px |
| H3 | 24px | 20px |
| Body | 18px | 16px |
| Small | 14px | 14px |

### Layout principles

- Mobile-first — assume 70%+ traffic is on phones.
- Generous white space — adoption is emotional; the page should feel calm, not pushy.
- **One CTA color** site-wide. No competing buttons.
- Maximum content width ~1200px on desktop.
- Sticky nav with single primary CTA always visible.

### Imagery direction

- Real Nebraska families when possible (with consent + photo release).
- Lucrece's professional headshot is canonical — use the same photo across founder appearances.
- Avoid generic stock "happy family" imagery. If stock is necessary, choose images that feel Midwestern, multi-ethnic, real-light, real-homes.

---

## 5. SEO Foundation (Site-Wide)

### Master keyword tiers

**Tier 1 — Primary (target on homepage + pillar pages):**
- nebraska stepparent adoption
- nebraska stepparent adoption forms
- stepparent adoption forms nebraska
- nebraska adoption forms

**Tier 2 — Secondary (target on pillar pages + supporting content):**
- nebraska stepparent adoption cost
- nebraska stepparent adoption process
- nebraska stepparent adoption requirements
- diy stepparent adoption nebraska
- stepparent adoption without a lawyer nebraska
- nebraska adoption attorney alternative
- how long does stepparent adoption take in nebraska
- nebraska adoption laws

**Tier 3 — Long-tail / question (target in FAQ + blog):**
- how to do a stepparent adoption in nebraska
- how much does a stepparent adoption cost in nebraska
- can i do a stepparent adoption without a lawyer in nebraska
- what forms do i need for a stepparent adoption in nebraska
- what if the other parent won't consent to stepparent adoption nebraska
- how to file for stepparent adoption in nebraska

**Tier 4 — Local (target on county landing pages):**
- douglas county stepparent adoption · omaha stepparent adoption attorney
- lancaster county stepparent adoption · lincoln stepparent adoption attorney
- sarpy county stepparent adoption · bellevue / papillion stepparent adoption
- hall county stepparent adoption · grand island stepparent adoption
- buffalo county stepparent adoption · kearney stepparent adoption
- scotts bluff county stepparent adoption
- madison county stepparent adoption · norfolk stepparent adoption
- platte county stepparent adoption · columbus stepparent adoption
- dodge county stepparent adoption · fremont stepparent adoption
- adams county stepparent adoption · hastings stepparent adoption

**Keyword assignment rule:** every page targets one Tier 1 OR Tier 2 keyword as primary, plus 2–3 supporting Tier 3 / Tier 4 keywords. Avoid keyword cannibalization — no two pages compete for the same primary keyword.

### AI search optimization (AEO / GEO) — site-wide principles

Every page should:

1. **Use question-format H2s and H3s** when possible. ChatGPT, Claude, Perplexity, and Google AI Overviews extract answers most easily from question-headed sections.
2. **Lead each section with a direct, factual answer.** First sentence = the answer. Following sentences = elaboration.
3. **Cite Nebraska statutes by name.** Reference Neb. Rev. Stat. § 43-101 et seq., § 43-104, etc. AI search rewards verifiable citations.
4. **Surface explicit numerics.** Costs ($299, $499, $3,000–$10,000), timelines (2–4 months), age requirements (19+, 10 years older), residency (6 months). AI summarizers extract numbers preferentially.
5. **Include comparison tables** where applicable. AI loves tables.
6. **Make author/expertise visible.** Lucrece's name + credential should appear on every page that gives substantive content.

### Schema markup strategy

Deploy these JSON-LD blocks where applicable:

| Schema type | Where |
|---|---|
| `Organization` / `LegalService` | Every page (in `<head>`) |
| `Person` (Lucrece) | Homepage, About, footer of every content page |
| `AggregateRating` | Homepage, About, Reviews page |
| `FAQPage` | Homepage, FAQ page, How It Works page |
| `BreadcrumbList` | Every page except homepage |
| `Article` | Every blog post |
| `Service` | Pricing page, How It Works page |
| `LocalBusiness` (with `areaServed`) | Each county landing page |

Master schema specs live in `homepage-redesign-v1.md` Section 8 and will be ported to a shared `schema-library-v1.md` once we have 3+ pages spec'd.

### Technical SEO baseline

- Mobile PageSpeed score 85+ (LCP < 2.5s, CLS < 0.1)
- Sitemap.xml auto-generated, submitted to Google Search Console + Bing Webmaster
- robots.txt allows all priority pages, blocks /wp-admin and staging
- Canonical tags on every page
- No duplicate content across county pages — each must be substantively unique
- Internal linking strategy: homepage → pillar pages → supporting content; county pages cross-link to each other and to homepage

---

## 6. Audience & Competitive Frame (Site-Wide)

### Target visitor

A married Nebraska resident in a blended family who:
- Just got quoted $3,000–$10,000 by a traditional adoption attorney
- Is searching late at night for a credible alternative
- Wants something safe (attorney-backed) but doesn't want to retain a lawyer for what feels like paperwork
- Has been the de facto parent for years and wants the legal status to match

### Competitive positioning

| Competitor | Their angle | Our advantage |
|---|---|---|
| stepparentadoptionforms.com | "100% Court Acceptance," 20+ yrs, multi-state | We're Nebraska-only; we have a face and a real bar credential |
| rapidadoption.com | 3-day turnaround, 15+ yrs, multi-state | Same — Nebraska-only + named attorney |
| Traditional Nebraska adoption attorneys | Full-service, $3K–$10K | We're 1/10 the cost for uncontested cases |
| LegalZoom-type sites | Generic, $200–$300, no review | We're attorney-prepared and Nebraska-specific |

### Our single-line positioning

**"Attorney-prepared Nebraska stepparent adoption forms — without the $5,000 attorney bill."**

Every page must support this positioning. Any page that doesn't is off-strategy.

---

## 7. Technical Foundation (Site-Wide)

### Stack decision (OPEN — see Decisions)

Two paths under consideration:

**Path A — Stay on WordPress.** Faster to ship, lowest disruption, existing funnel keeps working. Use a refreshed theme + custom child theme. Best if we want the homepage redesign live in 4–6 weeks.

**Path B — Migrate to Next.js (or similar).** Better long-term performance, easier to integrate the Phase 3 conversational AI intake, easier to deploy schema. Best if we believe the AI intake build is happening within 6 months.

**Recommended for now:** Path A for the redesign launch, with the AI intake potentially built as a Next.js subdomain or embedded widget. Lock the decision in the next session.

### Analytics & tracking (deploy site-wide)

- Google Analytics 4
- Microsoft Clarity (free heatmaps + session recording)
- Google Search Console
- Bing Webmaster Tools

**Conversion events to fire:**
- `qualifier_quiz_start`
- `qualifier_quiz_complete`
- `qualifier_quiz_qualified`
- `qualifier_quiz_disqualified` (with `disqualifier_reason`)
- `forms_purchase_initiated` (with `product` = DIY or DFY)
- `forms_purchase_completed`
- `bundy_law_referral_clicked`
- `lead_magnet_downloaded`

### Integrations

**Currently in place (audit needed):**
- Existing qualifier form — confirm tool (Gravity Forms? Typeform?)
- Invoice / payment system — confirm tool (Stripe? PayPal?)
- Trustindex review widget
- Email — `info@adoptionformsexpress.com` (canonical site-wide contact as of 2026-05-12; replaced the legacy `adoptionformsexpress@gmail.com` Gmail)

**Planned additions:**
- Email automation (ConvertKit or MailerLite) for lead magnet + post-purchase sequence
- Conversational AI intake (Phase 3)
- Calendly or similar for the support calls
- Schema markup deployment

### Performance targets

- LCP < 2.5s on mobile
- CLS < 0.1
- Mobile PageSpeed 85+
- WebP images, lazy-load below the fold
- Critical CSS inlined, deferred non-critical CSS

---

## 8. Master Roadmap

### Phase A — Copy lock (current phase)

- [x] Homepage redesign drafted (v1.1)
- [ ] Homepage spec reviewed + locked with Lucrece
- [ ] Qualifier quiz redesign drafted
- [ ] Pricing, About, How It Works drafted
- [ ] FAQ standalone page drafted
- [ ] Disqualified routing page drafted

### Phase B — Visual design

- [ ] Lock color palette
- [ ] Lock typography
- [ ] Source / shoot photography (Lucrece + family imagery)
- [ ] Build component library (buttons, cards, comparison tables)

### Phase C — Build (Claude Code session)

- [ ] Lock stack (WordPress vs. Next.js)
- [ ] Build homepage from spec
- [ ] Build qualifier quiz
- [ ] Build pricing, about, how-it-works
- [ ] Deploy schema markup site-wide
- [ ] QA on mobile + desktop

### Phase D — SEO content + county pages

- [ ] Build first 10 county landing pages
- [ ] Launch blog with 8 cornerstone articles (mapped to keyword tiers)
- [ ] Build lead magnet + email sequence

### Phase E — Launch + measure

- [ ] Set up GA4 + Clarity + Search Console
- [ ] Submit sitemap
- [ ] 30-day post-launch review of conversion lift
- [ ] AI search visibility audit (ChatGPT, Perplexity, Google AI Overviews)

### Phase F — AI intake build (separate workstream)

Tracked in `conversational-ai-intake-v1.md`. Likely Q3 2026 depending on Phase A–E progress.

---

## 9. Master Open Decisions

Cross-cutting decisions that apply to multiple pages. Page-specific open questions live in each page's doc.

| # | Decision | Status | Notes |
|---|---|---|---|
| 1 | Tech stack: WordPress vs. Next.js | ✅ Resolved 2026-04-28 | **Path A — WordPress** locked. Homepage built as a self-contained HTML file (`homepage.html`) that drops into a WordPress page or Custom HTML block. Future Phase 3 AI intake may live as a separate Next.js subdomain or embedded widget. |
| 2 | Final color palette | Open | Proposed in Section 4 — confirm in Phase B |
| 3 | Typography choice (Lora / Source Serif / Fraunces) | Open | Decide in Phase B |
| 4 | Photography direction: real families vs. stock | Open | Real preferred — needs photo release process |
| 5 | Lock pricing: $299 / $499 (the live site has 3 different numbers) | Open | Locked in homepage doc; confirm with Lucrece |
| 6 | Lucrece's exact bar admission date + bar number | Open | Need from Lucrece for credibility lines |
| 7 | Final form list (Section 5.10 of homepage doc) | Open | Need Lucrece sign-off before publishing |
| 8 | Disqualified routing language to Bundy Law | Open | UPL-sensitive — needs careful drafting |
| 9 | County rollout order: 10 at once, or 1/week? | Open | 10 at once gives faster topical authority signal |
| 10 | Review widget: keep Trustindex or move to native Google Reviews | Open | Trustindex is fine for now; revisit post-launch |
| 11 | Email platform: ConvertKit vs. MailerLite | Open | Decide before lead magnet build |
| 12 | Professional email address (move off gmail.com) | Open | Recommend `lucrece@adoptionformsexpress.com` or `hello@` |
| 13 | DFY page architecture: split into minor-child and adult URLs | ✅ Resolved 2026-04-28 (URLs refined 2026-04-30 and again 2026-05-01) | Two separate post-quiz funnels — minor-child and adult. The minor-child funnel evolved into a two-page architecture (sales page + checkout page) on 2026-05-01. Current URLs: `/dfy-minor-sales-page/` (minor-child sales page) + `/dfy-child-check-out-page/` (minor-child checkout, sibling top-level page) + `/qualified/done-for-you-adult/` (adult page). Minor-child sales-page URL evolution: original placeholder `/qualified/done-for-you-minor-child/` → `/buy-doneforyou-minor/` (2026-04-30) → `/dfy-minor-sales-page/` (2026-05-01 — chosen for naming symmetry with the new checkout page). |
| 14 | Old `/customized-adoption-forms/` URL — what to do with it | ✅ Resolved 2026-04-28 | Retire the page. 301 redirect to homepage `/` so existing SEO equity flows somewhere useful. |
| 15 | Quiz routing logic — confirm Typeform supports branching to two checkout URLs | Open | Verify before publishing the new pages. Quiz logic must route minor-child qualifying → minor-child URL, adult qualifying → adult URL, disqualified → disqualified routing page. |
| 16 | Adult-adoption SEO pillar — priority? | Open | Adult stepparent adoption is an underserved keyword cluster in Nebraska. Recommend prioritizing the pillar page in Phase D as a high-leverage SEO play. |
| 17 | Forms-product-specific testimonials | Open | Both DFY pages currently use placeholder reviews from broader Bundy Law cases. Need 3 specifically about the Done-For-You minor-child product and 3 specifically about adult adoption product. |
| 18 | Support email — dedicated address for these pages | ✅ Resolved 2026-05-12 | Locked: `info@adoptionformsexpress.com` as the single canonical contact across the entire site. Used in nav, escape hatch, footer, and all legal pages. Chosen over the originally recommended `support@…` because a single inbox is simpler to operate at this stage and `info@` reads as the natural general-contact channel for a small business. Applied to every HTML page (21 string replacements across 9 files) and propagated to every spec-doc current-spec mention. |
| 19 | Review count is hardcoded across pages | ✅ Resolved 2026-04-29 | Decision: visitor-facing review count displays as **"140+"** for durability. Exact `reviewCount` in schema markup remains precise (currently 142) and gets updated quarterly. Revisit live-feed widget integration (option C) post-launch. |
| 20 | Photo-release documentation for testimonials with photos | Open | Kristin's photo is now placed on the homepage. Recommend creating a simple email-based photo-release process: every time a testimonial-with-photo is added, send a one-line confirmation email asking "we'd like to feature your name, testimonial, and photo on the public Adoption Forms Express homepage — is that okay?" and save the email reply. Low-risk for Google-public photos but documents intent for any future dispute. Decide whether to formalize this in a simple template before more photo-paired testimonials are added. |
| 21 | Payment processor: ThriveCart (embedded checkout) | ✅ Resolved 2026-04-30 | ThriveCart embedded checkout is the payment processor for all forms products (DFY minor child, DFY adult, DIY products). Customer stays on the page through the entire transaction. Pages reserve placeholder space for ThriveCart embeds at hero CTA + final CTA. Per-page ThriveCart wiring tracked in each page-level doc. Production snippet for DFY minor-child captured in `dfy-minor-child-page-v1.md` Section 8. |
| 22 | Future task: dedicated refund-policy page | ✅ Resolved 2026-05-12 | Page built at `/refund-policy/` (`refund-policy.html`). Locks the 7-day eligibility window, pre-delivery / post-delivery distinction, request mechanism (reply to order confirmation OR email `info@adoptionformsexpress.com`), 5–10 business day processing, and exceptions clause. Hosting decision: own site at `/refund-policy/` (chosen over ThriveCart-hosted or PDF). **Surface decision (locked 2026-05-05, REVERSED 2026-05-12):** the page was originally NOT linked from the site footer — rationale was that visitors should see the policy at the moment it matters (post-purchase invoice/receipt) rather than buried in marketing-page footers. On 2026-05-12 Tyler reversed this — Refund Policy link was added to the site footer **site-wide** (12 of 13 deployed HTML files; `starter-guide.html` has no footer). The link appears in both the disclaimer paragraph (alongside Terms + Privacy as the third clickable governing-policy reference) and the legal-links bar. Rollout was two passes the same day: initial 3-page pass (homepage, privacy-policy, terms-of-use), then a consistency-gap pass covering `refund-policy.html` itself + the 8 gated product pages (4 sales + 4 checkouts). The Terms of Use page's "Refunds" section still defers to this page; sales-page FAQ Q6 and checkout-page reassurance lines remain the in-funnel surface. |

---

## 10. Master Change Log

End every session with an entry here. This is the cross-document log; individual page docs have their own.

**Older entries archived:** entries from 2026-04-28 through 2026-05-05 (most of the early-May funnel build / polish / mobile-fix-iteration / superseded-token work) live in `website-redesign-master-CHANGELOG.md`. Read that file for the full project history. When this in-line table grows past ~5–7 entries, move the older entries to the archive.

| Date | Doc(s) affected | Change | Author |
|---|---|---|---|
| 2026-05-05 | All four checkout HTML files + their spec docs, **Master** | ThriveCart logo updated, which regenerated the embeddable tokens for all four products. Updated all four checkout HTML files with new tokens (DFY minor 10: TOD8DE → UAXWPD; DFY adult 8: 0FGCA9 → POHMYG; DIY minor 4: TTC0UE → KP063D; DIY adult 7: A4PSQA → F1ED0D). Product IDs unchanged. All four spec docs updated to reflect the new snippets. Each spec doc bumped by 0.1. **Note:** all four tokens above have since been regenerated. See the 2026-05-12 four-product regen entry below for current values (product 10 = `JB96LS`; product 8 = `FGQ5PI`; product 4 = `PC00K4`; product 7 = `8XP52F`). | Claude / Tyler |
| 2026-05-05 | All four checkout HTML files + their spec docs, **Master** | **Mobile empty-space fix v2 (working version) applied uniformly to all four checkout pages.** Tyler's DevTools inspection revealed ThriveCart's embed script injects an `<iframe class="tc-v2-embeddable-el">` (not inline DOM as my read of the prior earlier-shared markup had suggested — that markup was iframe content) inside the `.tc-v2-embeddable-target` div, with an inline `style="height: 2387px"` hardcoded on it. On mobile the form's actual rendered content takes ~1300–1500px, leaving roughly 1000px of dead space that the user scrolls through inside the iframe before reaching our reassurance strip. The iframe also carries `scrolling="yes"`, so capping its height with CSS is safe — any overflow scrolls inside the iframe instead of being clipped. Fix added to all four checkout HTMLs in the same spot (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule): a `@media (max-width: 720px)` block tightening `.thrivecart-wrap` padding to `1.5rem 0` and applying `.thrivecart-wrap iframe.tc-v2-embeddable-el { max-height: 1800px !important; }`. 1800px is intentionally conservative — leaves a buffer for dynamic form expansion (coupon-code section, validation errors, address-state changes) while still cutting most of the dead space. Each spec doc bumped by another 0.1 (DFY minor v2.8 → v2.9, DFY adult v1.13 → v1.14, DIY minor v1.7 → v1.8, DIY adult v1.4 → v1.5). **Tuning playbook for Tyler post-deploy:** if dead space is still visible, lower the cap (1500 → 1300); if a scrollbar appears inside the iframe because the form was clipped, raise it (2000+). Desktop behavior unchanged. CSS-only; no HTML/copy/schema changes. The text-overlap-inside-embed issue (testimonial photo overlapping product description in the form area) remains a separate, unresolved ThriveCart-admin issue — not fixable from our checkout HTML. | Claude / Tyler |
| 2026-05-05 | All HTML files + 5 spec docs + Master | UPL-driven language change. Replaced "attorney call(s)" with "support call(s)" framing across the entire project. DFY products: "two 15-minute support calls". DIY products: "one 30-minute support call". Total support time per product unchanged (30 min). Added protective note on all 4 sales pages: "Support calls are for questions about your forms and the filing process — not personalized legal advice. If you need legal advice about your specific case, please contact a licensed attorney directly." Master doc Section 7 (Tech stack) line about Calendly also updated to drop "free attorney calls" framing. Schema descriptions across all 4 products updated. **Per Flag C resolution:** the DFY checkout schema/meta lines that previously read "Completed by a licensed Nebraska adoption attorney within 3 business days" were also updated to "Completed by our team within 3 business days" — the attorney designed/prepared the form templates (Lucrece's pedigree remains via "Attorney-prepared..." which is left intact), but the per-customer form completion is done by the team, not the attorney directly. Same edit applied to DFY sales pages' final-CTA paragraphs. Reviewed and approved by Lucrece H. Bundy, Esq. as licensed attorney owner. Per master doc Section 3 compliance review trigger, this approval is recorded in writing here. **Spec docs bumped:** homepage-redesign-v1.md v2.10 → v2.11; dfy-minor-child-page-v1.md v2.11 → v2.12; dfy-adult-page-v1.md v1.14 → v1.15; diy-minor-child-page-v1.md v1.8 → v1.9; diy-adult-page-v1.md v1.5 → v1.6. **One small additional voice edit Tyler should know about** — in `diy-adult.html`'s Lucrece signature quote, the original phrase "direct access to me when something specific to their adoption comes up" was implying Lucrece-as-attorney availability for the call, which contradicts the new support-call framing. Replaced with "a place to turn when something specific to their adoption comes up." If Tyler prefers a different wording there, easy follow-up. | Claude / Lucrece |
| 2026-05-05 | All 4 sales-page HTML files + 4 checkout-page HTML files + 4 sales-page spec docs + Master | Sales-page and checkout-page polish + refund policy formalized. (1) Final CTA reassurance line on all 4 sales pages simplified to just "Secure checkout" — refund line and "Questions? Email us" link removed. By the time qualifying visitors reach the sales page, refund/email-question messaging is friction, not reassurance. (2) DFY-only: removed bold from the "Two 15-minute support calls" item in "What's Included" to match list visual rhythm. (3) New wrong-package refund FAQ added to all 4 sales pages explaining the post-purchase confirmation-email step, the 7-day reply deadline, and that no refunds are available after delivery. Same Q&A across all four — refund policy is identical for all products. **Additional adjustment beyond the original brief:** the existing DFY-minor-child Q1 ("What if I realize my case is more complicated than I thought after I order?") previously mixed case-fit refund language with Bundy-Law-routing language; per Lucrece's request the answer was rewritten to drop the refund clauses (the new Q6 holds the canonical refund policy) and to explicitly point complicated cases to Bundy Law LLC for legal advice. The other three sales pages had no Q1 about refunds, so no Q1 rewrite was needed there. (4) New wrong-package refund line added to all 4 checkout pages near the ThriveCart embed; the existing reassurance strip's 7-day-refund clause was removed to avoid contradicting the new policy. New `.refund-note` CSS class added in each checkout `<style>` block (italic, smaller, muted). (5) Master Open Decisions: future task added (#22) for a dedicated refund-policy page. **Surface decision (locked this session):** the page is NOT linked from the site footer. Per Tyler's direction, the link will live in the post-purchase invoice/receipt only — visitors see it at the moment it actually matters rather than buried in the footer of marketing pages. Until the page exists, the FAQ Q6 and the checkout-page note carry the policy. **Locked refund policy:** refunds available between purchase and delivery; delivery happens only after buyer replies to confirmation email; if buyer doesn't reply within 7 days, purchase is considered final; no refunds after forms are sent. Same policy for all 4 products. **Spec docs bumped:** dfy-minor-child-page-v1.md v2.12 → v2.13; dfy-adult-page-v1.md v1.15 → v1.16; diy-minor-child-page-v1.md v1.9 → v1.10; diy-adult-page-v1.md v1.6 → v1.7. Reviewed and approved by Lucrece H. Bundy, Esq. as licensed attorney owner. UPL protective note retained on all 4 sales pages. | Claude / Lucrece |
| 2026-05-11 | dfy-minor-child-checkout.html, dfy-minor-child-page-v1.md, **Master** | Fourth ThriveCart token regen for **product 10 only** (DFY minor child) after Tyler made another adjustment in the ThriveCart admin. Product ID unchanged. Old token: HV1ZXD → new token: W3F688. Updated `dfy-minor-child-checkout.html` (lines 397–398) and `dfy-minor-child-page-v1.md` (token via `replace_all` + change-log entry + version v2.13 → v2.14). Other three checkout files (DFY adult / DIY minor / DIY adult) unaffected — Tyler only edited product 10 in this round. | Claude / Tyler |
| 2026-05-12 | **Master**, `website-redesign-master-CHANGELOG.md` | Archive pass: moved 8 older Section 10 entries to `website-redesign-master-CHANGELOG.md` — the four 2026-05-01 / 2026-05-04 funnel-build & polish entries (DIY minor-child build, DIY adult build, DFY minor-child hero copy clarification, homepage polish), plus four 2026-05-05 entries that are now superseded by later same-day work (mobile fix v1 + its revert, both replaced by mobile fix v2; two intermediate product-10 token regens, both replaced by the 2026-05-11 W3F688 regen). The five remaining inline entries are the load-bearing ones: ThriveCart-logo regen documents the current live tokens for products 4 / 7 / 8; mobile fix v2 is the working mobile fix in place across all four checkouts; UPL-driven language change is the canonical voice/UPL baseline; sales-page + refund-policy polish is the canonical refund-policy baseline; 2026-05-11 fourth token regen documents the current product 10 token. Drops the master doc back under the auto-load size threshold so the "large file impacting performance" warning stops firing each session. Section 11 master row bumped to v1.17. | Claude / Tyler |
| 2026-05-12 | `refund-policy.html` + 8 gated product pages (`dfy-adult.html`, `dfy-minor-child.html`, `diy-adult.html`, `diy-minor-child.html`, `dfy-adult-checkout.html`, `dfy-minor-child-checkout.html`, `diy-adult-checkout.html`, `diy-minor-child-checkout.html`) + **Master** | **Refund Policy footer link extended to the remaining 9 HTML files — closes the consistency gaps flagged in the prior footer-link entry.** Same three-part pattern applied per file as in the earlier same-day 3-page batch: (1) new `.footer-disclaimer a` CSS rule added to each file's `<style>` block (color override needed for muted-dark-background link visibility); (2) the disclaimer paragraph's plain-text "Terms of Use and Privacy Policy" reference rewritten as three clickable links — "Terms of Use, Privacy Policy, and Refund Policy"; (3) `<a>` for Refund Policy appended after the Privacy Policy link in the `.footer-bottom` legal-links bar. **Path style preserved per file:** `refund-policy.html` uses relative paths (matching its existing relative-path bar — its legal-links bar now also has a self-link to `/refund-policy/`, matching the self-link pattern Privacy + Terms have always had); the 8 gated product pages use absolute URLs (matching their existing absolute-URL bars). **Site-wide coverage now complete** — every deployed HTML file in the repo that has a `.footer-disclaimer` block (12 of 13 HTML files; `starter-guide.html` deliberately has no footer) surfaces all three legal pages in both footer locations. Master Decision #22 surface-decision note also updated to reflect site-wide coverage. Master v1.22 → v1.23. | Claude / Tyler |
| 2026-05-12 | `homepage.html`, `privacy-policy.html`, `terms-of-use.html`, **Master** | **Refund Policy link added to the site footer on 3 public-facing pages.** Reverses the surface decision in master Decision #22 (locked 2026-05-05 as NOT-in-footer; reversed 2026-05-12 per Tyler's directive). Link added to two locations in each file's footer: (1) `.footer-disclaimer` paragraph — the existing plain-text "Terms of Use and Privacy Policy" reference was rewritten as three clickable links: "Terms of Use, Privacy Policy, and Refund Policy" (all three linked for consistency rather than leaving the existing two as plain text while introducing one new link); (2) `.footer-bottom` legal-links bar — new `<a href=".../refund-policy/">Refund Policy</a>` appended after the Privacy Policy link. **New CSS rule added to each file's `<style>` block:** `.footer-disclaimer a { color: rgba(255, 255, 255, 0.85); text-decoration: underline; } .footer-disclaimer a:hover { color: white; }` — needed because the disclaimer's muted italic text on dark background would render the new links invisible without an explicit color override. **Path style preserved per file:** homepage.html uses absolute URLs (matching its existing absolute-URL legal-links bar); privacy-policy.html + terms-of-use.html use relative paths (matching their existing relative-path legal-links bar). **Scope (per Tyler's explicit directive):** `starter-guide.html` skipped — it has no site-footer (removed earlier). `refund-policy.html` itself NOT touched — its disclaimer paragraph still references only Terms of Use and Privacy Policy (consistency follow-up flagged to Tyler). The 8 gated product pages (4 sales + 4 checkouts) also NOT touched — their disclaimers still reference only Terms + Privacy (potential follow-up — gated pages may not need the same surface treatment as public pages, since visitors there have already started the funnel). Master Decision #22 surface-decision note updated to record the reversal. Master v1.21 → v1.22. | Claude / Tyler |
| 2026-05-12 | All 4 checkout HTML files (`dfy-minor-child-checkout.html`, `dfy-adult-checkout.html`, `diy-minor-child-checkout.html`, `diy-adult-checkout.html`) + 4 spec docs + **Master** | **Four-product ThriveCart token regen.** Tyler made admin-side adjustments to all four ThriveCart products at once, regenerating all four embeddable tokens. Product IDs unchanged. Updated each checkout HTML file (token in 2 places per file — `data-thrivecart-embeddable` attribute on the div + `id` on the script) and each spec doc via `replace_all`. **Old → new tokens:** product 10 (DFY minor child) `W3F688` → `JB96LS`; product 8 (DFY adult) `POHMYG` → `FGQ5PI` (and then `FGQ5PI` → `OBAALE` later the same day after one additional admin tweak — current product-8 token is **`OBAALE`**); product 4 (DIY minor child) `KP063D` → `PC00K4`; product 7 (DIY adult) `F1ED0D` → `8XP52F`. **Spec doc versions bumped:** dfy-minor-child-page-v1.md v2.15 → v2.16; dfy-adult-page-v1.md v1.16 → v1.18 (two regens); diy-minor-child-page-v1.md v1.11 → v1.12; diy-adult-page-v1.md v1.8 → v1.9. Master Section 11 rows updated to match. Master v1.19 → v1.21 (two bumps). **Reminder for Tyler post-deploy:** retest each of the four mobile checkouts — the 1800px iframe-height cap (mobile fix v2, 2026-05-05) may need tuning if any product's rendered form height changed materially with the admin tweaks. | Claude / Tyler |
| 2026-05-12 | **Master**, `homepage-redesign-v1.md` v2.14, all 9 deployed HTML files (`homepage.html` + 4 sales pages + 4 checkout pages), 3 legal pages (`privacy-policy.html`, `terms-of-use.html`, `refund-policy.html`) | **Business address + business name + legal-page effective-date placement.** **Address:** old `12020 Shamrock Plz, Ste 200, Omaha, NE 68154` → new `P.O. Box 45873, Omaha, Nebraska 68145`. Applied uniformly to (a) the one-line footer Contact bullet in all 9 deployed HTML files + all 3 legal pages (12 total footer updates), (b) the multi-line contact blocks in all 3 legal pages (privacy + terms + refund), (c) the `LegalService` schema `address` block in `homepage.html` (`streetAddress` → `P.O. Box 45873`; `postalCode` → `68145`; `addressRegion` stays `NE` per schema.org convention), (d) homepage spec doc Section 5.15 Column 4 Contact bullet + Section 8 schema example. **Business name:** the parenthetical "(A Bundy Law adoption service)" removed from the contact blocks on all 3 legal pages — canonical business name is just **Adoption Forms Express**. Adoption Forms Express and Bundy Law LLC remain affiliated businesses (founder Lucrece H. Bundy is the link), but the storefront product brand is its own name. **Effective-date placement on legal pages:** the top-of-page `<p class="legal-meta">` date line removed from all three legal-page headers (Privacy "Last updated October 20, 2023", Terms "Last updated October 20, 2023", Refund "Effective May 12, 2026"). Privacy keeps its existing bottom-of-content `Effective as of October 20th, 2023` line; Terms's top-of-content `<em>Effective as of October 20th, 2023</em>` line moved to the very bottom (now matches Privacy's placement, both styled with `.legal-effective` — italic, top-bordered, muted); Refund gets a new bottom-of-content `Effective as of May 12th, 2026` line styled with `.legal-effective` (CSS rule added to `refund-policy.html`'s `<style>` block since it didn't have one yet — copied verbatim from privacy/terms). Net result: all three legal-page headers now show just the coral "LEGAL" kicker + serif title, with the effective date consistently rendered at the very bottom of each page above the footer. Master Section 11 homepage row bumped v2.13 → v2.14; master v1.18 → v1.19. | Claude / Tyler |
| 2026-05-12 | **Master**, all 9 deployed HTML files (`homepage.html` + 4 sales pages + 4 checkout pages), 5 spec docs (`homepage-redesign-v1.md`, `dfy-minor-child-page-v1.md`, `diy-minor-child-page-v1.md`, `diy-adult-page-v1.md`, `lead-magnet-v1.md`), 3 new HTML files (`privacy-policy.html`, `terms-of-use.html`, `refund-policy.html`) | **Contact-email standardization + three legal pages built.** **Email:** `adoptionformsexpress@gmail.com` → `info@adoptionformsexpress.com` standardized site-wide (21 string replacements across 9 HTML files + current-spec mentions in 5 spec docs). `starter-guide.html` had no contact email, no change. `index.html` skipped (legacy file). `support@adoptionformsexpress.com` was never deployed (only ever a spec-doc placeholder). Master Section 7 Tech-Stack line rewritten to reflect the canonical address. **Resolves Open Decisions #18** (support email — dedicated address) **and the DFY minor-child page's Open Q #2** (final support email for the page) — both with `info@…` (chosen over the originally recommended `support@…` because a single inbox is simpler to operate at this stage). **Legal pages:** three new standalone HTML files built. `privacy-policy.html` at `/privacy-policy/` — content preserved verbatim from the live page; the four old email mentions (Children Under 13 contact, two unsubscribe paragraphs, Contact Us block) all swapped to `info@…`. `terms-of-use.html` at `/terms-of-use/` — content preserved verbatim from the live page with ONE structural change: the old "No Refunds" section ("All sales are final, and the Company does not offer any money-back guarantees…") replaced with a new "Refunds" section deferring refund eligibility to the Refund Policy page. `refund-policy.html` at `/refund-policy/` — brand new page in Lucrece's voice locking the 7-day eligibility window, the pre-delivery / post-delivery distinction (delivered = sent for DFY, downloaded for DIY), the request mechanism (reply to order confirmation OR email `info@…` with order number), 5–10 business day processing, and an exceptions clause for technical issues / duplicate charges. All three share homepage's nav + footer markup (with absolute-path anchors `/#how-it-works` etc. so cross-page nav works from a non-homepage URL) and a shared `.legal-*` content style block: centered coral "LEGAL" kicker + Fraunces title header, 720px-max single-column body with line-height 1.7, navy Fraunces h2s, bold Manrope h3s. Inline `<style>` on each page; no external CSS. Footer matches homepage exactly — Terms + Privacy in footer-bottom; Refund Policy is **not** in the footer per Decision #22's surface decision (link lives in post-purchase invoice/receipt only). **Resolves Open Decision #22** (future task: dedicated refund-policy page). **Spec docs bumped:** homepage-redesign-v1.md v2.12 → v2.13; dfy-minor-child-page-v1.md v2.14 → v2.15; diy-minor-child-page-v1.md v1.10 → v1.11; diy-adult-page-v1.md v1.7 → v1.8. Master v1.17 → v1.18. Master Section 2 architecture rows for Privacy + Terms flipped to 🔵 Built; new architecture row added for Refund Policy at 🔵 Built. **Tyler's WordPress deploy steps for the three legal pages:** (1) update/create top-level WP page at `/privacy-policy/` using Blank Slate template + paste `privacy-policy.html` body content; (2) same for `/terms-of-use/`; (3) create new top-level WP page at `/refund-policy/` using Blank Slate template + paste `refund-policy.html` body content; (4) verify all site-wide footer Terms + Privacy links resolve correctly; (5) verify `/refund-policy/` is NOT linked in the site footer. | Claude / Tyler |
| | | | |

---

## 11. Working Document Index

Every doc in the project, with location and current version.

| Doc | Filename | Latest version | Status |
|---|---|---|---|
| **Master** | `website-redesign-master.md` | v1.23 | 🟡 Active |
| Homepage | `homepage-redesign-v1.md` | v2.14 | 🔵 Built (`homepage.html`), ready for WordPress deploy |
| Qualifier quiz | `qualifier-quiz-v1.md` | — | ⚪ Not started |
| Pricing | `pricing-page-v1.md` | — | ⚪ Not started |
| DFY minor child (sales + checkout) | `dfy-minor-child-page-v1.md` | v2.16 | 🔵 Built — `dfy-minor-child.html` (sales page) + `dfy-minor-child-checkout.html` (transactional checkout, ThriveCart product 10) both on disk, ready for WordPress deploy |
| DFY sales — adult | `dfy-adult-page-v1.md` | v1.18 | 🔵 Built — `dfy-adult.html` (sales page) + `dfy-adult-checkout.html` (transactional checkout, ThriveCart product 8) both on disk, ready for WordPress deploy |
| DIY minor child (sales + checkout) | `diy-minor-child-page-v1.md` | v1.12 | 🔵 Built — `diy-minor-child.html` (sales page) + `diy-minor-child-checkout.html` (transactional checkout, ThriveCart product 4) both on disk, ready for WordPress deploy |
| DIY adult (sales + checkout) | `diy-adult-page-v1.md` | v1.9 | 🔵 Built — `diy-adult.html` (sales page) + `diy-adult-checkout.html` (transactional checkout, ThriveCart product 7) both on disk, ready for WordPress deploy |
| DFY public pillar (SEO) | `dfy-pillar-page-v1.md` | — | ⚪ Not started |
| Adult adoption pillar (SEO) | `adult-adoption-pillar-v1.md` | — | ⚪ Not started |
| About / Founder | `about-page-v1.md` | — | ⚪ Not started |
| How It Works | `how-it-works-v1.md` | — | ⚪ Not started |
| FAQ standalone | `faq-page-v1.md` | — | ⚪ Not started |
| County landing pages | `county-landing-pages-v1.md` | — | ⚪ Not started |
| SEO content calendar | `seo-content-calendar-v1.md` | — | ⚪ Not started |
| Lead magnet | `lead-magnet-v1.md` | — | ⚪ Not started |
| Conversational AI intake | `conversational-ai-intake-v1.md` | — | ⚪ Not started |
| Disqualified routing | `disqualified-routing-v1.md` | — | ⚪ Not started |
| Legal pages | `legal-pages-v1.md` | — | 🔵 HTML built — `privacy-policy.html`, `terms-of-use.html`, `refund-policy.html` all on disk and ready for WordPress deploy. Spec doc (`legal-pages-v1.md`) itself not yet written; per-page specs captured in master Section 10 entry 2026-05-12. |
| Schema library (future) | `schema-library-v1.md` | — | ⚪ Not started |

---

## 11.5 Testimonial Registry

A live registry of every testimonial we've evaluated, where it's placed (or reserved), and any notes. Update this any time a testimonial is added, swapped, or reserved for a future page.

**Currently placed (locked):**

| Reviewer | Source | Page | Status |
|---|---|---|---|
| Kristin | Google (Sep 2019) | Homepage — featured pull quote (with photo) | ✅ Live in HTML — paired with circular photo at `/wp-content/uploads/2026/04/Kristin.png`. Photo-release consent recommended before publish. |
| Catherine Day | Google (Sep 2024, Local Guide) | Homepage — three-up card 1 | ✅ Full text in HTML — strongest customer-voice line on the page ("all I had to do essentially, was pay and show up to the court") |
| Amanda Rumelhart | Google (Jul 2023) | Homepage — three-up card 2 | ✅ Full text in HTML — "$10K + 3 lawyers" competitive comparison |
| Ruby Leonard | Google (Local Guide, edited 2024) | Homepage — three-up card 3; **DIY minor-child sales page (`diy-minor-child.html`) — three-up card 1, full text**; **DIY minor-child checkout page (`diy-minor-child-checkout.html`) — compact two-up reassurance card with curated excerpt**; **DIY adult sales page (`diy-adult.html`) — three-up card 3, full text**; **DIY adult checkout page (`diy-adult-checkout.html`) — compact two-up reassurance card with curated excerpt** | ✅ Full text in HTML on homepage, DIY minor-child sales page, and DIY adult sales page (only forms-product-specific Google review in the entire 142-review set — placed in slot 1 on the DIY minor-child sales page and slot 3 on the DIY adult sales page where Catrice carries adult-adoption authority in slot 1); both DIY checkout pages use the same curated excerpt: *"We ended up purchasing the DIY Adoption documents for step-parent adoption and it was so easy to do and understand."* |
| Jennifer Jenkins | Google (Apr 2025) | DFY minor-child — card 1 | ✅ Full text in doc spec — curated excerpt locked for HTML three-up card (visual balance with Sarah's and Robyn's) |
| Sarah Hall | Google (Sep 2022) | DFY minor-child sales — card 2; **DFY minor-child checkout (`dfy-minor-child-checkout.html`) — compact two-up reassurance card**; **also on DIY minor-child sales page (`diy-minor-child.html`) — three-up card 2** | ✅ Full text in doc spec; same compact reassurance text used on the DFY checkout page; full text used on the DIY sales page (her "quick and effortless / handled everything" line works equally well as DFY-friendly social proof and as DIY-friendly reassurance that Lucrece's clients have a smooth experience) |
| Robyn Wallace | Google (Oct 2020) | DFY minor-child — card 3 | ✅ Full text in doc spec — uniquely validates procedural rails ("detailed instructions on how to fill out the forms and updates and reminders") |
| Catrice Jackson | Google (Aug 2022) | DFY adult sales — card 1, full text; **DFY adult checkout page (`dfy-adult-checkout.html`) — compact two-up reassurance card, curated excerpt**; **DIY adult sales page (`diy-adult.html`) — three-up card 1, curated ~66-word excerpt** | ✅ Only Google review explicitly mentioning adult adoption — anchors slot 1 on both adult sales pages, carrying adult-adoption authority. DIY adult sales page uses a curated ~66-word excerpt for visual balance with the shorter Patty/Ruby cards in slots 2/3: *"She went above and beyond to help my family. She was extremely informative, knowledgeable about adult adoption, kind, very patient, and very professional. She really made me feel like I had nothing to worry about. With her amazing service, my husband was able to legally adopt my 30 year old son. There are no words to describe what this means to me as a mother."* DFY adult checkout uses a shorter curated excerpt: *"Lucrece... went above and beyond to help my family. She was extremely informative, knowledgeable about adult adoption, kind, very patient... and very professional. With her amazing service, my husband was able to legally adopt my 30 year old son."* |
| Gary Boettcher | Google (May 2019) | DFY adult — card 2 | ✅ Full text in doc spec |
| Patty Bales | Google (Sep 2020) | DFY adult sales — card 3; **DIY adult sales page (`diy-adult.html`) — three-up card 2, full text**; **DFY minor-child checkout (`dfy-minor-child-checkout.html`)**; **DFY adult checkout (`dfy-adult-checkout.html`)**; **DIY minor-child checkout (`diy-minor-child-checkout.html`)**; **DIY adult checkout (`diy-adult-checkout.html`)** — compact two-up reassurance card on all four checkout pages | ✅ Full text in doc spec and in HTML on DIY adult sales page (slot 2 — cost-anxiety reducer between Catrice's adult-adoption authority and Ruby's DIY product validation); strong "no hidden fees" line; all four checkout pages use the same curated excerpt: *"Of course price seems to always play a role and she is very reasonable with no hidden fees!"* The cost-anxiety counter is universal — works for $499 DFY and $299 DIY, minor-child and adult, equally well. |
| Kevin Shafer | Google (Jan 2022) | DIY minor-child sales page (`diy-minor-child.html`) — three-up card 3 | ✅ Full text in HTML — "would absolutely use again" line works as the closing slot 3 (post-purchase satisfaction angle, complementing Ruby's product-specific authority and Sarah's process-smoothness). Moved from reserve to placed 2026-05-01. |

**Reserved for future pages (do not use elsewhere without trade analysis):**

| Reviewer | Source | Reserved for | Reason |
|---|---|---|---|
| _(none currently — all previously reserved testimonials are now placed)_ | | | |

**Known forms-product customers — candidates for future testimonial requests:**

These are clients Lucrece has confirmed purchased the forms product, but whose existing Google reviews don't specifically mention the product or aren't yet collected. They're prime candidates to ask for a *new* written testimonial when we build the DIY checkout page or expand the homepage's product-specific social proof.

| Reviewer | Existing Google review? | Notes |
|---|---|---|
| Hein | Unknown | Mentioned by Lucrece as adult-adoption client; review status TBD |
| Strebin | Unknown | Mentioned by Lucrece as adult-adoption client; review status TBD |
| McVay | Unknown | Mentioned by Lucrece as adult-adoption client; review status TBD |

**Do not use:**

| Reviewer | Reason |
|---|---|
| Megan Findeis | Decision logged 2026-04-29: do not use this testimonial. |

**Strong candidates surfaced from review review (potential future use):**

| Reviewer | Source | Best fit |
|---|---|---|
| LaCyndria McClarty | Google (Dec 2020) | Future "switched from another attorney" angle — *"After getting the runaround for several years from other attorneys…"* |
| Adam Buda | Google (Dec 2022) | Same angle — *"Lucrece was the adoption lawyer that we had been looking for for years. Finally finding her was the Godsend we needed…"* |
| Angie Busch | Google (Oct 2022) | Same angle — *"We had been with another lawyer before for two years…"* |

These are strong candidates for a future "we tried other attorneys first" social proof block on a comparison or pillar page.

---

## 12. Session Workflow Cheat Sheet

For starting any new session in Claude Code, Cowork, or chat:

**Starting a session**
1. Upload this master document.
2. Upload the page-level doc(s) you're working on this session.
3. Tell the assistant: "Read the master doc, then [specific task]."
4. Glance at Master Open Decisions and Master Change Log to see what's still unresolved or what changed since last time.

**During the session**
- If a decision affects only one page, update that page's doc.
- If a decision affects the whole site (voice, design, SEO, stack), update **this master**.
- If you create a new companion doc, register it in Section 11.

**Ending a session**
1. Update the relevant page-level doc's change log.
2. Update **Section 10 (Master Change Log)** here.
3. Update **Section 9 (Master Open Decisions)** if anything got resolved or any new decision opened.
4. Update **Section 2 (Site Architecture & Page Status)** if any page changed status.
5. Bump the version number on this master if shared standards changed.

---

*End of v1.0 — Master Working Document*
