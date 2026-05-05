# Adoption Forms Express — Website Redesign Master Document

**Document type:** Master / index for the entire site redesign
**Owner:** Lucrece H. Bundy / Tyler
**Site:** adoptionformsexpress.com
**Version:** 1.14
**Last updated:** May 5, 2026
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
| 18 | Support email — dedicated address for these pages | Open | Both DFY page docs reference a `[support email]` placeholder. Recommend creating `support@adoptionformsexpress.com` before publishing. |
| 19 | Review count is hardcoded across pages | ✅ Resolved 2026-04-29 | Decision: visitor-facing review count displays as **"140+"** for durability. Exact `reviewCount` in schema markup remains precise (currently 142) and gets updated quarterly. Revisit live-feed widget integration (option C) post-launch. |
| 20 | Photo-release documentation for testimonials with photos | Open | Kristin's photo is now placed on the homepage. Recommend creating a simple email-based photo-release process: every time a testimonial-with-photo is added, send a one-line confirmation email asking "we'd like to feature your name, testimonial, and photo on the public Adoption Forms Express homepage — is that okay?" and save the email reply. Low-risk for Google-public photos but documents intent for any future dispute. Decide whether to formalize this in a simple template before more photo-paired testimonials are added. |
| 21 | Payment processor: ThriveCart (embedded checkout) | ✅ Resolved 2026-04-30 | ThriveCart embedded checkout is the payment processor for all forms products (DFY minor child, DFY adult, DIY products). Customer stays on the page through the entire transaction. Pages reserve placeholder space for ThriveCart embeds at hero CTA + final CTA. Per-page ThriveCart wiring tracked in each page-level doc. Production snippet for DFY minor-child captured in `dfy-minor-child-page-v1.md` Section 8. |

---

## 10. Master Change Log

End every session with an entry here. This is the cross-document log; individual page docs have their own.

**Older entries archived:** entries from 2026-04-28 through 2026-05-01 (DFY adult two-page funnel completion) live in `website-redesign-master-CHANGELOG.md`. Read that file for the full project history. When this in-line table grows past ~5–7 entries, move the older entries to the archive.

| Date | Doc(s) affected | Change | Author |
|---|---|---|---|
| 2026-05-01 | diy-adult.html, diy-adult-checkout.html, diy-adult-page-v1.md, **Master** | DIY adult funnel built — the FINAL of the four product funnels. Both pages mirror their DIY minor-child counterparts structurally — same CSS, same component patterns, same architecture. Sales page (diy-adult.html) at /diy-adult-sales-page/: DIY-adult-specific copy throughout (4-item qualification recap, adult-aware signature block, court hearing prep emphasis on adult-specific judge questions, FAQ Q4 surfaces name-change use case, three-card testimonial trio with most-layered anxiety coverage in the project — Catrice/Patty/Ruby), CTAs link to /diy-adult-check-out-page/. Checkout page (diy-adult-checkout.html) at /diy-adult-check-out-page/: ThriveCart product 7 embedded (token tc-adoptionssimplified-7-A4PSQA), $299 product summary, testimonials Ruby Leonard (curated excerpt) + Patty Bales. Both pages noindex. diy-adult-page-v1.md → v1.1. Master Section 2 updated: two new architecture rows added (DIY sales — adult + DIY checkout — adult), both 🔵 Built. **The full four-product, eight-page conversion funnel is now feature-complete.** Tyler's WordPress deploy steps: (1) create new top-level WP page at /diy-adult-sales-page/ with Blank Slate template, paste diy-adult.html body content, set noindex via SEO plugin, exclude from sitemap; (2) create separate new top-level WP page at /diy-adult-check-out-page/ with Blank Slate template, paste diy-adult-checkout.html body content, set noindex via SEO plugin, exclude from sitemap; (3) update qualifier quiz Typeform routing logic so DIY-qualifying adult visitors land on /diy-adult-sales-page/. | Claude / Tyler |
| 2026-05-04 | dfy-minor-child.html, dfy-minor-child-page-v1.md | DFY minor-child sales-page hero copy clarified for product specificity. Section 4.2 eyebrow: "✓ You qualify" → "✓ You qualify for the DFY Minor Child Adoption Package". Section 4.2 H1: "You're a great fit for our Done-For-You package." → "You're a great fit for a Minor Child Done-For-You package." Both edits propagated to the HTML. Reason: visitors arriving from the qualifier quiz now see the specific product they qualified for in both the eyebrow and H1, removing ambiguity between minor-child and adult variants. dfy-minor-child-page-v1.md bumped to v2.5. | Claude / Tyler |
| 2026-05-04 | homepage.html, homepage-redesign-v1.md | Homepage polish: hero credibility line and founder credential line both forced to a single line on desktop (smaller font + tighter gap + `white-space: nowrap`, with mobile-only wrap fallback; founder line restructured into three flex spans mirroring the hero pattern). Copy clarity update across three placements — DIY $299 card, DFY $499 card, and What's Included → The Guidance — where "scoped to questions about your forms" was rewritten as "to answer your questions about the forms" (aligns with master Section 3 voice principles; "scoped" reads as legalese). homepage-redesign-v1.md bumped to v2.10. | Claude / Tyler |
| 2026-05-01 | diy-minor-child.html (new), diy-minor-child-checkout.html (new), diy-minor-child-page-v1.md, **Master** | **DIY minor-child funnel built — third of four product funnels now feature-complete.** Both DIY HTML files built as structural siblings of their DFY minor-child counterparts (same CSS, design tokens, component patterns, footer, FAQ accordion mechanic). **Sales page (`diy-minor-child.html`, 1048 lines) at `/diy-minor-sales-page/`:** capability-framed hero ("You're set up to do your stepparent adoption *yourself* — with confidence"), 5-item qualification recap, two-column "What's Included" with bold-stacked Guidance layout (new `.included-col li strong { display: block; ... }` CSS rule keeps the column from reading chopped-up next to the plain-bullet Forms list), 4-step "What Happens Next" with at-your-pace framing, Lucrece signature block + personal-voice quote (new `.signature-quote` element above the name card), three Google-verified testimonials (Ruby Leonard slot 1 — full text, the only forms-product-specific Google review in the entire 142-review set; Sarah Hall slot 2; Kevin Shafer slot 3 — moved out of reserve into placement), 5-question pre-purchase FAQ leading with "What if I get stuck?" anxiety, navy final CTA, escape hatch with upgrade-to-DFY path. `noindex,nofollow` + Product schema only. Both CTAs link to `/diy-minor-checkout-page/`. **Checkout page (`diy-minor-child-checkout.html`, 455 lines) at `/diy-minor-checkout-page/`:** structural sibling of `dfy-minor-child-checkout.html`, ThriveCart product `4` embedded (token `tc-adoptionssimplified-4-TTC0UE`), $299 confirmation header, two-up reassurance testimonials (Ruby Leonard curated excerpt + Patty Bales). **Mid-build copy iterations beyond original v1.0 spec:** (1) Hero qualification recap — "Stepchild is under 19" → "Stepchild is a minor"; consent-state bullet expanded to three states ("will consent, their rights have been terminated, or they are deceased") to mirror the homepage's three-state framing. (2) Forms last bullet — "All forms are blank, ready for you to fill in your information" → "All forms are given to you, ready to fill in with your information" (giving framing). (3) Guidance column restructured to bold-stacked layout. (4) **Email access removed** — dropped Email-access bullet from Guidance (3 items now), removed email-access reference from FAQ Q1 (reframed as "two places to turn"). General contact mailto links remain in nav/footer; product no longer markets ongoing email support as a feature. (5) "What Happens Next" H2 + step 3 H3: `&nbsp;` between "your" and "pace" so "pace" doesn't orphan. (6) **"Instant" framing replaced** across 4 spots (hero CTA note, Step 1 title + description, FAQ Q5, checkout subhead) — page now sets accurate expectations: brief confirmation-email step before delivery, with forms typically sent within one business day. Strategic notes in spec Sections 4.2/4.4/4.6 updated to reflect corrected positioning (still faster than DFY's 3 business days, just not literally instant). **Doc updates:** `diy-minor-child-page-v1.md` → v1.1 (status, header version + last-updated, change-log entry). Master Section 2 — two new architecture rows (DIY sales — minor child + DIY checkout — minor child), both 🔵 Built. Master Section 11 — new umbrella "DIY minor child (sales + checkout)" row at v1.1 / 🔵 Built; existing DFY minor-child row label cleaned up to match the umbrella pattern. Master Section 11.5 — Ruby Leonard, Sarah Hall, Patty Bales placement entries updated; Kevin Shafer moved from reserve to placed; reserve table now empty. **Tyler's WordPress-side action items:** (1) create new top-level WP page at `/diy-minor-sales-page/` with Blank Slate template, paste `diy-minor-child.html` body content, set noindex via SEO plugin, exclude from sitemap; (2) create separate new top-level WP page at `/diy-minor-checkout-page/` with Blank Slate template, paste `diy-minor-child-checkout.html` body content, set noindex via SEO plugin, exclude from sitemap; (3) update qualifier quiz Typeform routing logic so DIY-qualifying minor-child visitors land on `/diy-minor-sales-page/`. The DIY adult funnel is now the only remaining product funnel not yet built. | Claude / Tyler |
| 2026-05-05 | All four checkout HTML files + their spec docs, **Master** | ThriveCart logo updated, which regenerated the embeddable tokens for all four products. Updated all four checkout HTML files with new tokens (DFY minor 10: TOD8DE → UAXWPD; DFY adult 8: 0FGCA9 → POHMYG; DIY minor 4: TTC0UE → KP063D; DIY adult 7: A4PSQA → F1ED0D). Product IDs unchanged. All four spec docs updated to reflect the new snippets. Each spec doc bumped by 0.1. | Claude / Tyler |
| 2026-05-05 | All four checkout HTML files + their spec docs, **Master** | Mobile layout fix applied uniformly to all four checkout pages (`dfy-minor-child-checkout.html`, `dfy-adult-checkout.html`, `diy-minor-child-checkout.html`, `diy-adult-checkout.html`). Added the same `@media (max-width: 720px)` block to each file's embedded `<style>` (immediately after the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule) that tightens `.thrivecart-wrap` vertical padding to `1.5rem 0` and forces `min-height: 0` + `height: auto` on the injected ThriveCart iframe. Reason: Tyler reported that on mobile the injected ThriveCart iframe was being given a desktop-sized fixed height after load, leaving a large empty white gap between the form's "Complete Order" button and the reassurance strip + two-up testimonials below. CSS-only fix; no HTML/copy/schema changes. Each spec doc bumped by 0.1 (DFY minor v2.6 → v2.7, DFY adult v1.11 → v1.12, DIY minor v1.5 → v1.6, DIY adult v1.2 → v1.3). **Known follow-up risk:** if ThriveCart's v2 embed renders inline DOM rather than an iframe on a given page, the `iframe` selector becomes a no-op there and we'll need to inspect the live page to identify the actual element with the fixed pixel height and re-target. **Separate ThriveCart-admin issue still open (not code):** Tyler also flagged a text overlap inside the embed (the testimonial photo/text overlapping the product description/"Especially For You / $499" block on mobile). That's rendered by ThriveCart from product-page settings inside the ThriveCart admin and is not fixable from our checkout HTML — needs to be addressed by repositioning/removing the testimonial widget or shortening the product description in the ThriveCart product page settings. | Claude / Tyler |
| 2026-05-05 | All four checkout HTML files + their spec docs, **Master** | **Reverted the prior entry's mobile fix** across all four checkout pages. The `@media (max-width: 720px)` block was removed from each file, restoring them to their pre-fix state. Reason: forcing `height: auto !important` on the injected ThriveCart iframe collapsed the form into the iframe's intrinsic default height (~150px), squishing the form fields to the point users couldn't comfortably enter their info. The original empty-space gap is back, but the form is fully usable again. Each spec doc bumped by another 0.1 (DFY minor v2.7 → v2.8, DFY adult v1.12 → v1.13, DIY minor v1.6 → v1.7, DIY adult v1.3 → v1.4). **Next step (waiting on Tyler):** before retrying, Tyler will DevTools-inspect the live mobile checkout (Chrome mobile emulation, right-click the empty area → Inspect) and report the actual injected element's tag, class/id, and computed `height` — and the same for its parent. With the real element identified, the next fix can target it precisely instead of guessing at iframe behavior. The text-overlap-inside-embed issue from the prior entry remains unresolved and unrelated — still requires fix in the ThriveCart admin (testimonial widget repositioning / product-description shortening), not in our HTML. | Claude / Tyler |
| 2026-05-05 | dfy-minor-child-checkout.html, dfy-minor-child-page-v1.md, **Master** | ThriveCart embed token regenerated again for **product 10 only** (DFY minor child) after Tyler adjusted spacing in the ThriveCart admin to address the prior text-overlap-inside-embed issue. Confirms the empirical pattern: ThriveCart mints a new embeddable token on most product saves, not just specific changes (logo last time, spacing this time). Product ID unchanged. Old token: UAXWPD → new token: 1OP2TU. Updated `dfy-minor-child-checkout.html` (lines 376–377) and `dfy-minor-child-page-v1.md` (token references via replace_all + change-log entry + version v2.9 → v2.10). Other three checkout files (DFY adult / DIY minor / DIY adult) unaffected — Tyler only edited product 10 in this round. **Reminder for Tyler post-deploy:** retest the mobile checkout to confirm the 1800px iframe-height cap is still appropriate; the form's actual rendered height may have changed with the spacing adjustment. | Claude / Tyler |
| 2026-05-05 | dfy-minor-child-checkout.html, dfy-minor-child-page-v1.md, **Master** | Third ThriveCart token regen of the day for **product 10 only** after Tyler made an additional spacing tweak in the ThriveCart admin to add a bit more room. Product ID unchanged. Old token: 1OP2TU → new token: HV1ZXD. Updated `dfy-minor-child-checkout.html` and `dfy-minor-child-page-v1.md` (token via replace_all + change-log entry + version v2.10 → v2.11). Other three checkout files unaffected. **Reminder for Tyler post-deploy:** retest the mobile checkout — with the additional spacing the form's rendered height likely grew slightly, so the 1800px iframe-height cap may need to be raised if a scrollbar appears inside the embed (or lowered if dead space is still visible). | Claude / Tyler |
| 2026-05-05 | All four checkout HTML files + their spec docs, **Master** | **Mobile empty-space fix v2 (working version) applied uniformly to all four checkout pages.** Tyler's DevTools inspection revealed ThriveCart's embed script injects an `<iframe class="tc-v2-embeddable-el">` (not inline DOM as my read of the prior earlier-shared markup had suggested — that markup was iframe content) inside the `.tc-v2-embeddable-target` div, with an inline `style="height: 2387px"` hardcoded on it. On mobile the form's actual rendered content takes ~1300–1500px, leaving roughly 1000px of dead space that the user scrolls through inside the iframe before reaching our reassurance strip. The iframe also carries `scrolling="yes"`, so capping its height with CSS is safe — any overflow scrolls inside the iframe instead of being clipped. Fix added to all four checkout HTMLs in the same spot (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule): a `@media (max-width: 720px)` block tightening `.thrivecart-wrap` padding to `1.5rem 0` and applying `.thrivecart-wrap iframe.tc-v2-embeddable-el { max-height: 1800px !important; }`. 1800px is intentionally conservative — leaves a buffer for dynamic form expansion (coupon-code section, validation errors, address-state changes) while still cutting most of the dead space. Each spec doc bumped by another 0.1 (DFY minor v2.8 → v2.9, DFY adult v1.13 → v1.14, DIY minor v1.7 → v1.8, DIY adult v1.4 → v1.5). **Tuning playbook for Tyler post-deploy:** if dead space is still visible, lower the cap (1500 → 1300); if a scrollbar appears inside the iframe because the form was clipped, raise it (2000+). Desktop behavior unchanged. CSS-only; no HTML/copy/schema changes. The text-overlap-inside-embed issue (testimonial photo overlapping product description in the form area) remains a separate, unresolved ThriveCart-admin issue — not fixable from our checkout HTML. | Claude / Tyler |
| 2026-05-05 | All HTML files + 5 spec docs + Master | UPL-driven language change. Replaced "attorney call(s)" with "support call(s)" framing across the entire project. DFY products: "two 15-minute support calls". DIY products: "one 30-minute support call". Total support time per product unchanged (30 min). Added protective note on all 4 sales pages: "Support calls are for questions about your forms and the filing process — not personalized legal advice. If you need legal advice about your specific case, please contact a licensed attorney directly." Master doc Section 7 (Tech stack) line about Calendly also updated to drop "free attorney calls" framing. Schema descriptions across all 4 products updated. **Per Flag C resolution:** the DFY checkout schema/meta lines that previously read "Completed by a licensed Nebraska adoption attorney within 3 business days" were also updated to "Completed by our team within 3 business days" — the attorney designed/prepared the form templates (Lucrece's pedigree remains via "Attorney-prepared..." which is left intact), but the per-customer form completion is done by the team, not the attorney directly. Same edit applied to DFY sales pages' final-CTA paragraphs. Reviewed and approved by Lucrece H. Bundy, Esq. as licensed attorney owner. Per master doc Section 3 compliance review trigger, this approval is recorded in writing here. **Spec docs bumped:** homepage-redesign-v1.md v2.10 → v2.11; dfy-minor-child-page-v1.md v2.11 → v2.12; dfy-adult-page-v1.md v1.14 → v1.15; diy-minor-child-page-v1.md v1.8 → v1.9; diy-adult-page-v1.md v1.5 → v1.6. **One small additional voice edit Tyler should know about** — in `diy-adult.html`'s Lucrece signature quote, the original phrase "direct access to me when something specific to their adoption comes up" was implying Lucrece-as-attorney availability for the call, which contradicts the new support-call framing. Replaced with "a place to turn when something specific to their adoption comes up." If Tyler prefers a different wording there, easy follow-up. | Claude / Lucrece |
| | | | |

---

## 11. Working Document Index

Every doc in the project, with location and current version.

| Doc | Filename | Latest version | Status |
|---|---|---|---|
| **Master** | `website-redesign-master.md` | v1.14 | 🟡 Active |
| Homepage | `homepage-redesign-v1.md` | v2.11 | 🔵 Built (`homepage.html`), ready for WordPress deploy |
| Qualifier quiz | `qualifier-quiz-v1.md` | — | ⚪ Not started |
| Pricing | `pricing-page-v1.md` | — | ⚪ Not started |
| DFY minor child (sales + checkout) | `dfy-minor-child-page-v1.md` | v2.12 | 🔵 Built — `dfy-minor-child.html` (sales page) + `dfy-minor-child-checkout.html` (transactional checkout, ThriveCart product 10) both on disk, ready for WordPress deploy |
| DFY sales — adult | `dfy-adult-page-v1.md` | v1.15 | 🔵 Built — `dfy-adult.html` (sales page) + `dfy-adult-checkout.html` (transactional checkout, ThriveCart product 8) both on disk, ready for WordPress deploy |
| DIY minor child (sales + checkout) | `diy-minor-child-page-v1.md` | v1.9 | 🔵 Built — `diy-minor-child.html` (sales page) + `diy-minor-child-checkout.html` (transactional checkout, ThriveCart product 4) both on disk, ready for WordPress deploy |
| DIY adult (sales + checkout) | `diy-adult-page-v1.md` | v1.6 | 🔵 Built — `diy-adult.html` (sales page) + `diy-adult-checkout.html` (transactional checkout, ThriveCart product 7) both on disk, ready for WordPress deploy |
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
