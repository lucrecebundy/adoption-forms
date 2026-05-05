# Done-For-You Minor-Child Stepparent Adoption — Post-Qualification Checkout Page

**Document type:** Page-level working document
**Owner:** Lucrece H. Bundy / Tyler
**URLs:** `/dfy-minor-sales-page/` (sales page — `dfy-minor-child.html`); `/dfy-child-check-out-page/` (transactional checkout page — `dfy-minor-child-checkout.html`). The two pages are sibling top-level pages in WordPress (not parent/child).
**Replaces:** `/customized-adoption-forms/` (split into two pages by audience)
**Sister doc:** `dfy-adult-page-v1.md` (adult-adoption equivalent)
**Version:** 2.10
**Last updated:** May 5, 2026
**Status:** Built — both `dfy-minor-child.html` (post-quiz sales page) and `dfy-minor-child-checkout.html` (transactional checkout page housing the ThriveCart embed) now exist on disk; ready for WordPress deploy

---

## How to Use This Document

This is the page-level working doc for the **post-qualification checkout page** for the Done-For-You product when the qualifying case involves a **minor child** (under 19). It assumes the master doc (`website-redesign-master.md`) is already loaded and inherits all site-wide standards from it (brand voice, UPL guardrails, design tokens, etc.).

The adult-adoption equivalent lives in a separate sister doc (`dfy-adult-page-v1.md`). The two docs share structure; only the audience-specific content differs.

---

## 1. Strategic Frame — What This Page Is And Isn't

### What this page IS

A **post-qualification checkout page**. The visitor has already:

1. Found the site
2. Decided to take the qualifier quiz
3. Completed the quiz
4. Been told they qualify for the Done-For-You package
5. Been routed here by the quiz logic because the case involves a minor child

By the time they're on this page, they've made every meaningful decision except *click the buy button*. The page exists to make them feel **confident, informed, and ready** to pay $499 right now.

### What this page IS NOT

- **Not an SEO page.** It carries `<meta name="robots" content="noindex,nofollow">`. It is not in the sitemap. We do not want strangers landing here.
- **Not a marketing page.** No selling. No persuasion. No competitor comparisons. The visitor is already sold — anything that feels like marketing is friction.
- **Not a discovery page.** No links to "learn more," "see other options," "compare products." Every link off this page is either the purchase button, the support escape hatch, or footer-standard.
- **Not the SEO pillar.** A separate, future, public-facing page (`/done-for-you-adoption-forms-nebraska/`) will do that job. That page funnels TO the qualifier quiz; this page is what's BEHIND the qualifier quiz.

### Why the gating matters

If a stranger lands on this page from a Google search, they see "$499" with no context for who Lucrece is, what the qualifier rules out, or why the price is what it is. They bounce. Worse, they could buy without qualifying first — creating refund overhead and possible UPL exposure if their case isn't actually a fit. The qualifier quiz IS the gate. This page is what's behind the gate.

### One-line page goal

**Confirm qualification → reinforce trust → enable instant purchase.**

---

## 2. The Visitor — Who Lands Here

A married Nebraska resident who:

- Just completed the qualifier quiz
- Has been told they qualify
- Their stepchild is a minor (under 19)
- Has chosen the Done-For-You option (vs. DIY)
- Is ready to pay $499 today, but wants reassurance before clicking

What they need from this page:

- Confirmation they're in the right place
- A clear, complete picture of what they're paying for
- A specific picture of what happens *next* after they pay
- Reassurance that they're not alone in this — Lucrece is real and reachable
- An easy, fast purchase path

What they do NOT need from this page:

- A pitch
- A comparison to DIY
- A long-form FAQ on Nebraska adoption law (that's the homepage's job)
- A pricing comparison to other attorneys (the qualifier already established this)
- More social proof than necessary

---

## 3. Page Structure (Top to Bottom)

```
1.  Sticky nav (logo only — no menu items, this is a checkout-style page)
2.  Hero / Qualification Confirmation
3.  What You Get (the package, fully spelled out)
4.  How It Works After You Order (the next 3-day flow)
5.  Trust block (Lucrece signature, 3 forms-specific testimonials)
6.  Pre-purchase FAQ (short, focused on last-minute concerns)
7.  Final CTA (the purchase button, large, obvious)
8.  Escape hatch (small, "if your situation has changed")
9.  Footer (with UPL disclaimer)
```

**Roughly half the length of the homepage.** This is intentional — every section that doesn't move the visitor closer to clicking buy is friction.

---

## 4. Section-by-Section Copy

### 4.1 Sticky Nav

A stripped-down nav. No "How It Works," no "FAQ," no "Pricing." We don't want them browsing — we want them buying.

```
[Logo: Adoption Forms Express]                    Need help? Email us →
```

**Notes:**
- The logo links to homepage but doesn't draw attention to it
- Right-side link is a `mailto:` to your support inbox — not a phone number, not a "book a call" CTA
- No hamburger on mobile — just logo + email link

---

### 4.2 Hero / Qualification Confirmation

This is the most important section. It must feel like a continuation of the quiz.

**Eyebrow (small, success green):**
✓ You qualify for the DFY Minor Child Adoption Package

**H1:**
You're a great fit for a Minor Child Done-For-You package.

**Subhead:**
Based on your answers, your Nebraska stepparent adoption is exactly the kind of case our Done-For-You package was built for. Here's what you'll get and what happens next.

**Below the subhead — qualification recap (callout box):**
> Based on your quiz answers:
> ✓ You're legally married to the child's biological parent
> ✓ Your stepchild is a minor and has lived with you for 6+ months
> ✓ You meet Nebraska's age and residency requirements
> ✓ Your case is uncontested
>
> *That makes you a perfect fit for the $499 Done-For-You package.*

**Primary CTA — ThriveCart embed:**

This is the first of two ThriveCart embed locations on the page (hero + final CTA). The button rendered by ThriveCart triggers the embedded checkout experience — customer stays on the page through the entire transaction.

The production embed snippet is captured in Section 8 (ThriveCart Integration). Paste it here at HTML build time.

The button styling should match the homepage's primary CTA (warm coral, rounded, prominent). Check ThriveCart's button-styling options to use site colors; if ThriveCart's styling controls are limited, wrap their default button in a styled container.

**Below the CTA, small text:**
*Secure checkout · Most orders delivered within 3 business days*

**Notes:**
- The "you qualify" eyebrow does heavy emotional work — it confirms what the quiz just told them and grounds the page
- The qualification recap is critical: it bridges the quiz outcome and the page content. The visitor should feel "yes, this page is for me, specifically"
- The CTA appears here above the fold so a visitor who's already decided can buy immediately without scrolling. Most won't — but the option being there reduces anxiety
- "Secure checkout" + the turnaround line are micro-trust signals at the moment of decision
- **ThriveCart integration:** the embed handles the entire transaction — credit card collection, processing, confirmation, and customer email — without leaving the page. The page just reserves visual real estate for ThriveCart's button and (typically) a popup overlay.

---

### 4.3 What You Get

The full product spelled out. No mystery, no padding.

**Eyebrow:** WHAT'S INCLUDED

**H2:** Everything you need to finalize your stepparent adoption.

**Two-column layout:**

**Column 1 — The Forms (completed by us)**
- Petition for Adoption (Nebraska form, completed with your information)
- Consent forms
- Notice of Adoption
- Decree of Adoption (proposed)
- All other Nebraska-required supporting documents based on your specific situation

**Column 2 — The Guidance**
- Step-by-step filing instructions specific to your Nebraska county court
- Court hearing prep document with the exact questions a Nebraska judge is most likely to ask
- Background check instructions — you complete the checks yourself; we provide step-by-step guidance for what your county requires
- New birth certificate ordering instructions
- **Two free 15-minute calls** with Lucrece Bundy, Esq. (a licensed Nebraska adoption attorney) to answer questions about your forms

**Below the columns:**
*Court filing fees (~$60–$90 depending on county) and certified copy fees are paid directly to your local court and not included.*

**Notes:**
- Listing each form by its real name reinforces "this is a real attorney product, not a template fill-in"
- The "completed with your information" emphasis in column 1 is the key DFY differentiator — separates this from the DIY package
- The two attorney calls are a premium touch worth highlighting — most product purchases at this price don't include direct attorney access
- The filing fee disclosure is here (not buried) because it's the single most common refund-trigger surprise for new buyers

---

### 4.4 How It Works After You Order

This is the section that closes the deal for hesitant buyers. They want to know exactly what happens after they click the button.

**Eyebrow:** WHAT HAPPENS NEXT

**H2:** From order to inbox in 3 business days.

**4-step horizontal layout:**

**Step 1 — You complete a secure intake form (15 minutes)**
After payment, you'll get a link to a confidential intake form. You'll provide the names, dates, addresses, and details our team needs to fill out your forms accurately. Most families finish in 10–15 minutes.

**Step 2 — Our team prepares your forms (1–3 business days)**
Our team completes your forms, and Lucrece personally reviews every package before it goes out. No rush, no template-fill — every detail is checked against Nebraska statute and your specific situation.

**Step 3 — You receive your completed package by email**
Your package will include every form filled out and ready to file, your county-specific filing checklist, your court hearing prep guide, and the ordering instructions for your new birth certificate.

**Step 4 — You file with your county court**
Take your forms to your county court clerk. Pay the filing fee (~$60–$90). Get your hearing date. Your two free 15-minute attorney calls are available throughout — schedule them whenever you need them.

**Below the steps:**
*Most uncontested Nebraska stepparent adoptions finalize 4–6 months after filing.*

**Notes:**
- The 15-minute intake estimate sets expectations that this is fast — not another long ordeal
- "Lucrece personally reviews every package" is critical and true. It's the trust anchor of the whole product. Don't soften it.
- The 4–6 month timeline at the bottom manages the post-purchase expectation curve — this is the data point most likely to come back as a "why is this taking so long?" support email if not pre-set
- Each step is concrete and time-bound. Vague steps create anxiety; specific steps create confidence.

---

### 4.5 Trust Block

Brief. Specifically targeted. Not exhaustive.

**Eyebrow:** YOU'RE IN GOOD HANDS

**Small Lucrece signature block (compact, left-aligned, with thumbnail photo on the side):**

[Photo: Lucrece's professional headshot, small and circular]

**Lucrece H. Bundy, Esq.**
Founder, Adoption Forms Express
Licensed Nebraska Adoption Attorney
200+ Nebraska Adoptions Finalized

**Below the signature block — three short stepparent-adoption-specific testimonials:**

**Three review cards (Google-verified, all stepparent adoption clients):**

> "I chose Bundy Law to complete a stepparent adoption. I was truly amazed at how pain-free Lucrece made the process. In the past, with custody orders it has been so much work, but Lucrece handled everything. I felt like I could breathe for the first time in nearly a decade. From the first phone call we had, I knew she was the right choice. Before I even hired her she gave me great advice, which made me feel that she truly cares about the adoption process and this isn't just another case to her. I definitely made the right choice in my representation. Thanks again Lucrece!"
> — Jennifer Jenkins (Apr 2025)
>
> **Curated excerpt for HTML three-up card** (locked v2.3 — shorter version chosen for visual balance with Sarah's and Robyn's cards; drops the front and back framing while preserving the strongest emotional beats including "I could breathe for the first time in nearly a decade" and the "she truly cares" line):
>
> > "I was truly amazed at how pain-free Lucrece made the process. In the past, with custody orders it has been so much work, but Lucrece handled everything. I felt like I could breathe for the first time in nearly a decade. Before I even hired her she gave me great advice, which made me feel that she truly cares about the adoption process and this isn't just another case to her."

> "The adoption process was quick and effortless. Mrs. Bundy handled everything for us. We couldn't be more happy!"
> — Sarah Hall (Sep 2022)

> "Working with Lucrece was amazing! Our stepparent adoption went so smoothly, and she did all the work! We also got detailed instructions on how to fill out the forms and updates and reminders as the process progressed. Our day in court was so smooth, and Lucrece was so helpful, kind, and easy to work with. Definitely recommend!"
> — Robyn Wallace (Oct 2020)

**Notes:**
- Three testimonials is enough. More than that and we're padding.
- Curated testimonials > full review wall on this page. The homepage already has the full Trustindex widget; no need to duplicate.
- The Lucrece signature block is the single most important trust element. Real attorney, real face, real credentials, real number of cases.
- Sarah Hall's "handled everything for us" is the single most powerful line for a Done-For-You product page — it's the visitor's expectation in their own words.
- Robyn Wallace's "detailed instructions on how to fill out the forms and updates and reminders" is a uniquely valuable line: it validates the procedural rails of the product (instructions, reminders, updates), not just the outcome. This is the part anxious buyers want to hear most.
- Each testimonial does a different job: Jennifer (recent + emotional/anxiety reduction), Sarah (DFY product promise — "handled everything"), Robyn (procedural specifics — "instructions, reminders, updates").

---

### 4.6 Pre-Purchase FAQ

Tightly focused on last-second purchase concerns. NOT general adoption-law FAQs (those live on the homepage and standalone FAQ page).

**Eyebrow:** BEFORE YOU PURCHASE

**H2:** A few quick answers.

**Accordion FAQ (5 questions, all about the buying experience):**

**Q: What if I realize my case is more complicated than I thought after I order?**
Email us at [support email] within 7 days of purchase and we'll review your situation. If your case turns out not to be a fit for the Done-For-You package, we'll refund your purchase in full. If your case needs full attorney representation, we'll connect you directly with Bundy Law LLC.

**Q: What information do I need to provide?**
The intake form will ask for the legal names of all parties, the child's birth certificate details, your marriage certificate details, addresses, and basic case history. You won't need to provide anything you don't already have on hand.

**Q: How long does turnaround take?**
Most Done-For-You packages are completed and delivered within 3 business days of receiving your intake form. If your case has unusual circumstances (e.g., unusual non-custodial parent situation), it may take an extra day or two — we'll let you know.

**Q: What if I have questions during my case?**
Your package includes two free 15-minute attorney calls with Lucrece, available whenever you need them — before filing, before your hearing, or at any point in between. The calls are scoped to questions about your forms package.

**Q: What does the $499 not include?**
The $499 covers your completed forms package, the two attorney calls, and the filing/hearing/birth certificate guidance. It does NOT cover your county's filing fee (~$60–$90 paid directly to the court), certified copies of your finalized adoption decree, or any background-check fees if your county requires them.

**Notes:**
- Five questions max. The visitor's hand is on the buy button — too many FAQs sends them down a rabbit hole.
- The refund question is critical and goes first because it directly defuses the biggest anxiety: "what if I bought the wrong thing?"
- Every answer reinforces what's in the package vs. what isn't, with no ambiguity
- The "what does it not include" question is anti-buyer-remorse insurance

---

### 4.7 Final CTA

Single, large, unmissable.

**H2:** Ready to get started?

**Below H2:**
Your Done-For-You package, completed by a licensed Nebraska adoption attorney, delivered in 3 business days.

**Primary CTA — ThriveCart embed (second location):**

Same ThriveCart embed snippet as the hero CTA. Paste the captured snippet from Section 8 here as well, styled to be large and centered.

**Important:** ThriveCart sometimes requires unique IDs or different handling when the same product embed appears more than once on the same page. The captured snippet uses `id="tc-adoptionssimplified-10-1OP2TU"` on the script tag — when reused twice, both instances share the same ID, which is invalid HTML and may cause the second embed to misbehave. See Section 8 for fix options if it does.

**Below the CTA, small reassurance line:**
*Secure checkout · 7-day refund if your case isn't a fit · Questions? [Email us]*

**Notes:**
- This is the only CTA below the fold. No "or compare to DIY," no "or book a consult."
- The reassurance line consolidates the three biggest pre-click anxieties (security, refund, support) into one tight stripe of text
- The email link is a soft escape hatch — gives the hesitant buyer somewhere to go besides clicking the back button

---

### 4.8 Escape Hatch (Small, Discreet)

Below the final CTA, in muted text:

*If your situation has changed since you took the qualifier quiz — for example, your spouse's other parent is no longer agreeing to the adoption, or your case is now contested — please email us at [support email] before purchasing. We can connect you with Bundy Law LLC for full attorney representation if your case has become contested.*

**Notes:**
- Required for UPL protection — gives anyone whose situation has shifted a clean off-ramp
- Phrased as guidance, not warning — we're not trying to scare them away from the purchase
- Important: this routes contested cases to Bundy Law (revenue stays in the family of businesses)

---

### 4.9 Footer

Same footer as homepage, with the standard UPL disclaimer. No changes.

---

## 5. Visual System

Inherits everything from `website-redesign-master.md` Section 4. No page-specific overrides.

The page should feel **calmer and more focused** than the homepage. Specifically:

- Less section-to-section color contrast (avoid alternating between cream and white aggressively — keep most of the page on the cream background for continuity)
- More whitespace around the primary CTA
- The qualification confirmation block should feel celebratory but not loud — think "warm welcome" not "sales push"
- Lucrece's photo should be smaller than on the homepage (signature block, not founder spotlight) — we don't need to re-establish credibility; the visitor came in already trusting

---

## 6. SEO & Indexing

### Critical: this page is NOT indexed.

**`<head>` requirements:**
```html
<meta name="robots" content="noindex,nofollow">
<link rel="canonical" href="https://adoptionformsexpress.com/dfy-minor-sales-page/">
```

**Sitemap:** Not included in `sitemap.xml`.

**Internal links:** No site-wide nav links to this page. Only entrypoint is the qualifier quiz Typeform redirect.

**Why no indexing:**
- Strangers shouldn't land here without context
- The qualifier quiz is the gate; this page is what's behind the gate
- We don't want this page competing with our (future) public-facing pillar page for Done-For-You searches

### Future SEO sister page

A public-facing pillar page (`/done-for-you-adoption-forms-nebraska/`) will be built in a future phase. That page:
- IS indexed
- Targets keywords like "nebraska done for you adoption forms," "nebraska stepparent adoption attorney prepare forms"
- Funnels TO the qualifier quiz
- Does the SEO and AI search work this page deliberately doesn't

That work is tracked separately in the master doc.

---

## 7. Schema Markup

Minimal — we don't want this page generating rich results in search since it shouldn't be in search.

**Recommended:**

`Product` schema (without `aggregateRating` to avoid implying public reviewability of this specific URL):

```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "Done-For-You Nebraska Stepparent Adoption Forms (Minor Child)",
  "description": "Attorney-prepared Nebraska stepparent adoption forms for minor-child cases. Completed by a licensed Nebraska adoption attorney within 3 business days. Includes two attorney calls and complete filing guidance.",
  "brand": { "@type": "Brand", "name": "Adoption Forms Express" },
  "offers": {
    "@type": "Offer",
    "price": "499",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock"
  }
}
```

**NOT included on this page:** `FAQPage` schema. The pre-purchase FAQ here is for buyers, not searchers. We don't want these Q&As surfacing as rich results.

---

## 8. Technical Implementation Notes

- Page is built as a single self-contained HTML file in the same style as `homepage.html`
- Same design tokens, typography, button styles, FAQ accordion logic
- File name: `dfy-minor-child.html`
- Deployed to URLs: `/dfy-minor-sales-page/` (sales page) and `/dfy-child-check-out-page/` (transactional checkout where ThriveCart is embedded). The two pages are sibling top-level WordPress pages — not parent/child. The sales page's two CTA buttons link to the checkout page; the checkout page is the only place ThriveCart loads.
- WordPress: the page already exists on the live WordPress site at this URL with the old design; the new HTML build replaces its content at the same URL
- WordPress page settings: set to "noindex" via your SEO plugin (Yoast, Rank Math, etc.) — belt-and-suspenders alongside the meta tag
- Removed from primary nav menu
- 301 redirect: old `/customized-adoption-forms/` page redirects to `/` (homepage) so the existing inbound SEO equity flows somewhere useful instead of evaporating

### ThriveCart Integration

**Payment processor:** ThriveCart (embedded checkout — customer stays on the page through the entire transaction).

**Captured embed snippet** (resolved 2026-04-30 — production snippet for the $499 DFY Minor-Child product, provided by Tyler from ThriveCart admin):

```html
<div class="tc-v2-embeddable-target" data-thrivecart-account="adoptionssimplified" data-thrivecart-tpl="v2" data-thrivecart-product="10" data-thrivecart-embeddable="tc-adoptionssimplified-10-1OP2TU"></div>
<script async src="//tinder.thrivecart.com/embed/v2/thrivecart.js" id="tc-adoptionssimplified-10-1OP2TU"></script>
```

Account `adoptionssimplified` · Product ID `10` · Embed token `tc-adoptionssimplified-10-1OP2TU`. Paste at both CTA locations (Section 4.2 hero + Section 4.7 final CTA) during HTML build.

**Two embed locations on the page:**
1. Hero CTA (Section 4.2) — one ThriveCart embed
2. Final CTA (Section 4.7) — second ThriveCart embed

**Implementation details for the HTML build:**
- Paste the snippet above at both CTA locations
- Style the surrounding container at both locations to match the homepage's primary CTA visual treatment (warm coral, generous padding, prominent placement)
- ThriveCart's button styling can usually be customized in the ThriveCart admin — match brand colors there if possible, otherwise wrap their button in a styled container

**Known wrinkles to watch for:**
- **Duplicate-`id` consideration:** the snippet's `<script>` tag has `id="tc-adoptionssimplified-10-1OP2TU"`. Pasting it twice creates two `<script>` tags with the same `id`, which is invalid HTML and may cause the second embed to misbehave. If the second embed fails to render on test: (a) ask ThriveCart for a second-instance variant, or (b) manually unique-ify the `id` on the second `<script>` AND the matching `data-thrivecart-embeddable` attribute on its `<div>` (e.g., suffix both with `-2`)
- ThriveCart popups sometimes interact poorly with site headers/footers that have `position: sticky` — test the popup overlay on mobile after deployment
- The embedded ThriveCart cart may load slightly slower than the rest of the page; consider a "Loading checkout…" skeleton state during JS load

**What ThriveCart handles automatically (no extra work for the page):**
- Credit card collection and processing
- Order confirmation page (set up in ThriveCart admin to redirect to the post-purchase intake form)
- Customer email receipt
- Refund handling

**What still needs to be set up separately (post-deployment, not in this build):**
- ThriveCart "thank you" / success URL → redirect to a post-purchase intake form (Typeform, JotForm, or similar) to collect the customer's case data
- ThriveCart webhook to email the team when an order comes in
- ThriveCart refund policy aligned with the "7-day refund if case isn't a fit" copy on the page

---

## 9. Open Questions / Decisions Needed

| # | Question | Status | Notes |
|---|---|---|---|
| 1 | Collect 3 forms-product-specific testimonials | ✅ Resolved 2026-04-29 | Locked: Jennifer Jenkins (truncated — pull full from Google), Sarah Hall (full text), Kevin Shafer (full text). All three are Google-verified stepparent adoption clients. |
| 2 | Final support email for the page | Open | Recommend a dedicated `support@adoptionformsexpress.com` instead of the current Gmail. Decide before launch. |
| 3 | Refund policy specifics | Open | "7-day refund if case isn't a fit" is proposed copy — Lucrece should confirm the actual policy before publishing. |
| 4 | Intake form mechanism | Open | Currently stated as "you'll get a link to a confidential intake form" — confirm what tool (Typeform? Google Form? JotForm? Custom?) so we can wire the post-purchase flow. |
| 5 | Quiz routing logic | Open | The Typeform must be configured so that qualifying minor-child cases route here, qualifying adult cases route to the adult page, and disqualified visitors route to a disqualified-routing page. Need to verify quiz logic supports this. |
| 6 | County-specific filing-fee accuracy | Open | $60–$90 range — Lucrece to confirm current Nebraska filing-fee range. |
| 7 | Background check fee disclosure | Open | Current FAQ mentions "background-check fees if your county requires them" — confirm which counties require this and what the fee range is. |
| 8 | ThriveCart embed snippet | ✅ Resolved 2026-04-30 | Production snippet captured verbatim in Section 8. Account: `adoptionssimplified` · Product `10` · Embed token `tc-adoptionssimplified-10-1OP2TU`. To be pasted at both CTA locations during HTML build. |
| 9 | ThriveCart success URL → intake form wiring | Open | After successful purchase, ThriveCart should redirect customer to a post-purchase intake form. Confirm the intake form tool (Typeform/JotForm/etc.) and configure the success URL in ThriveCart admin. Tied to Open Question #4. |
| 10 | ThriveCart button styling | Open | Decide whether to (a) configure ThriveCart's native button styling in their admin to match site colors, or (b) wrap their button in a styled site container. Visual decision affecting hero + final CTA appearance. |

---

## 10. Change Log

| Date | Change | Author |
|---|---|---|
| 2026-04-28 | v1.0 — Initial DFY minor-child page spec drafted | Claude / Tyler |
| 2026-04-29 | v1.1 — Section 4.3: removed "Waiver of Notice" from forms list; removed "Email access for follow-up questions" from guidance list; clarified the 2 attorney calls are scoped to questions about the forms package. Section 4.4: timeline updated from 2–4 months to 4–6 months (and matching reference in notes). Section 4.6 FAQ Q4: removed reference to email support to stay consistent with package change. | Claude / Tyler |
| 2026-04-29 | v1.2 — Section 4.5 testimonials locked: Jennifer Jenkins (truncated — pull full from Google), Sarah Hall (full text), Kevin Shafer (full text). All Google-verified stepparent-adoption clients. Open Question #1 resolved. | Claude / Tyler |
| 2026-04-29 | v1.3 — Kevin Shafer swapped out for Robyn Wallace in Section 4.5 (third testimonial slot). Reason: Robyn's review uniquely validates the procedural rails of the product ("detailed instructions on how to fill out the forms and updates and reminders as the process progressed") — much stronger for a checkout page than Kevin's general satisfaction. Kevin moved into testimonial reserve registry for future page placement. New trio: Jennifer (anxiety relief), Sarah (DFY promise), Robyn (procedural specifics). | Claude / Tyler |
| 2026-04-29 | v2.0 — Built `dfy-minor-child.html`: single self-contained HTML file matching `homepage.html`'s design language (Fraunces + Manrope, same color palette, same FAQ accordion mechanic). Includes: stripped checkout-style nav, qualification-confirmation hero with success-green eyebrow + qualification recap callout, "What's Included" two-column section, "What Happens Next" 4-step timeline, Lucrece signature block (small circular photo) + 3 forms-product-specific testimonials, 5-question pre-purchase FAQ (no FAQPage schema by design), navy final-CTA band, escape hatch for contested-case routing. Schema: Product only (`noindex,nofollow`). Buy buttons placeholder-linked to `#` with TODO comments for Stripe URL. | Claude / Tyler |
| 2026-04-29 | v2.1 — Content edits made during build review, propagated to both spec doc and HTML. Section 4.3 (What's Included): "Notice of Hearing" → "Notice of Adoption" (form-name correction); "Background check authorizations" moved from Forms column to Guidance column with new framing — "Background check instructions — you complete the checks yourself; we provide step-by-step guidance for what your county requires"; "Consent forms — custodial parent, plus non-custodial where applicable" simplified to just "Consent forms". Section 4.4 (What Happens Next): H2 "From order to filed forms in 3 business days" → "From order to inbox in 3 business days" (the 3-day window is delivery, not filing — visitors won't necessarily file the day they receive forms); step 2 "A trained paralegal completes your forms" → "Our team completes your forms"; step 3 "You'll get a PDF package with…" rewritten to "Your package will include…" (we deliver via Google Drive link in practice, but the page no longer specifies delivery format). | Claude / Tyler |
| 2026-04-29 | v2.2 — Form Sneak Peek removed across the project; lead-magnet freebie replaces it. dfy-minor-child.html footer: "Form Sneak Peek" link → "Free Nebraska Adoption Guide" (stubbed `#` with TODO for the future `/starter-guide` URL). No on-page-content changes — DFY checkout page deliberately stays focused on purchase, so the freebie only appears in the footer (not in the body, hero, or final CTA). Spec doc Section 4.9 still says "Same footer as homepage, with the standard UPL disclaimer. No changes." — that statement remains accurate; the homepage footer just gained a different Services link. | Claude / Tyler |
| 2026-04-30 | v2.3 — Three layered changes ported in one update. (1) **URL alignment:** confirmed the live URL is `/buy-doneforyou-minor/` (not the placeholder `/qualified/done-for-you-minor-child/` we'd been using); updated header URL line, Section 6 canonical, Section 8 deployment URL. The page already exists on the live WordPress site at this URL; the new HTML build replaces its content. (2) **ThriveCart Integration:** Section 4.2 (hero CTA) and 4.7 (final CTA) updated to use ThriveCart embed instead of standard button. Section 8 gains new "ThriveCart Integration" subsection with the production embed snippet captured verbatim (account `adoptionssimplified`, product `10`, embed token `tc-adoptionssimplified-10-1OP2TU`); duplicate-`id` test consideration documented; what ThriveCart handles automatically vs. what still needs separate setup also captured. Section 9 gains Open Questions #8 (✅ resolved with snippet), #9 (success URL wiring, open), #10 (button styling decision, open). (3) **Jennifer Jenkins testimonial:** Section 4.5 full review text captured verbatim; curated excerpt locked for the HTML three-up card (visual balance with Sarah's and Robyn's cards — drops front/back framing, preserves the strongest emotional beats including "I could breathe for the first time in nearly a decade" and "she truly cares about the adoption process"). | Claude / Tyler |
| 2026-05-01 | v2.4 — `dfy-minor-child-checkout.html` refactored from a sales-page clone (1027 lines, full hero/qualification-recap/What-You-Get/How-It-Works/Lucrece-signature/FAQ/dual-ThriveCart-embeds) into a true short transactional checkout page (~455 lines, 44% of original). New page structure: minimal nav → success-green confirmation header (✓ Secure checkout pill + product-name H1 + `$499 · 3-business-day delivery · 2 attorney calls` subhead) → smaller h2 "Complete your payment below" → single full-width ThriveCart embed → lock-emoji reassurance strip → two compact two-up testimonials (Sarah Hall, Patty Bales) → standard footer. **Funnel architecture clarified this session:** Homepage → Qualifier Quiz → DFY Sales Page (`dfy-minor-child.html`) → DFY Checkout Page (`dfy-minor-child-checkout.html`) → ThriveCart processes payment. The sales page does the convincing; the checkout page only takes payment. **Note:** the spec body of this doc (Sections 4.2, 4.7, 8) still describes the original single-page architecture with two ThriveCart embed locations on a single page — the body has not been rewritten to reflect the two-file split. That decision (full v3.0 rewrite vs. keep this doc + write a separate `dfy-minor-child-checkout-v1.md`) is deferred. **Note:** the checkout page currently has `<link rel="canonical">` pointing to `/buy-doneforyou-minor/`, which is also the sales page's URL — needs URL resolution before WordPress deploy. | Claude / Tyler |
| 2026-05-01 | URL conflict resolved (open issue from earlier in session). Two-page funnel now has two distinct URLs: sales page at `/buy-doneforyou-minor/` (existing live URL — unchanged so the qualifier-quiz Typeform redirect keeps working), checkout page at `/buy-doneforyou-minor/checkout/` (new sub-path). Header URL line in this doc updated from single URL to both URLs. Section 8 deployment URL line updated to reflect both URLs and the role of each. `dfy-minor-child-checkout.html` canonical updated to `https://adoptionformsexpress.com/buy-doneforyou-minor/checkout/`. The two CTA buttons on `dfy-minor-child.html` (hero + final CTA) — previously placeholder `<a href="#">` with TODO comments — now link to `/buy-doneforyou-minor/checkout/`; stale TODO comments removed. ThriveCart embed only loads on the checkout page (no duplicate-instance concern). **WordPress deploy step (Tyler):** create the new checkout WP page as a child of the existing Buy DFY Minor page with slug `checkout`, paste the `dfy-minor-child-checkout.html` body content, mark noindex via SEO plugin. | Claude / Tyler |
| 2026-05-01 | Checkout URL revised: Tyler created the WordPress checkout page as a **top-level page** at `/dfy-child-check-out-page/` rather than as a child page at `/buy-doneforyou-minor/checkout/`. The two pages are now sibling top-level WordPress pages, not parent/child. URLs aligned across all four files: `dfy-minor-child-checkout.html` canonical now `https://adoptionformsexpress.com/dfy-child-check-out-page/`; `dfy-minor-child.html` two CTA buttons (hero + final CTA) updated to `https://adoptionformsexpress.com/dfy-child-check-out-page/`; this doc's header URL line and Section 8 deployment URL updated to match; master Section 2 architecture row updated to match. Also: minor typography fix on `dfy-minor-child.html` — added `&nbsp;` between "business" and "days" in the "What Happens Next" H2 ("From order to inbox in 3 business days.") and step 2 H3 ("Our team prepares your forms (1–3 business days)") so "days" doesn't orphan onto its own line on narrow widths. | Claude / Tyler |
| 2026-05-01 | Sales page URL revised again. Tyler chose `/dfy-minor-sales-page/` as the sales-page WordPress slug (replacing `/buy-doneforyou-minor/`) for naming symmetry with the checkout page (`/dfy-child-check-out-page/`). URLs aligned: `dfy-minor-child.html` canonical updated (also caught and fixed a stale canonical that had been pointing to the original `/qualified/done-for-you-minor-child/` placeholder all along — it had missed the prior 2026-04-30 alignment); this doc's header URL line, Section 6 canonical example, and Section 8 deployment URL updated to match; master Section 2 architecture row + Decision #13 updated. **Tyler's WordPress side (not in this code update):** (1) update Typeform quiz redirect from `/buy-doneforyou-minor/` to `/dfy-minor-sales-page/`; (2) set 301 redirect in WordPress from old `/buy-doneforyou-minor/` to new `/dfy-minor-sales-page/` so any inbound links from the old URL don't 404. | Claude / Tyler |
| 2026-05-04 | v2.5 — Hero copy clarified to make the product identity unambiguous on the post-quiz landing. Section 4.2 (hero) eyebrow: "✓ You qualify" → "✓ You qualify for the DFY Minor Child Adoption Package". Section 4.2 H1: "You're a great fit for our Done-For-You package." → "You're a great fit for a Minor Child Done-For-You package." Both edits propagated to `dfy-minor-child.html`. Rationale: visitors arriving from the qualifier quiz now see the specific product they qualified for in both the eyebrow and H1, removing any ambiguity between minor-child and adult variants of the DFY package. No structural or schema changes. | Claude / Tyler |
| 2026-05-05 | v2.6 — ThriveCart embed token updated for this product after logo change in ThriveCart admin. Product ID unchanged; only the embeddable token regenerated. Old token: TOD8DE → new token: UAXWPD. | Claude / Tyler |
| 2026-05-05 | v2.7 — Mobile checkout layout fix in `dfy-minor-child-checkout.html`. Added a `@media (max-width: 720px)` block in the embedded `<style>` (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule) that tightens `.thrivecart-wrap` vertical padding and forces `min-height: 0` + `height: auto` on the injected ThriveCart iframe. Reason: on mobile the injected iframe was being given a desktop-sized fixed height, which left a large empty white gap between the form and the reassurance strip / two-up testimonials below it. No HTML or copy changes; CSS-only mobile fix. May need follow-up if ThriveCart's v2 embed turns out not to use an iframe (renders inline DOM instead) — in which case the iframe selector is a no-op and we'll need to target the actual injected container after inspecting it on the live page. | Claude / Tyler |
| 2026-05-05 | v2.8 — **Reverted v2.7's mobile fix** in `dfy-minor-child-checkout.html`. The `@media (max-width: 720px)` block was removed, restoring the file to its pre-v2.7 state. Reason: forcing `height: auto !important` on the injected ThriveCart iframe collapsed the form into the iframe's intrinsic default height (~150px), squishing the form fields to the point users couldn't comfortably enter their info. The original empty-space gap is back, but the form is usable. Next attempt deferred until Tyler can DevTools-inspect the live mobile checkout (Chrome mobile emulation, right-click the empty area → Inspect) and report the actual injected element's tag, class/id, and computed `height` — then we can target the real offender instead of guessing. | Claude / Tyler |
| 2026-05-05 | v2.9 — **Mobile empty-space fix v2 (correct version) in `dfy-minor-child-checkout.html`.** Tyler's DevTools inspection revealed the actual culprit: ThriveCart's embed script injects an `<iframe class="tc-v2-embeddable-el">` inside the `.tc-v2-embeddable-target` div and hardcodes an inline `style="height: 2387px"` on it. On mobile that's ~1000px taller than the form's actual rendered content, creating the empty-space gap below the visible form (the user is still scrolling inside the iframe through dead space until they exit it and reach our reassurance strip). The injected iframe also carries `scrolling="yes"`, which means we can safely cap its height with CSS — any overflow scrolls inside the iframe rather than being clipped. Fix: re-added the `@media (max-width: 720px)` block (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule) with `.thrivecart-wrap iframe.tc-v2-embeddable-el { max-height: 1800px !important; }` plus tightened wrap padding to `1.5rem 0`. The 1800px cap is conservative (form likely needs ~1300–1500px on mobile) — leaves a buffer for dynamic form expansion (coupon-code section, address validation errors, etc.) while still cutting most of the dead space. **Tuning:** if dead space is still visible after deploy, lower the cap (1500 → 1300); if a scrollbar appears inside the iframe because the form was clipped, raise it (2000+). Behavior change is mobile-only (≤720px); desktop unchanged. CSS-only; no HTML/copy/schema changes. | Claude / Tyler |
| 2026-05-05 | v2.10 — ThriveCart embed token regenerated again for product 10 after Tyler adjusted spacing in the ThriveCart admin (separate from the prior logo-change regen). Confirms the empirical pattern: ThriveCart mints a new embeddable token on most product saves, not just specific changes. Product ID unchanged. Old token: UAXWPD → new token: 1OP2TU. Token swapped in `dfy-minor-child-checkout.html` (lines 376–377) and across all token references in this spec doc via `replace_all`. Only this one product was edited in the admin this round, so the other three checkout files (DFY adult / DIY minor / DIY adult) are unaffected. | Claude / Tyler |
| | | |

---
*End of v1.0 — DFY Minor-Child Page Working Document*
