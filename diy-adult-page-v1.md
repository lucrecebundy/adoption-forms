# DIY Adult Stepparent Adoption — Post-Qualification Sales Page

**Document type:** Page-level working document
**Owner:** Lucrece H. Bundy / Tyler
**URLs:** `/diy-adult-sales-page/` (sales page — `diy-adult.html`); `/diy-adult-check-out-page/` (transactional checkout page — `diy-adult-checkout.html`). The two pages will be sibling top-level pages in WordPress, mirroring the established two-page architecture.
**Sister docs:**
- `diy-minor-child-page-v1.md` (the structural template — DIY minor child)
- `dfy-adult-page-v1.md` (the adult-content reference — DFY adult)
**Version:** 1.1
**Last updated:** May 1, 2026
**Status:** Built — `diy-adult.html` and `diy-adult-checkout.html` on disk; pending WordPress deploy

---

## How to Use This Document

This is the page-level working doc for the **DIY adult product** — the $299 self-serve forms package for qualifying Nebraska stepparent adoption cases involving an adult stepchild (19+).

**Two-page architecture:** this is the SALES page (`/diy-adult-sales-page/`) — it does the convincing. The CHECKOUT page (`/diy-adult-check-out-page/`) is a separate sibling top-level page that does the transaction with an embedded ThriveCart. Both CTA buttons on this sales page link to the checkout page. The full funnel is: Homepage → Qualifier Quiz → THIS sales page → `/diy-adult-check-out-page/` → ThriveCart processes payment.

Inherits all site-wide standards from the master doc (`website-redesign-master.md`).

This is the fourth and final product page being built. It draws from two sister docs:
- **Structural pattern** from `diy-minor-child-page-v1.md` (DIY framing, capability emphasis, "what if I get stuck" anxiety reduction)
- **Audience content** from `dfy-adult-page-v1.md` (adult-adoption qualification criteria, consent dynamics, name-change considerations, real-world deadline framing)

The DIY adult buyer is at the **intersection** of two narrow audiences: someone doing an adult adoption AND choosing to handle the paperwork themselves. The page must address both:
1. "Is adult adoption legitimate as a self-serve product?" (adult adoption legitimacy)
2. "Can I figure this out on my own?" (DIY capability)

---

## 1. Strategic Frame — What This Page Is And Isn't

### What this page IS

A **post-qualification sales page** for the DIY adult product. The visitor:

1. Found the site
2. Took the qualifier quiz
3. Was told they qualify for the DIY adult package
4. Was routed here by quiz logic (because their stepchild is 19+ AND they indicated comfort with paperwork or price sensitivity)

The page exists to make them feel **confident, capable, and ready** to click through to the checkout page and complete the $299 purchase.

### What this page IS NOT

- **Not an SEO page.** `<meta name="robots" content="noindex,nofollow">`. Not in the sitemap.
- **Not a checkout page.** ThriveCart embeds do NOT live on this page — they live on `/diy-adult-check-out-page/` (a separate sibling page). The two CTA buttons on this page link to that checkout page.
- **Not a comparison page.** No DIY-vs-DFY comparison table. The qualifier quiz routed this specific visitor to the DIY adult product; they're here to evaluate THIS product, not choose between products.
- **Not a hand-holding manual.** This is a sales page, not the actual instructions. The instructions are part of what they receive after purchase.
- **Not the SEO pillar.** A future, public-facing `/adult-stepparent-adoption-nebraska/` page will do the SEO work. That page funnels TO the qualifier quiz. This page is what's BEHIND the qualifier quiz.

---

## 2. The Visitor — Who Lands Here

A Nebraska resident who:

- Has decided to adopt their adult stepchild (19+)
- The stepchild has consented to the adoption
- Their spouse (the adoptee's biological parent) has consented
- Took the qualifier quiz and was routed to DIY (typically because they indicated price sensitivity, comfort with paperwork, or selected "show me both options" and is now evaluating DIY first)

### How this visitor differs from the DIY minor-child buyer

| | DIY Minor-Child Buyer | DIY Adult Buyer |
|---|---|---|
| Age of stepparent | Often 30s–40s | Often 50s–70s |
| Legal-system experience | May be first time in court | Often been through estates, divorces, name changes |
| Anxiety primary axis | "Will I do this right?" | "Is this legitimate? Am I doing this for the right reasons?" |
| Anxiety secondary axis | "What if my biological-parent consent gets contested?" | "Will this hold up legally? (estate / inheritance) " |
| Time pressure | Sometimes ("we want it done before kindergarten") | Often acute ("before the wedding," "before mom dies," "name on the headstone") |
| Emotional weight | Building a family | Honoring a relationship that already exists |
| Interest in the lawyer call | Backup for procedural questions | Validation that the legal foundation is sound |

### What they need from this page

- Confirmation they're in the right place
- Specific reassurance that adult stepparent adoption is a recognized, well-understood Nebraska legal process — and that the DIY product handles it correctly
- A clear, generous list of what's in the $299 package
- Address the primary anxiety: "Is this real for adults? Can I trust DIY for something with this much weight?"
- Address the secondary anxiety: "What if I get stuck?"
- A signal of attorney expertise (Lucrece's adult-adoption credibility)
- Quick, decisive CTA to the checkout

### What they do NOT need

- A hard sell
- A persuasive argument that adoption is meaningful (they already feel that)
- Detailed explanation of consent law (the qualifier quiz already vetted this)
- Comparison to the DFY product (they've already chosen DIY)

---

## 3. Page Structure (Top to Bottom)

```
1. Stripped checkout-style nav (logo + Email us)
2. Confirmation hero (eyebrow: "✓ You qualify" + H1 + qualification recap callout + primary CTA → checkout)
3. What You Get (forms + instructions + 1 attorney call — generous detail)
4. How It Works After You Order (4-step: download → review → fill out → file)
5. Trust Block (Lucrece signature block + 3 testimonials)
6. Pre-Purchase FAQ (DIY-adult-specific anxieties)
7. Final CTA (single, prominent — links to checkout)
8. Escape Hatch (small, discreet — for visitors who realize DIY isn't right; includes upgrade-to-DFY path)
9. Footer
```

This structure mirrors `diy-minor-child.html` exactly. Every section maps 1:1 in DOM order, CSS classes, and component patterns. Only the audience-specific copy differs.

---

## 4. Section-by-Section Copy

### 4.1 Sticky Nav

```
[Logo: Adoption Forms Express]                    Need help? Email us →
```

Same as DIY minor-child page — minimal nav, no menu items. Email link: `mailto:adoptionformsexpress@gmail.com`.

---

### 4.2 Hero — Confirmation + Primary CTA

**Eyebrow (success-green pill with checkmark):**
✓ YOU QUALIFY

**H1:**
Your DIY adult stepparent adoption package is ready to download.

**Subhead (one short paragraph):**
Based on your answers, your case meets the criteria for our DIY adult package. You'll get every Nebraska form you need, step-by-step instructions, and one attorney call when questions come up — all for $299.

**Qualification recap callout box (5 items):**

Eyebrow: WHAT YOU TOLD US
- ✓ Your stepchild is 19 or older
- ✓ Your stepchild consents to the adoption
- ✓ Your spouse (the adoptee's biological parent) consents
- ✓ The absent biological parent is deceased, consents to the adoption, or had their parental rights terminated before your stepchild turned 19
- ✓ You're a Nebraska resident

**Primary CTA button:**
Continue to Checkout — $299
*(button links to `/diy-adult-check-out-page/`)*

**CTA subtext (one line):**
Secure checkout · Forms delivered within 1 business day · Includes one attorney call

**Notes:**
- 5-item qualification recap. The absent-biological-parent bullet was added after Tyler's review of the v1.1 build — the adoptee's other biological parent must be deceased, have consented, or have had their rights terminated before the stepchild turned 19 for the case to qualify for DIY adult. Without this, the case is not a clean uncontested adult stepparent adoption and shouldn't have been routed to this product.
- "$299" appears in subhead and on the CTA — visitor sees price twice, removing surprise at checkout
- The CTA does NOT load ThriveCart on this page — clicking it routes the visitor to `/diy-adult-check-out-page/` where the ThriveCart embed lives
- The primary anxiety being defused here: "Is DIY adult adoption a real thing?" — the qualification recap and clean callout pattern signal "yes, this is exactly what your situation calls for"

---

### 4.3 What You Get

**Eyebrow:** WHAT'S INCLUDED

**H2:** Everything you need to finalize your adult stepparent adoption.

**Subhead (one line):**
Your $299 package includes forms, step-by-step instructions, and one attorney call.

**Two-column layout:**

**Column 1 — The Forms (you fill out, we provide)**
- Petition for Adult Adoption (Nebraska form)
- Consent forms (your spouse + the adult adoptee)
- Notice of Adoption
- Decree of Adoption (proposed)
- All other Nebraska-required supporting documents based on your specific situation

**Column 2 — The Guidance (so you can fill them out confidently)**
- Step-by-step written instructions for every form
- Filing instructions for your specific Nebraska county
- Background check authorization — you complete the checks yourself; we provide step-by-step guidance for what your county requires
- Court hearing prep document with the questions a Nebraska judge is most likely to ask in adult adoption cases
- One attorney call with Lucrece (30 minutes) — use it whenever you get stuck

**Below the columns, a small reassurance line:**
*All forms are prepared by Lucrece H. Bundy, Esq., a licensed Nebraska adoption attorney with 200+ adoption cases — including adult stepparent adoptions.*

**Notes:**
- Generous detail in this section is intentional — DIY buyers want to know EXACTLY what they're getting for $299. Vague "everything you need" copy creates anxiety.
- "Including adult stepparent adoptions" in the reassurance line is critical — adult adoption is rare enough that DIY adult buyers worry the attorney's experience is weighted toward minor-child cases. Surface the adult experience explicitly.
- The court hearing prep is a particularly strong asset for the DIY adult buyer — judges sometimes ask different questions in adult adoption cases (e.g., probing for inheritance/estate motives), and a prep document specifically tuned to adult cases reduces that anxiety.
- The "you complete the checks yourself" framing for background checks is the same pattern as DIY minor — it's accurate AND it sets the right DIY expectation.

---

### 4.4 What Happens Next After You Order

**Eyebrow:** HOW IT WORKS AFTER YOU ORDER

**H2:** From order to finalized adoption — at your pace.

**4-step horizontal timeline (DIY-tuned, mirroring DIY minor):**

**Step 1 — Order & confirmation email**
Right after checkout, we'll send a short email to confirm a few details about your case. Once you reply, we'll send all your forms and the instruction guide — typically within one business day.

**Step 2 — Review the instructions**
Read through the step-by-step guide. Most clients spend 30–60 minutes here just reviewing what's ahead — no decisions yet, just orientation.

**Step 3 — Fill out the forms**
Work through the forms at your own pace. The instructions tell you exactly what goes where. Most clients finish in 2–4 hours over a weekend.

**Step 4 — File and finalize**
Submit your forms to your Nebraska county court. Pay the filing fee. Attend the brief hearing. Most adult adoption cases finalize within 4–6 months from filing.

**Below the timeline, a small reassurance line:**
*Stuck somewhere? Use your attorney call. That's exactly what it's for.*

**Notes:**
- 4-step structure mirrors DIY minor-child for cross-page consistency
- Adult adoption has the same 4–6 month timeline as minor-child cases at the courthouse end (per `dfy-adult-page-v1.md` v1.8 timeline correction)
- Step 3 time estimate (2–4 hours over a weekend) is realistic for most cases — DIY buyers want a concrete time commitment so they can plan
- The "stuck somewhere?" line at the end is the second time the page surfaces the attorney call as a safety net — important because the DIY buyer's #1 anxiety is "what if I get stuck"
- Step 4 acknowledges the filing fee and hearing without making them feel scary or unexpected

---

### 4.5 Trust Block — Lucrece Signature + Testimonials

**Lucrece signature block (small circular photo + 4–6 line copy):**

Photo: Lucrece's professional headshot, circular crop
URL: `https://adoptionformsexpress.com/wp-content/uploads/2026/04/497A2015-scaled.jpg`

Copy:
> Hi, I'm **Lucrece H. Bundy**, a licensed Nebraska adoption attorney. I built the DIY package for the families I see most often: comfortable doing paperwork themselves, but wanting the security of attorney-prepared forms — and direct access to me when something specific to their adoption comes up.
>
> I've handled hundreds of Nebraska adoption cases, including adult stepparent adoptions where the adoptee is decades older than the stepparent. I know which forms get tripped up, which counties have idiosyncratic filing rules, and which questions the judges actually ask at the hearing. My job is to make sure your forms are correct, your filing path is clear, and you know exactly when to use the attorney call.

**Three review cards (Google-verified, curated for the DIY adult intersection):**

**Card 1 — Catrice Jackson** (adult-adoption authority — the only Google review explicitly mentioning adult adoption). Curated excerpt (~66 words) for visual balance with the other two cards; preserves the unique adult-adoption authority signal, the concrete "30 year old son" proof point, and one emotional beat:

> "She went above and beyond to help my family. She was extremely informative, knowledgeable about adult adoption, kind, very patient, and very professional. She really made me feel like I had nothing to worry about. With her amazing service, my husband was able to legally adopt my 30 year old son. There are no words to describe what this means to me as a mother."
> — **Catrice Jackson** (Aug 2022)

**Card 2 — Patty Bales** (cost-anxiety reducer — directly relevant for DIY price-conscious buyers):

> "We used Lucrece for an adoption. She was very professional, pleasant and great to work with. She was quick to respond to questions and everything was very smooth. I would highly recommend. She was an absolute delight to go though this process with. Of course price seems to always play a role and she is very reasonable with no hidden fees! Thanks for helping make this happen."
> — **Patty Bales** (Sep 2020)

**Card 3 — Ruby Leonard** (DIY product validation — only Google review explicitly mentioning DIY purchase):

> "She is super friendly and knowledgeable. She helped us understand and know every case scenario possible. Thank you! We ended up purchasing the DIY Adoption documents for step-parent adoption and it was so easy to do and understand. When I had questions she would answer my emails promptly. She is very professional and very helpful. We are just waiting for the final court date. Thank you so much for having this available."
> — **Ruby Leonard** (Local Guide, edited 2024)

**Notes:**
- **Three different anxiety axes covered:** Catrice = "is adult adoption legitimate?", Patty = "what about price/transparency?", Ruby = "can I actually figure DIY out?"
- This is the most layered testimonial trio on any page in the project. The DIY adult page has the most narrow audience — needs proof from each angle.
- Catrice is in slot 1 because the adult-adoption authority is the foundation. If they don't believe adult adoption is "a real thing," nothing else matters.
- Patty is in slot 2 because price transparency is the next biggest concern — DIY buyers chose this product partly because of price; the testimonial validates the choice.
- Ruby is in slot 3 because DIY product validation closes the deal: "yes, real customers actually used the DIY package successfully."
- The Lucrece signature copy is a hybrid of the DIY minor-child language ("comfortable doing paperwork themselves...security of attorney-prepared forms") AND the DFY adult language ("including adult stepparent adoptions where the adoptee is decades older than the stepparent"). Both reassurances matter for this audience.

---

### 4.6 Pre-Purchase FAQ

5 questions, accordion format. Adult-DIY-specific anxieties.

**Eyebrow:** QUESTIONS BEFORE YOU BUY

**H2:** What people ask before clicking through to checkout.

**Q1: What if I get stuck on a form?**
Two places to turn. First, the step-by-step instructions cover every section of every form in plain English. Second, you have one attorney call with Lucrece — most clients use it about halfway through, after they've reviewed everything but before they file. Between the two, most DIY adult adoption cases finish without needing more.

**Q2: Do biological parents need to consent to an adult adoption in Nebraska?**
Yes — written consent is required from the adoptee's biological parent (typically your spouse) and from the adult adoptee themselves. Both consent forms are filed with the petition. The DIY package includes both consent forms with step-by-step instructions for completion. The absent biological parent's consent is not required for adult stepparent adoption in Nebraska — that's one of the reasons this case type qualifies for DIY.

**Q3: How long does the whole process take?**
From the day you file until the adoption is finalized: typically 4–6 months. The variability depends on your county's court calendar, not on the forms. The DIY package includes filing instructions for your specific county so the actual filing day is straightforward.

**Q4: Can the adult adoptee change their last name as part of the adoption?**
Yes — name change is one of the most common reasons adults pursue stepparent adoption. The DIY package's Petition for Adult Adoption includes the optional name-change request, and the Decree of Adoption (proposed) reflects the new name. Tell us in the post-checkout intake email if name change is part of your case and we'll make sure the right field is highlighted in your forms.

**Q5: What if I live in Nebraska but the adoptee lives somewhere else?**
The petition is filed in the Nebraska county where you live, and the court hearing happens there in person. If the adoptee lives out of state, they'll need to travel to Nebraska for the hearing.

**Notes:**
- Q1 mirrors the DIY minor-child Q1 pattern — the natural anxiety question gets a confidence-building answer ("most cases finish without needing more"). No "email us" escape hatch and no upgrade-to-DFY-credit mention; the page is built to do the convincing work itself, not to invite people to bypass it with email questions.
- Q2 mirrors the DFY adult page Q1 (same correction applied — biological parents DO need to consent), adapted for DIY framing
- Q3 timeline corrected to 4–6 months per DFY adult v1.8 timeline correction
- Q4 surfaces the name-change use case which is often the trigger for adult adoption — and tells the visitor that the package handles it
- Q5 gives the essence of the rule without getting into the weeds: petition filed where the petitioner lives in Nebraska; in-person hearing in that county; out-of-state adoptee travels to Nebraska. The military-deployment exception, the "everyone must appear" detail, and the package-instructions reference are intentionally omitted to keep the answer tight. Earlier drafts suggested remote appearance "depending on the judge" — that was wrong; corrected per Lucrece's guidance.
- 5 questions matches the DFY adult and DIY minor pattern — enough to cover the main anxieties without overwhelming

---

### 4.7 Final CTA

**H2:** Ready to make it official?

**Below H2 (one line):**
Your DIY adult adoption package, prepared by a licensed Nebraska adoption attorney, in your inbox tomorrow.

**Primary CTA button:**
Continue to Checkout — $299
*(button links to `/diy-adult-check-out-page/`)*

**Below the CTA, small reassurance line:**
*Secure checkout · 7-day refund if your case isn't a fit*

**Notes:**
- "Make it official" intentionally echoes the DFY adult page H2 — same emotional anchor for adult-adoption visitors
- "In your inbox tomorrow" is concrete, time-specific, lower-anxiety than "within 1 business day" (same content, more emotional)
- Same `/diy-adult-check-out-page/` destination as the hero CTA — ThriveCart loads on the checkout page, not here
- Same 7-day refund promise as all other product pages

---

### 4.8 Escape Hatch

A small, discreet section for visitors realizing DIY isn't right for them.

**H3:** Not sure DIY is right for your situation?

**Copy:**
Adult adoption sometimes has wrinkles that don't fit a self-serve product — for example, the adoptee lives out of state, the biological parent's consent is contested, or you're navigating an estate-planning deadline. If any of that sounds familiar, the Done-For-You package handles everything for $499 — same forms, but we complete and file them for you. Or, if your situation is really complex, [Bundy Law LLC](https://lbundylaw.com/) handles adoption cases that need full attorney representation.

> If you'd rather have us complete the forms for you, our [Done-For-You package](/dfy-adult-sales-page/) is $499 and we deliver completed forms within 3 business days.

**Notes:**
- Surfaces the upgrade-to-DFY path explicitly — same pattern as DIY minor-child escape hatch
- The wrinkles listed (out-of-state, contested consent, estate deadlines) are the most common reasons an adult-adoption DIY visitor might realize this isn't quite right for them
- Bundy Law LLC link gives the highest-complexity escape valve
- The link to DFY adult is intentional — it's a sister product, and a visitor who's already decided "I want this handled professionally" is a perfect upsell to DFY
- No "email us" line — visitors who don't fit DIY should self-route to DFY or Bundy Law via the existing links. The page is designed to do the convincing work itself, not to invite visitors to email instead of reading.

---

### 4.9 Footer

Inherited verbatim from `diy-minor-child.html`. Same UPL disclaimer, same social links, same footer structure. No DIY-vs-DFY product distinction in the footer — just the standard navigation.

---

## 5. Visual System

Inherits all design tokens from the homepage and other product pages. No custom styling for this page. Specifically:

- Fonts: Fraunces (display), Manrope (body)
- Colors: navy primary, coral accent, cream background, success green
- Spacing: same `--max-width: 1240px` and consistent rhythm tokens
- Components: same hero callout, same two-column "What's Included," same 4-step timeline, same FAQ accordion, same final-CTA panel, same footer

The DIY adult page should be visually indistinguishable from the DIY minor-child page in style — only audience-specific copy differs.

---

## 6. SEO & Indexing

- `<meta name="robots" content="noindex,nofollow">` — gated post-quiz page must not be indexed
- Canonical: `https://adoptionformsexpress.com/diy-adult-sales-page/`
- Excluded from sitemap (set in WordPress SEO plugin)
- No internal links from indexed pages — only entrypoint is qualifier quiz redirect
- No FAQPage schema — same reasoning as other gated pages (must not surface in search)

---

## 7. Schema Markup

Single JSON-LD `Product` block (no `FAQPage`, no `AggregateRating`):

```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "DIY Nebraska Adult Stepparent Adoption Forms",
  "description": "Self-serve Nebraska adult stepparent adoption forms package (for stepchildren age 19+). Attorney-prepared forms with step-by-step instructions and one attorney call. Prepared by a licensed Nebraska adoption attorney.",
  "brand": { "@type": "Brand", "name": "Adoption Forms Express" },
  "offers": {
    "@type": "Offer",
    "price": "299",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock"
  }
}
```

---

## 8. Technical Implementation Notes

- Page is built as a single self-contained HTML file in the same style as `diy-minor-child.html`
- Same design tokens, typography, button styles, FAQ accordion logic
- File name: `diy-adult.html`
- Deployed to URL: `/diy-adult-sales-page/`
- WordPress: created as a new top-level page (Blank Slate template), with a Custom HTML block holding the body content
- WordPress page settings: set to "noindex" via SEO plugin — belt-and-suspenders alongside the meta tag
- Removed from primary nav menu
- Both CTA buttons (hero + final) link to `/diy-adult-check-out-page/` (a separate sibling top-level WordPress page)

### ThriveCart Integration

This page does NOT contain the ThriveCart embed. ThriveCart lives on the separate checkout page at `/diy-adult-check-out-page/`. The CTAs on this sales page link to that checkout page.

For the **checkout page** (`diy-adult-checkout.html`), use the production ThriveCart embed snippet for the DIY adult product:

```html
<div class="tc-v2-embeddable-target" data-thrivecart-account="adoptionssimplified" data-thrivecart-tpl="v2" data-thrivecart-product="7" data-thrivecart-embeddable="tc-adoptionssimplified-7-A4PSQA"></div>
<script async src="//tinder.thrivecart.com/embed/v2/thrivecart.js" id="tc-adoptionssimplified-7-A4PSQA"></script>
```

ThriveCart product ID: 7
Embeddable token: `tc-adoptionssimplified-7-A4PSQA`

---

## 9. Open Questions / Decisions Needed

| # | Question | Status | Notes |
|---|---|---|---|
| 1 | DIY adult sales-page testimonials | ✅ Resolved 2026-05-01 | Locked: Catrice Jackson (slot 1 — adult-adoption authority), Patty Bales (slot 2 — cost transparency), Ruby Leonard (slot 3 — DIY product validation). Three different anxiety axes; most-layered trio in the project. |
| 2 | DIY adult checkout testimonials | ✅ Resolved 2026-05-01 | Locked: Ruby Leonard (curated short excerpt — DIY product validation) + Patty Bales (cost transparency) — same pair as DIY minor checkout, since they address the DIY-buyer payment moment best. |
| 3 | DIY-to-DFY upgrade credit mechanism (adult) | Open | FAQ Q1 promises "we credit your $299 toward the $499 package" — same mechanism as DIY minor-child. Confirm operationally feasible in ThriveCart and Bundy Law's system. May need a manual process initially. |
| 4 | Post-checkout intake email content | Open | After ThriveCart purchase, the team sends a short email to confirm case details. Same pattern as DIY minor-child. Consider whether DIY adult needs different intake fields (e.g., name-change confirmation, adoptee's geographic location) than DIY minor.  |

---

## 10. Change Log

| Date | Change | Author |
|---|---|---|
| 2026-05-01 | v1.1 — Both DIY adult HTML files built. `diy-adult.html` (sales page) mirrors `diy-minor-child.html` structurally; DIY-adult-specific copy from spec (adult-aware signature block, FAQ with name-change use case, escape hatch acknowledging adult-specific wrinkles, testimonials Catrice/Patty/Ruby). `diy-adult-checkout.html` mirrors `diy-minor-child-checkout.html` structurally; ThriveCart product 7 embedded; testimonials Ruby Leonard (curated excerpt) + Patty Bales (same pair as DIY minor checkout). Both pages are noindex, no FAQPage schema. Both CTAs on the sales page link to `/diy-adult-check-out-page/`. **Mid-build copy correction:** qualification recap originally drafted as 4 items expanded to 5 — added the absent-biological-parent bullet ("deceased, consents to the adoption, or had their parental rights terminated before your stepchild turned 19") after Tyler caught that this is a real DIY-qualifying gate, not a missing-by-design simplification. Section 4.2 of this spec updated to match. The DIY adult funnel is feature-complete locally — pending WordPress deploy. The full four-product, eight-page conversion funnel is now feature-complete. | Claude / Tyler |
| 2026-05-01 | v1.0 — Initial DIY adult sales page spec drafted. Modeled on `diy-minor-child-page-v1.md` (DIY structural patterns) with adult-content adaptations from `dfy-adult-page-v1.md` (qualification recap, consent dynamics, name-change FAQ, timeline, "make it official" framing). Key DIY-adult specifics: 4-item qualification recap (vs 5 for DIY minor due to fewer adult-adoption qualifying criteria), explicit "knowledgeable about adult adoption" reassurance in signature block, court hearing prep doc emphasizes adult-specific judge questions, FAQ leads with "what if I get stuck?" anxiety + Q4 surfaces name-change use case, escape hatch acknowledges adult-specific wrinkles (out-of-state adoptee, estate deadlines). Three-card testimonial trio is the most layered in the project: Catrice (adult-adoption authority), Patty (cost transparency), Ruby (DIY product validation). ThriveCart product 7 (token tc-adoptionssimplified-7-A4PSQA) confirmed as DIY adult product — embed lives on the checkout page, not this sales page. | Claude / Tyler |
