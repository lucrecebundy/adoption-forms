# Adoption Forms Express — Website Redesign Master Document

**Document type:** Master / index for the entire site redesign
**Owner:** Lucrece H. Bundy / Tyler
**Site:** adoptionformsexpress.com
**Version:** 1.6
**Last updated:** May 1, 2026
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
| DFY pillar (public SEO) | `/done-for-you-adoption-forms-nebraska/` | Indexed pillar page funneling to quiz | `dfy-pillar-page-v1.md` | ⚪ Not started |
| Adult adoption pillar (public SEO) | `/adult-stepparent-adoption-nebraska/` | Indexed pillar page targeting underserved adult-adoption keywords | `adult-adoption-pillar-v1.md` | ⚪ Not started |
| About / Founder | `/about` | Lucrece bio, firm story, credentials | `about-page-v1.md` | ⚪ Not started |
| How It Works | `/how-it-works` | Long-form process walkthrough | `how-it-works-v1.md` | ⚪ Not started |
| FAQ (full) | `/faq` | Expanded FAQ standalone page | `faq-page-v1.md` | ⚪ Not started |
| County landing pages | `/counties/[county-slug]` | Local SEO — 1 page per priority county | `county-landing-pages-v1.md` | ⚪ Not started |
| Blog | `/blog` | SEO content engine | `seo-content-calendar-v1.md` | ⚪ Not started |
| Conversational AI intake | TBD | Phase 3 AI flow replacing/augmenting qualifier | `conversational-ai-intake-v1.md` | ⚪ Not started |
| Lead magnet landing | `/starter-guide` | Email capture + free PDF ("Free Nebraska Adoption Guide") | `lead-magnet-v1.md` | ⚪ Not started — but already referenced as the secondary CTA on homepage (hero + final CTA + FAQ footnote) and in the homepage + DFY footer. Currently stubbed to `#` in HTML. |
| Terms of Use | `/terms-of-use` | Legal — keep current, audit copy | `legal-pages-v1.md` | ⚪ Not started |
| Privacy Policy | `/privacy-policy` | Legal — keep current, audit copy | `legal-pages-v1.md` | ⚪ Not started |
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
- Email — currently `adoptionformsexpress@gmail.com` (consider professional inbox post-launch)

**Planned additions:**
- Email automation (ConvertKit or MailerLite) for lead magnet + post-purchase sequence
- Conversational AI intake (Phase 3)
- Calendly or similar for the free 15-minute attorney calls
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
| 18 | Support email — dedicated address for these pages | Open | Both DFY page docs reference a `[support email]` placeholder. Recommend creating `support@adoptionformsexpress.com` before publishing. |
| 19 | Review count is hardcoded across pages | ✅ Resolved 2026-04-29 | Decision: visitor-facing review count displays as **"140+"** for durability. Exact `reviewCount` in schema markup remains precise (currently 142) and gets updated quarterly. Revisit live-feed widget integration (option C) post-launch. |
| 20 | Photo-release documentation for testimonials with photos | Open | Kristin's photo is now placed on the homepage. Recommend creating a simple email-based photo-release process: every time a testimonial-with-photo is added, send a one-line confirmation email asking "we'd like to feature your name, testimonial, and photo on the public Adoption Forms Express homepage — is that okay?" and save the email reply. Low-risk for Google-public photos but documents intent for any future dispute. Decide whether to formalize this in a simple template before more photo-paired testimonials are added. |
| 21 | Payment processor: ThriveCart (embedded checkout) | ✅ Resolved 2026-04-30 | ThriveCart embedded checkout is the payment processor for all forms products (DFY minor child, DFY adult, DIY products). Customer stays on the page through the entire transaction. Pages reserve placeholder space for ThriveCart embeds at hero CTA + final CTA. Per-page ThriveCart wiring tracked in each page-level doc. Production snippet for DFY minor-child captured in `dfy-minor-child-page-v1.md` Section 8. |

---

## 10. Master Change Log

End every session with an entry here. This is the cross-document log; individual page docs have their own.

| Date | Doc(s) affected | Change | Author |
|---|---|---|---|
| 2026-04-28 | Homepage | v1.0 — Initial homepage redesign spec drafted | Claude / Tyler |
| 2026-04-28 | Homepage | v1.1 — Added Executive Summary section near top | Claude / Tyler |
| 2026-04-28 | **Master** | v1.0 — Master working document created; site architecture, shared standards, master roadmap, master open decisions, change log all established | Claude / Tyler |
| 2026-04-28 | **Master** | v1.1 — Stack decision locked (Path A, WordPress). Homepage status updated to Built. | Claude / Tyler |
| 2026-04-28 | Homepage | v2.0 — Built `homepage.html` — single self-contained HTML file with inline CSS, JSON-LD schema (LegalService, AggregateRating, FAQPage), FAQ accordion, all 15 sections from spec, both professional photos placed (hero + founder spotlight). WordPress-ready. | Claude / Tyler |
| 2026-04-28 | DFY pages, **Master** | Split old `/customized-adoption-forms/` page into two post-qualification checkout pages: `dfy-minor-child-page-v1.md` v1.0 and `dfy-adult-page-v1.md` v1.0. Both gated (noindex), entered only via qualifier quiz routing. Old URL to be 301 redirected to homepage. Master doc updated: site architecture, working doc index, two new resolved decisions (#13, #14) plus four new open decisions (#15–#18). Two future SEO pillar pages registered as not-started. | Claude / Tyler |
| 2026-04-29 | DFY minor-child | v1.1 — Removed "Waiver of Notice" from forms list. Removed email support from package (only 2 attorney calls included, scoped to questions about the forms). Timeline updated 2–4 months → 4–6 months. FAQ updated to match. **Note: same edits may need to apply to homepage doc/HTML and dfy-adult-page-v1 — flagged to user for decision.** | Claude / Tyler |
| 2026-04-29 | Homepage doc, Homepage HTML, DFY adult | Cross-doc consistency edits propagated. Homepage doc → v2.1 (timeline updated, Waiver of Notice removed, call line scoped to forms). Homepage HTML updated to match (FAQ schema, FAQ accordion, How It Works, Section 5.10 forms list, both pricing cards). DFY adult → v1.1 (email access removed, calls scoped to forms). | Claude / Tyler |
| 2026-04-29 | Homepage doc, Homepage HTML, **Master** | Review count updated 118 → 142 across the homepage doc (v2.2) and homepage HTML (4 places: schema `reviewCount`, hero credibility, image badge, trust strip). Master doc: new open decision #19 added flagging the hardcoding issue and recommending a more durable solution (live-feed widget, or "150+" rounded). |  Claude / Tyler |
| 2026-04-29 | Homepage doc, Homepage HTML, **Master** | Open decision #19 resolved: visitor-facing review count rounded to "140+" across all visible spots in HTML and doc. Schema markup retains exact count for Google compliance. Homepage doc → v2.3. | Claude / Tyler |
| 2026-04-29 | DFY adult | v1.2 — Three testimonials locked for Section 4.5: Catrice Jackson, Gary Boettcher, Patty Bales (all adult-adoption clients, all Google-verified). Catrice's review is full text; Boettcher and Bales are truncated and need full text pulled from Google before HTML build. Page-level Open Question #1 resolved. | Claude / Tyler |
| 2026-04-29 | DFY minor-child, Homepage doc, Homepage HTML | DFY minor-child v1.2: testimonials locked (Jennifer Jenkins, Sarah Hall, Kevin Shafer); Open Question #1 resolved. Homepage doc v2.4: Section 5.11 three-up swapped to Catherine Day, Kevin Shafer, Sarah Hall. Homepage HTML updated to match. Each page now uses Google-verified testimonials curated for its specific audience. | Claude / Tyler |
| 2026-04-29 | DFY adult | v1.3 — Gary Boettcher full review text added (was previously truncated). Bales remains the only truncated testimonial across all four pages with locked testimonials. | Claude / Tyler |
| 2026-04-29 | DFY adult | v1.4 — Patty Bales full review text added. DFY adult page is now fully testimonial-locked with all three Google-verified texts. Status moved from 🟡 Draft to 🟢 Ready for HTML build. | Claude / Tyler |
| 2026-04-29 | Homepage doc, Homepage HTML, **Master** | Homepage doc → v2.5: Sarah Hall swapped out for Ruby Leonard in three-up testimonials. Reason: Ruby's review is the only forms-product-specific Google review in the entire 142-review set. Sarah Hall reserved for future DIY checkout page. Master doc: new Section 11.5 Testimonial Registry created — permanent home for placement, reserves, candidates, and known forms-product customers (Megan Findeis logged). | Claude / Tyler |
| 2026-04-29 | Homepage doc, Homepage HTML, DFY minor-child, **Master** | Three swaps in one batch. (1) Catherine Day full text added to homepage three-up — used a curated excerpt including her strongest customer-voice line ("all I had to do essentially, was pay and show up to the court"). Homepage doc → v2.6. (2) Kevin Shafer swapped out of DFY minor-child card 3 in favor of Robyn Wallace, whose review uniquely validates procedural rails ("detailed instructions on how to fill out the forms and updates and reminders"). DFY minor-child doc → v1.3. Kevin moved to testimonial reserve. (3) Master testimonial registry updated to reflect new placements. Megan Findeis moved to "Do not use" per Tyler. Both homepage and DFY minor-child page now status 🟢 (testimonials locked, ready for HTML build / deploy). | Claude / Tyler |
| 2026-04-29 | Homepage doc, Homepage HTML, **Master** | Featured testimonial restructured. Kristin's testimonial now serves as the featured pull quote with a circular photo (Kristin.png in WordPress media). Amanda's "$10K + 3 lawyers" testimonial moved into three-up card 2 (replacing Kevin Shafer). Kevin moves to testimonial reserve. New CSS class `.review-featured-photo` added. Master doc: testimonial registry reflects new placements; new open decision #20 added re: photo-release documentation as project-wide practice. Homepage doc → v2.7. | Claude / Tyler |
| 2026-04-29 | DFY minor-child doc + new HTML, DFY adult doc, Homepage doc, Homepage HTML, **Master** | Big cross-doc consistency session + new HTML build. (1) **`dfy-minor-child.html` built** — single self-contained HTML file inheriting all `homepage.html` design tokens (Fraunces + Manrope, color palette, FAQ accordion mechanic). Sections: stripped checkout-style nav, qualification-confirmation hero with success-green eyebrow + recap callout, "What's Included" two-column, "What Happens Next" 4-step timeline, Lucrece signature block (small circular photo) + 3 forms-product testimonials, 5-question pre-purchase FAQ (no FAQPage schema by design), navy final-CTA, escape hatch. `noindex,nofollow` + `Product` schema only. Buy buttons placeholder-linked (`#`) with TODO comments for Stripe URL. (2) **Form-name correction** — "Notice of Hearing" → "Notice of Adoption" propagated across `homepage.html`, `homepage-redesign-v1.md`, `dfy-minor-child-page-v1.md`, `dfy-adult-page-v1.md`, `dfy-minor-child.html` (5 files). `index.html` deliberately left untouched — confirmed legacy file. (3) **Background check authorization moved** from Forms column to Guidance column on both DFY page docs and the minor-child HTML, with new framing — "you complete the checks yourself; we provide step-by-step guidance for what your county requires." (4) **Consent forms simplified** across all package descriptions to just "Consent forms" (no specification) so the package list is unified across all pages. (5) **Adult page Forms column** rewritten to mirror minor-child page word-for-word (Tyler corrected an earlier inaccurate claim — adult adoption requires consent from BOTH biological parents AND the adult adoptee themselves; doesn't require *fewer* forms). (6) **"What Happens Next" section** edits across both DFY docs + minor-child HTML: H2 "From order to filed forms in 3 business days" → "From order to inbox in 3 business days" (3-day window is delivery, not filing); step 2 "trained paralegal" → "Our team"; step 3 PDF mention removed (delivery via Google Drive link in practice, but not surfaced in copy). Versions bumped: `homepage-redesign-v1.md` → v2.8, `dfy-minor-child-page-v1.md` → v2.1 (with HTML build at v2.0), `dfy-adult-page-v1.md` → v1.5. Site architecture row for DFY minor-child updated to 🔵 Built. | Claude / Tyler |
| 2026-04-29 | Homepage doc, Homepage HTML, DFY minor-child doc + HTML, **Master** | Form Sneak Peek retired across the entire project; lead-magnet freebie ("Free Nebraska Adoption Guide") takes its place. **Homepage:** hero secondary CTA, final CTA secondary button, and footer Services link all swapped from sneak-peek to the freebie (homepage doc + homepage.html). **New addition** — homepage FAQ section now ends with a soft sub-CTA footnote: "Still have questions? Get the free Nebraska Adoption Guide…" (new `.faq-footnote` CSS class). This is the lead magnet's dedicated conversion point on the homepage, catching FAQ readers who aren't ready for the quiz. **DFY minor-child:** footer Services link swapped (HTML only — body of DFY page deliberately stays purchase-focused, no freebie in the hero / final CTA / escape hatch). **Master architecture:** Sneak Peek row removed from Section 2 + Section 11 (working doc index). Lead magnet landing row updated with note that it's now referenced from homepage and DFY footer. **All freebie links currently stubbed to `#`** with TODO comments — wire to `/starter-guide` once the lead-magnet landing page is built. Resolves homepage doc Open Question #7 (lead magnet on homepage). Versions bumped: `homepage-redesign-v1.md` → v2.9, `dfy-minor-child-page-v1.md` → v2.2, master → v1.3. | Claude / Tyler |
| 2026-04-30 | DFY minor-child, **Master** | DFY minor-child v2.2 → v2.3 (master → v1.4). Three layered changes ported in a single update. **(1) URL alignment:** confirmed the live URL is `/buy-doneforyou-minor/` (not the placeholder `/qualified/done-for-you-minor-child/`); updated spec doc header / Section 6 canonical / Section 8 deployment URL, master Section 2 site architecture, master Decision #13 notes. The page already exists on the live WordPress site at this URL; the new HTML build replaces its content. **(2) ThriveCart Integration:** ThriveCart embedded checkout speccd as the payment processor for all forms products. Both CTA locations on the DFY minor-child page (Section 4.2 hero + Section 4.7 final) updated to use the embed instead of a standard button. New "ThriveCart Integration" subsection added to spec doc Section 8 with the production embed snippet captured verbatim (account `adoptionssimplified`, product `10`, embed token `tc-adoptionssimplified-10-TOD8DE`); duplicate-`id` test consideration documented; what ThriveCart handles automatically vs. what still needs separate setup also captured. Three new page-level open questions added: #8 (✅ resolved with snippet), #9 (success URL → intake form wiring, open), #10 (button styling decision, open). **Master Decision #21 added:** ThriveCart confirmed as canonical payment processor site-wide. **(3) Jennifer Jenkins testimonial:** Section 4.5 truncated review replaced with full text captured verbatim; curated excerpt locked for the HTML three-up card (visual balance with Sarah's and Robyn's — drops front/back framing, preserves "I could breathe for the first time in nearly a decade" and "she truly cares about the adoption process"). Master Section 11.5 testimonial registry updated. | Claude / Tyler |
| 2026-05-01 | dfy-minor-child-checkout.html, dfy-minor-child-page-v1.md, **Master** | DFY minor-child architecture split into a two-page funnel: sales page (`dfy-minor-child.html`) does the convincing; checkout page (`dfy-minor-child-checkout.html`) only takes payment. The checkout page was originally built as a sales-page clone in a prior session — refactored this session from 1027 → 455 lines (~44%). New checkout structure: minimal nav, success-green confirmation header (✓ Secure checkout + product-name H1 + $499 subhead), smaller h2 "Complete your payment below," single full-width ThriveCart embed, lock-emoji reassurance strip, two compact testimonials (Sarah Hall, Patty Bales), standard footer. Master testimonial registry updated to reflect Sarah Hall and Patty Bales now also placed on the checkout page. dfy-minor-child-page-v1.md bumped → v2.4 (header status updated; spec body still describes original single-page architecture, deferred for future rewrite). **Open issue (URL conflict):** the checkout page's canonical currently points to `/buy-doneforyou-minor/`, which is also the sales page's URL — needs resolution before WordPress deploy. | Claude / Tyler |
| 2026-05-01 | dfy-minor-child.html, dfy-minor-child-checkout.html, dfy-minor-child-page-v1.md, **Master** | URL conflict resolved. Two distinct URLs assigned to the two-page funnel: sales page stays at the existing `/buy-doneforyou-minor/` (no upstream change needed — quiz Typeform redirect keeps working), checkout page moves to new sub-path `/buy-doneforyou-minor/checkout/`. Changes applied: (1) `dfy-minor-child-checkout.html` canonical updated; (2) `dfy-minor-child.html` two CTA buttons (hero + final CTA) updated from placeholder `href="#"` to `href="/buy-doneforyou-minor/checkout/"`; stale TODO comments removed; (3) `dfy-minor-child-page-v1.md` header URL line and Section 8 deployment URL updated to reflect both URLs; (4) **Master Section 2:** the single "DFY checkout — minor child" row split into two rows: "DFY sales page — minor child" (`/buy-doneforyou-minor/`) and "DFY checkout — minor child" (`/buy-doneforyou-minor/checkout/`). **Tyler's WordPress deploy step:** create the new checkout WP page as a child of the existing Buy DFY Minor page with slug `checkout`, paste the `dfy-minor-child-checkout.html` body content, mark noindex via SEO plugin. ThriveCart now only loads on the checkout page — no duplicate-instance concern. | Claude / Tyler |
| 2026-05-01 | dfy-minor-child.html, dfy-minor-child-checkout.html, dfy-minor-child-page-v1.md, **Master** | Checkout URL revised after WordPress deploy. Tyler created the checkout WP page as a **top-level page** at `/dfy-child-check-out-page/` rather than as a child of `/buy-doneforyou-minor/`. The two pages are now sibling top-level WordPress pages, not parent/child. URLs aligned across all four files: `dfy-minor-child-checkout.html` canonical → `/dfy-child-check-out-page/`; `dfy-minor-child.html` two CTA buttons → `https://adoptionformsexpress.com/dfy-child-check-out-page/`; `dfy-minor-child-page-v1.md` header URL line + Section 8 deployment URL updated; master Section 2 architecture row for the checkout page updated. Also: minor typography fix on `dfy-minor-child.html` — `&nbsp;` added between "business" and "days" in the "What Happens Next" H2 and step 2 H3 so "days" doesn't orphan to its own line on narrow widths. | Claude / Tyler |
| 2026-05-01 | dfy-minor-child.html, dfy-minor-child-page-v1.md, **Master** | Sales page URL revised. Tyler renamed the sales-page WordPress slug from `/buy-doneforyou-minor/` to `/dfy-minor-sales-page/` for naming symmetry with the checkout page (`/dfy-child-check-out-page/`). URLs aligned: `dfy-minor-child.html` canonical updated to `https://adoptionformsexpress.com/dfy-minor-sales-page/` (also caught a stale canonical that had been pointing to the original `/qualified/done-for-you-minor-child/` placeholder URL all along — it missed the 2026-04-30 alignment round; now corrected); `dfy-minor-child-page-v1.md` header URL line, Section 6 canonical example, Section 8 deployment URL updated; master Section 2 architecture row updated; master Decision #13 updated to reflect the URL evolution and add a third revision date. **Tyler's WordPress-side action items (not in this code update):** (1) update the qualifier-quiz Typeform redirect from `/buy-doneforyou-minor/` to `/dfy-minor-sales-page/`; (2) set a 301 redirect in WordPress from `/buy-doneforyou-minor/` to `/dfy-minor-sales-page/` so any inbound links to the old URL don't 404. | Claude / Tyler |
| 2026-05-01 | dfy-adult-page-v1.md, **Master** | dfy-adult-page-v1.md → v1.9. Section 1 strategic visitor-archetype bullet ("Surprised that the process is more straightforward than minor-child adoption (no consent of biological parents required, no home study, often a single court hearing)") rewritten to align with the v1.7 (consent) and v1.8 (timeline + hearing) corrections. New text: "Surprised by how procedurally light adult adoption is on the front end — no home study, less documentation than minor-child cases — even though the courthouse timeline is similar (4–6 months)." Internal/strategic copy only — no HTML change required. | Claude / Tyler |
| 2026-05-01 | dfy-adult-page-v1.md, dfy-adult.html, **Master** | dfy-adult-page-v1.md → v1.8. Adult-adoption timeline corrected per Tyler: "6–10 weeks" replaced with **4–6 months** in Section 4.4 step 4, Section 4.4 notes, and Section 4.6 FAQ Q3 answer. Two related factual claims Tyler flagged as inaccurate were also removed: "no biological-parent notification waiting period" and "the hearing is typically shorter / simpler hearing" — both deleted from FAQ Q3 and the Section 4.4 notes. The "faster than minor-child" framing dropped entirely (adult and minor-child now share the 4–6 month timeline). Section 4.4 notes reframe the adult-adoption advantage as procedural (less documentation up front, no home study) rather than calendar speed. Section 9 Open Question #2 (timeline) ✅ resolved at 4–6 months. Edits propagated to `dfy-adult.html` (FAQ Q3 + step 4). | Claude / Tyler |
| 2026-05-01 | dfy-adult-page-v1.md, dfy-adult.html, **Master** | dfy-adult-page-v1.md → v1.7. Section 4.6 FAQ Q1 ("Do biological parents need to consent to an adult adoption in Nebraska?") answer corrected per Tyler — flipped from "No" to "Yes", with the professional rewrite specifying that written consent is required from the spouse (the adult adoptee's biological parent) and from the adult adoptee themselves, both filed with the petition. Edit propagated to `dfy-adult.html`. Notes bullet on why Q1 goes first also updated to match the new framing. **Section 4.3 internal note also narrowed in this edit (Tyler chose option a):** the v1.5 "both biological parents plus the adult adoptee" framing replaced with "your spouse (the adoptee's biological parent) and the adult adoptee themselves." The absent biological parent's consent is NOT required for a Nebraska adult-stepparent case. The customer-facing "Consent forms" line is generic enough to keep working for both adult and minor-child without surfacing the underlying consent-party difference. | Claude / Tyler |
| 2026-05-01 | dfy-adult-page-v1.md, dfy-adult.html, **Master** | **Architecture lock — all four products get the two-page treatment.** The two-page funnel pattern proven on the minor-child product (sales page does the convincing → separate checkout page does the transaction with embedded ThriveCart) is now the standard for all four forms products: DFY minor, DFY adult, DIY minor, DIY adult. URL convention locked: `/dfy-{audience}-sales-page/` and `/dfy-{audience}-checkout-page/` (DIY pages will follow the same pattern). **Adult sales page repositioned (v1.5 → v1.6):** dfy-adult-page-v1.md retitled from "Post-Qualification Checkout Page" to "Post-Qualification Sales Page". URL locked to `/dfy-adult-sales-page/` (replacing placeholder `/qualified/done-for-you-adult/`). Both hero and final CTAs updated to "Continue to Checkout — $499" and link to `/dfy-adult-checkout-page/` (the future adult checkout page, not yet built). "How to Use", "What this page IS / IS NOT", canonical, deployment URL, Section 8 all updated. ThriveCart embed will live on the future checkout page, not on the sales page. **Adult sales page HTML built (`dfy-adult.html`):** 1044 lines, near-identical sibling of `dfy-minor-child.html` (same CSS, fonts, design tokens, FAQ accordion mechanic, footer). Adult-specific content swapped in: H1, subhead, 4-item qualification recap (vs 6 for minor-child), Forms/Guidance package list with adult-tweaks (calls description references "adult-adoption experience"; birth-cert line references stepchild's name change), 4-step "What Happens Next" with adult-specific times (10-min intake, 6–10 week finalize) + closing line acknowledging real-world deadlines, signature block with "including adult stepparent adoptions" cred line, three full Google-verified adult-adoption testimonials (Catrice Jackson, Gary Boettcher, Patty Bales), 5-question pre-purchase FAQ (adult-specific Qs/As — biological-parent consent, name change, timeline, out-of-state, what's not included), final CTA H2 "Ready to make it official?", escape hatch with adult-specific estate/inheritance language. `noindex,nofollow` + Product schema only. **Master Section 2 update:** single "DFY checkout — adult" row split into two rows: "DFY sales — adult" (🔵 Built) + "DFY checkout — adult" (⚪ Not started). **Master Section 11 update:** dfy-adult-page-v1.md → v1.6 / 🔵 Built. | Claude / Tyler |
| 2026-05-01 | dfy-adult-checkout.html (new), dfy-adult-page-v1.md, **Master** | **Adult two-page funnel completed.** New file `dfy-adult-checkout.html` built as a structural sibling of `dfy-minor-child-checkout.html` — same `<style>` block verbatim, same minimalist nav (logo + "Email us"), same body section order (confirmation header → ThriveCart embed → reassurance strip → two-up testimonials → footer), same `noindex,nofollow`, same Schema.org Product block adapted to the adult product. Adult-specific changes: title, meta description, canonical (`/dfy-adult-checkout-page/`), schema name + description (Adult Stepparent Adoption Forms, $499), confirmation H1 ("Done-For-You Nebraska Adult Stepparent Adoption Forms"), ThriveCart embed swapped to product `8` (token `tc-adoptionssimplified-8-0FGCA9`), two-up testimonials swapped to **Catrice Jackson** (curated excerpt — only Google review explicitly mentioning adult adoption: *"...went above and beyond...knowledgeable about adult adoption...my husband was able to legally adopt my 30 year old son"*) and **Patty Bales** (same "no hidden fees" line as on the minor-child checkout — strong cost-anxiety counter for both audiences). Sales page (`dfy-adult.html`) required no changes — its two CTA buttons already pointed at `/dfy-adult-checkout-page/`. **Doc updates:** `dfy-adult-page-v1.md` → v1.10 (status updated, Section 8 deployment notes now list both files + the ThriveCart product 8 embed details, change log entry added). Master Section 2 architecture row for the adult checkout page flipped from ⚪ Not started → 🔵 Built; Master Section 11 working-doc index updated to v1.10. **Master testimonial registry update needed (Section 11.5):** Catrice Jackson now also placed on the adult checkout page (in addition to her DFY adult sales-page card 1); Patty Bales now placed on the adult checkout page in addition to the minor-child checkout AND her DFY adult sales-page card 3. **Tyler's WordPress-side action item:** create the new checkout WP page as a top-level page with slug `dfy-adult-checkout-page`, paste the `dfy-adult-checkout.html` body content, mark noindex via SEO plugin. ThriveCart now only loads on the checkout page — no duplicate-instance concern. | Claude / Tyler |
| | | | |

---

## 11. Working Document Index

Every doc in the project, with location and current version.

| Doc | Filename | Latest version | Status |
|---|---|---|---|
| **Master** | `website-redesign-master.md` | v1.6 | 🟡 Active |
| Homepage | `homepage-redesign-v1.md` | v2.9 | 🔵 Built (`homepage.html`), ready for WordPress deploy |
| Qualifier quiz | `qualifier-quiz-v1.md` | — | ⚪ Not started |
| Pricing | `pricing-page-v1.md` | — | ⚪ Not started |
| DFY checkout — minor child | `dfy-minor-child-page-v1.md` | v2.4 | 🔵 Built — `dfy-minor-child.html` (sales page) + `dfy-minor-child-checkout.html` (transactional checkout) both on disk, ready for WordPress deploy |
| DFY sales — adult | `dfy-adult-page-v1.md` | v1.10 | 🔵 Built — `dfy-adult.html` (sales page) + `dfy-adult-checkout.html` (transactional checkout, ThriveCart product 8) both on disk, ready for WordPress deploy |
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
| Legal pages audit | `legal-pages-v1.md` | — | ⚪ Not started |
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
| Ruby Leonard | Google (Local Guide, edited 2024) | Homepage — three-up card 3 | ✅ Full text in HTML — only forms-product-specific Google review in the entire 142-review set |
| Jennifer Jenkins | Google (Apr 2025) | DFY minor-child — card 1 | ✅ Full text in doc spec — curated excerpt locked for HTML three-up card (visual balance with Sarah's and Robyn's) |
| Sarah Hall | Google (Sep 2022) | DFY minor-child — card 2; **also on DFY checkout page (`dfy-minor-child-checkout.html`) — compact two-up reassurance card** | ✅ Full text in doc spec; same compact reassurance text used on the checkout page |
| Robyn Wallace | Google (Oct 2020) | DFY minor-child — card 3 | ✅ Full text in doc spec — uniquely validates procedural rails ("detailed instructions on how to fill out the forms and updates and reminders") |
| Catrice Jackson | Google (Aug 2022) | DFY adult — card 1; **also on DFY adult checkout page (`dfy-adult-checkout.html`) — compact two-up reassurance card** | ✅ Full text in doc spec — only Google review explicitly mentioning adult adoption; checkout page uses curated excerpt: *"Lucrece... went above and beyond to help my family. She was extremely informative, knowledgeable about adult adoption, kind, very patient... and very professional. With her amazing service, my husband was able to legally adopt my 30 year old son."* |
| Gary Boettcher | Google (May 2019) | DFY adult — card 2 | ✅ Full text in doc spec |
| Patty Bales | Google (Sep 2020) | DFY adult — card 3; **also on both DFY checkout pages (`dfy-minor-child-checkout.html` and `dfy-adult-checkout.html`) — compact two-up reassurance card** | ✅ Full text in doc spec — strong "no hidden fees" line; both checkout pages use the same curated excerpt: *"Of course price seems to always play a role and she is very reasonable with no hidden fees!"* |

**Reserved for future pages (do not use elsewhere without trade analysis):**

| Reviewer | Source | Reserved for | Reason |
|---|---|---|---|
| Sarah Hall | Google (Sep 2022) | Future DIY checkout page (`/qualified/diy-minor-child/`) | "Handled everything" reads perfectly for any product. Currently placed on DFY minor-child sales page AND on the DFY checkout page; she can sit on multiple pages since the audiences don't overlap. |
| Kevin Shafer | Google (Jan 2022) | Future page TBD — strong general satisfaction + "would absolutely use again" line | Held in reserve. Strong candidate for About / Founder page, qualifier-results page, or any page needing a generic-but-warm satisfaction quote. |

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
