# Adoption Forms Express — Website Redesign Master Document

**Document type:** Master / index for the entire site redesign
**Owner:** Lucrece H. Bundy / Tyler
**Site:** adoptionformsexpress.com
**Version:** 1.0
**Last updated:** April 28, 2026
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
| Homepage | `/` | Top of funnel, qualifier entry | `homepage-redesign-v1.md` | 🟡 Draft v1.1 — review pending |
| Qualifier quiz | `/qualify` | 60-second eligibility quiz | `qualifier-quiz-v1.md` | ⚪ Not started |
| Pricing | `/pricing` | Standalone pricing comparison | `pricing-page-v1.md` | ⚪ Not started |
| About / Founder | `/about` | Lucrece bio, firm story, credentials | `about-page-v1.md` | ⚪ Not started |
| How It Works | `/how-it-works` | Long-form process walkthrough | `how-it-works-v1.md` | ⚪ Not started |
| Sneak Peek | `/sneak-peek` | Form preview (existing, may need refresh) | `sneak-peek-v1.md` | ⚪ Not started |
| FAQ (full) | `/faq` | Expanded FAQ standalone page | `faq-page-v1.md` | ⚪ Not started |
| County landing pages | `/counties/[county-slug]` | Local SEO — 1 page per priority county | `county-landing-pages-v1.md` | ⚪ Not started |
| Blog | `/blog` | SEO content engine | `seo-content-calendar-v1.md` | ⚪ Not started |
| Conversational AI intake | TBD | Phase 3 AI flow replacing/augmenting qualifier | `conversational-ai-intake-v1.md` | ⚪ Not started |
| Lead magnet landing | `/starter-guide` | Email capture + free PDF | `lead-magnet-v1.md` | ⚪ Not started |
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
| 1 | Tech stack: WordPress vs. Next.js | Open | Recommend Path A for now, decide formally next session |
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

---

## 10. Master Change Log

End every session with an entry here. This is the cross-document log; individual page docs have their own.

| Date | Doc(s) affected | Change | Author |
|---|---|---|---|
| 2026-04-28 | Homepage | v1.0 — Initial homepage redesign spec drafted | Claude / Tyler |
| 2026-04-28 | Homepage | v1.1 — Added Executive Summary section near top | Claude / Tyler |
| 2026-04-28 | **Master** | v1.0 — Master working document created; site architecture, shared standards, master roadmap, master open decisions, change log all established | Claude / Tyler |
| | | | |

---

## 11. Working Document Index

Every doc in the project, with location and current version.

| Doc | Filename | Latest version | Status |
|---|---|---|---|
| **Master** | `website-redesign-master.md` | v1.0 | 🟡 Active |
| Homepage | `homepage-redesign-v1.md` | v1.1 | 🟡 Draft, review pending |
| Qualifier quiz | `qualifier-quiz-v1.md` | — | ⚪ Not started |
| Pricing | `pricing-page-v1.md` | — | ⚪ Not started |
| About / Founder | `about-page-v1.md` | — | ⚪ Not started |
| How It Works | `how-it-works-v1.md` | — | ⚪ Not started |
| FAQ standalone | `faq-page-v1.md` | — | ⚪ Not started |
| Sneak Peek | `sneak-peek-v1.md` | — | ⚪ Not started |
| County landing pages | `county-landing-pages-v1.md` | — | ⚪ Not started |
| SEO content calendar | `seo-content-calendar-v1.md` | — | ⚪ Not started |
| Lead magnet | `lead-magnet-v1.md` | — | ⚪ Not started |
| Conversational AI intake | `conversational-ai-intake-v1.md` | — | ⚪ Not started |
| Disqualified routing | `disqualified-routing-v1.md` | — | ⚪ Not started |
| Legal pages audit | `legal-pages-v1.md` | — | ⚪ Not started |
| Schema library (future) | `schema-library-v1.md` | — | ⚪ Not started |

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
