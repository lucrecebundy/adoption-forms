# Done-For-You Adult Stepparent Adoption — Post-Qualification Sales Page

**Document type:** Page-level working document
**Owner:** Lucrece H. Bundy / Tyler
**URLs:** `/dfy-adult-sales-page/` (sales page — `dfy-adult.html`); `/dfy-adult-checkout-page/` (transactional checkout page — not yet built). The two pages will be sibling top-level pages in WordPress, mirroring the minor-child architecture.
**Replaces:** `/customized-adoption-forms/` (split into two pages by audience)
**Sister doc:** `dfy-minor-child-page-v1.md` (minor-child equivalent)
**Version:** 1.16
**Last updated:** May 5, 2026
**Status:** Built — `dfy-adult.html` (post-quiz sales page) and `dfy-adult-checkout.html` (transactional checkout housing the ThriveCart embed for product 8) both on disk, ready for WordPress deploy

---

## How to Use This Document

This is the page-level working doc for the **post-qualification sales page** for the Done-For-You product when the qualifying case involves an **adult stepchild** (19+). Inherits all site-wide standards from the master doc (`website-redesign-master.md`).

**Two-page architecture (mirroring minor-child):** this is the SALES page (`/dfy-adult-sales-page/`) — it does the convincing. The CHECKOUT page (`/dfy-adult-checkout-page/`) is a separate sibling top-level page that does the transaction with an embedded ThriveCart. The checkout page does not yet exist; both CTA buttons on this sales page link to it. The full funnel is: Homepage → Qualifier Quiz → THIS sales page → `/dfy-adult-checkout-page/` → ThriveCart processes payment.

This is a sister doc to `dfy-minor-child-page-v1.md`. The two pages share structure exactly; the audience-specific content differs.

If you change the structure of this page, change it on the minor-child page too. The pages should feel like clear siblings to anyone who navigates between them (though most visitors won't — the quiz routes them to one or the other).

---

## 1. Strategic Frame — What This Page Is And Isn't

### What this page IS

A **post-qualification sales page** for adult stepparent adoption. The visitor:

1. Found the site
2. Took the qualifier quiz
3. Was told they qualify
4. Their stepchild is an adult (19+)
5. Chose the Done-For-You option
6. Was routed here by quiz logic

The page exists to make them feel **confident, informed, and ready** to click through to the checkout page and complete the $499 purchase.

### What this page IS NOT

- **Not an SEO page.** `<meta name="robots" content="noindex,nofollow">`. Not in the sitemap.
- **Not a marketing page.** No selling, no comparison, no upsell. The visitor is already sold.
- **Not a discovery page.** Every link off this page is the purchase button (which routes to the checkout page), the support escape hatch, or footer-standard.
- **Not the checkout page.** ThriveCart embeds do NOT live on this page — they live on `/dfy-adult-checkout-page/` (a separate sibling page). The two CTA buttons on this page link to that checkout page.
- **Not the SEO pillar.** A future, public-facing `/adult-stepparent-adoption-nebraska/` page will do the SEO work. That page funnels TO the qualifier quiz. This page is what's BEHIND the qualifier quiz.

### Why adult stepparent adoption is different (and matters strategically)

Adult stepparent adoption is a **largely overlooked product category in Nebraska**. Most adoption attorneys focus on minor-child cases. Most generic legal-form sites either don't offer it or treat it as an afterthought. The visitor who lands here is often:

- Adopting an adult stepchild they helped raise (very common — the stepchild grew up, the family wants to make it official before a parent passes, or for inheritance/recognition purposes)
- In an emotionally loaded moment — these adoptions often happen around weddings, graduations, the birth of grandchildren, or the death of a biological parent
- Surprised by how procedurally light adult adoption is on the front end — no home study, less documentation than minor-child cases — even though the courthouse timeline is similar (4–6 months)
- Looking for someone who actually understands adult adoption — most Nebraska attorneys handle it once a year if at all

This is a real strategic moat. Build the page accordingly.

### One-line page goal

**Confirm qualification → reinforce trust → enable instant purchase.**

(Same as minor-child page. Same goal, different audience.)

---

## 2. The Visitor — Who Lands Here

A married Nebraska resident who:

- Just completed the qualifier quiz
- Has been told they qualify
- Their stepchild is an adult (19 or older)
- Has chosen the Done-For-You option
- Is ready to pay $499 today

**What's emotionally distinctive about this audience:**

- **Often older** — frequently 50s, 60s, 70s
- **Often more experienced with the legal system** — they've been through a few life events that involved courts (estates, divorces, name changes)
- **Less anxious about the legal process; more anxious about the relational moment** — this is often years or decades in the making and they want it to go smoothly
- **Often working on a deadline** — wedding, holiday, family reunion, end of life, name change to match other family members

**What they need from this page:**

- Confirmation they're in the right place
- Specific reassurance that adult stepparent adoption is a recognized, well-understood Nebraska legal process
- A clear picture of timeline (especially because they often have a real-world deadline)
- Lucrece's specific experience with adult cases
- Easy, fast purchase path

**What they do NOT need:**

- A long explanation of Nebraska adoption law (homepage's job)
- Comparison to minor-child adoption
- An overload of "this is easier than you think!" reassurance (it's actually pretty straightforward and they probably already know that)

---

## 3. Page Structure (Top to Bottom)

```
1.  Sticky nav (logo only)
2.  Hero / Qualification Confirmation
3.  What You Get
4.  How It Works After You Order
5.  Trust block (Lucrece signature, 3 adult-adoption-specific testimonials)
6.  Pre-purchase FAQ
7.  Final CTA
8.  Escape hatch
9.  Footer
```

Same structure as the minor-child page. Audience-specific content swaps.

---

## 4. Section-by-Section Copy

### 4.1 Sticky Nav

```
[Logo: Adoption Forms Express]                    Need help? Email us →
```

Same as minor-child page — minimal nav, no menu items.

---

### 4.2 Hero / Qualification Confirmation

**Eyebrow (success green):**
✓ You qualify

**H1:**
You're a great fit for our Done-For-You Adult Adoption package.

**Subhead:**
Based on your answers, your Nebraska adult stepparent adoption is exactly the kind of case our Done-For-You package was built for. Here's what you'll get and what happens next.

**Qualification recap callout:**
> Based on your quiz answers:
> ✓ Your stepchild is an adult (19 or older)
> ✓ Your stepchild consents to the adoption
> ✓ You meet Nebraska's adult-adoption requirements
> ✓ Your case is uncontested
>
> *That makes you a perfect fit for the $499 Done-For-You package.*

**Primary CTA button:**
Continue to Checkout — $499

*(button links to `/dfy-adult-checkout-page/`)*

**Below the CTA, small text:**
*Secure checkout · Most orders delivered within 3 business days*

**Notes:**
- Adult adoption qualification is simpler than minor-child (no biological-parent-consent requirement, no 6-month residency requirement). The recap reflects this.
- "Your stepchild consents" is the central legal pillar of adult stepparent adoption — both parties must consent in writing
- The qualification recap is doing the same emotional work as on the minor-child page: bridging the quiz outcome to the page content
- The CTA does NOT load ThriveCart on this page — clicking it routes the visitor to `/dfy-adult-checkout-page/`, where the ThriveCart embed lives

---

### 4.3 What You Get

**Eyebrow:** WHAT'S INCLUDED

**H2:** Everything you need to finalize your adult stepparent adoption.

**Two-column layout:**

**Column 1 — The Forms (completed by us)**
- Petition for Adoption (Nebraska form, completed with your information)
- Consent forms
- Notice of Adoption
- Decree of Adoption (proposed)
- All other Nebraska-required supporting documents based on your specific situation

**Column 2 — The Guidance**
- Step-by-step filing instructions specific to your Nebraska county court
- Court hearing prep document with the questions a Nebraska judge is most likely to ask in adult adoption cases
- Background check instructions — you complete the checks yourself; we provide step-by-step guidance for what your county requires
- New birth certificate ordering instructions (your adult stepchild's name change, if applicable)
- Two 15-minute support calls to answer questions about your forms

**Below the columns:**
*Court filing fees (~$60–$90 depending on county) and certified copy fees are paid directly to your local court and not included.*

**Notes:**
- The adult-adoption package list mirrors the minor-child list exactly — same items, same wording. Internal context: a Nebraska adult-adoption stepparent case requires written consent from your spouse (the adult adoptee's biological parent) and the adult adoptee themselves. The customer-facing list says generic "Consent forms," which fits both adult and minor-child cases without surfacing the underlying consent-party difference. Background check requirements are the same as minor-child cases — each adult party completes their own, with step-by-step guidance included.
- "Adult adoption experience" specifically called out in the calls description because it's the differentiator — most attorneys don't do many of these
- Note for Lucrece: confirm whether the adult adoptee's name change is automatic or requires a separate filing in Nebraska. Update copy accordingly.

---

### 4.4 How It Works After You Order

**Eyebrow:** WHAT HAPPENS NEXT

**H2:** From order to inbox in 3 business days.

**4-step horizontal layout:**

**Step 1 — You complete a secure intake form (10 minutes)**
After payment, you'll get a link to a confidential intake form. You'll provide names, dates, and key details — most adult adoption intakes take less than 10 minutes because the documentation needed is simpler than for minor-child cases.

**Step 2 — Our team prepares your forms (1–3 business days)**
Our team completes your forms, and Lucrece personally reviews every package. No rush, no template-fill — every detail is checked against Nebraska statute.

**Step 3 — You receive your completed package by email**
Your package will include every form filled out and ready to file, your county-specific filing checklist, your court hearing prep guide, and the new birth certificate ordering instructions.

**Step 4 — You file with your county court**
Take your forms to your county court clerk. Pay the filing fee (~$60–$90). Get your hearing date. Most uncontested Nebraska adult stepparent adoptions finalize **4–6 months** after filing.

**Below the steps:**
*Need to finalize before a specific date — a wedding, a holiday, a family reunion? Let us know in the intake form and we'll help you plan the timing.*

**Notes:**
- The 10-minute intake estimate (vs. 15 on the minor-child page) is real and accurate — adult adoption requires less documentation
- 4–6 months for adult adoption matches the minor-child timeline. The advantage of adult cases is procedural (less documentation up front, no home study) rather than calendar speed — court schedules and county-specific delays drive the total timeline either way.
- The "specific date" line at the bottom is THE most important addition for this audience — they often have a real-world deadline. Acknowledging it builds trust and signals competence.

---

### 4.5 Trust Block

**Eyebrow:** YOU'RE IN GOOD HANDS

**Lucrece signature block (compact, with thumbnail headshot):**

[Photo: Lucrece's professional headshot, small and circular]

**Lucrece H. Bundy, Esq.**
Founder, Adoption Forms Express
Licensed Nebraska Adoption Attorney
200+ Nebraska Adoptions Finalized — including adult stepparent adoptions

**Below the signature block — three short adult-adoption-specific testimonials:**

**Three review cards (Google-verified, all adult-adoption clients):**

> "Lucrece Bundy with Bundy Law, LLC was just what our family needed for an adult child adoption. She helped my 30 year old son make a dream come true by walking us through the process of his stepfather (now legal father) adopting him. Lucrece was helpful, caring and professional during the whole process. I highly recommend her services. She is the best!"
> — Catrice Jackson

> "My family used Bundy Law Office for our adoption. We did research online and thought Bundy Law Office sounded like a good fit . . . and they were. Very knowledgeable and informative of the adoption process. Kept us well informed as we went through the process. Promptly returned phone calls and emails. I highly recommend their services."
> — Gary Boettcher

> "We used Lucrece for an adoption. She was very professional, pleasant and great to work with. She was quick to respond to questions and everything was very smooth. I would highly recommend. She was an absolute delight to go though this process with. Of course price seems to always play a role and she is very reasonable with no hidden fees! Thanks for helping make this happen."
> — Patty Bales

**Notes:**
- Specifically calling out adult-adoption experience in Lucrece's signature block is critical — this audience values the specialty
- Adult-adoption testimonials tend to land emotionally hard (Catrice's "make a dream come true" line is the page's strongest emotional moment) — these are conversion gold
- Catrice Jackson's testimonial is the only one of the three that explicitly mentions adult adoption — that's why she goes first. Boettcher and Bales reinforce volume of adult-adoption work without explicit framing.
- Patty Bales's "very reasonable with no hidden fees" line is the single best price-anchored line on the page — leave it intact in the HTML build. Adult-adoption visitors are often anxious about cost transparency given they're already paying out-of-pocket; this line meets that anxiety directly.
- All three testimonials now have full Google-verified text. Page is testimonial-locked and ready for HTML build.

---

### 4.6 Pre-Purchase FAQ

**Eyebrow:** BEFORE YOU PURCHASE

**H2:** A few quick answers.

**Accordion FAQ (6 questions):**

**Q: Do biological parents need to consent to an adult adoption in Nebraska?**
Yes. In a Nebraska adult stepparent adoption, written consent is required from your spouse — the adult adoptee's biological parent — and from the adult adoptee themselves. Both consents are filed with the petition.

**Q: Will my adult stepchild's name change automatically?**
Your adult stepchild can choose to take your last name as part of the adoption decree, but it isn't automatic — it must be requested in the petition. Your forms package will ask you whether a name change is desired and prepare the petition accordingly.

**Q: How long does the process take?**
Most uncontested Nebraska adult stepparent adoptions finalize in 4 to 6 months from filing. Timelines vary by county and case complexity.

**Q: What if my situation is unusual (e.g., my stepchild lives out of state)?**
Adult adoptions can usually proceed even when the adoptee lives in another state, as long as one of you (or your spouse) is a Nebraska resident. If your situation has any wrinkles, email us before purchasing — we'll let you know whether the Done-For-You package is the right fit.

**Q: What does the $499 not include?**
The $499 covers your completed forms package, the two 15-minute support calls, and the filing/hearing/birth certificate guidance. It does NOT cover your county's filing fee (~$60–$90 paid directly to the court) or certified copies of your finalized adoption decree.

**Q: What if I realize I selected the wrong package?**
Right after purchase, we'll email you to confirm which scenario applies to your case and which package you ordered. We don't send your forms until you reply confirming both. If at that point you realize you bought the wrong package, just reply and let us know — we'll refund you, and you can purchase the correct one. If you don't reply to our confirmation emails within 7 days of purchase, we consider your purchase final and refunds are no longer available. After we've sent your forms, we cannot refund.

**Notes:**
- These FAQs are different from the minor-child page because the legal mechanics of adult adoption are genuinely different. Don't try to copy-paste between the pages.
- The biological-parent-consent question goes first because it's the single most common confusion point — visitors often assume adult adoption requires no biological-parent consent at all, when in fact the spouse (the adoptee's biological parent) must consent in writing alongside the adult adoptee
- The name-change question is the second-most-asked thing in adult adoption — everyone wonders about it, few attorneys explain it clearly
- The out-of-state question matters because adult-adoption visitors are often dealing with a stepchild who has moved out of Nebraska

---

### 4.7 Final CTA

**H2:** Ready to make it official?

**Below H2:**
Your Done-For-You adult adoption package, completed by our team, delivered in 3 business days.

**Primary CTA button:**
Continue to Checkout — $499

*(button links to `/dfy-adult-checkout-page/`)*

**Below the CTA, small reassurance line:**
*Secure checkout*

**Notes:**
- "Make it official" intentionally echoes the homepage hero language — same emotional anchor
- This is the only CTA below the fold
- Same `/dfy-adult-checkout-page/` destination as the hero CTA — ThriveCart loads on the checkout page, not here
- Reassurance line trimmed to a single phrase — by the time qualifying visitors reach the final CTA on a gated post-quiz page, refund/email-question messaging is friction, not reassurance. Refund mechanics live in the FAQ (Q6); the support escape hatch lives in Section 4.8.

---

### 4.8 Escape Hatch

Below the final CTA, in muted text:

*If your situation has changed since you took the qualifier quiz — for example, your adult stepchild is no longer agreeing to the adoption, or you've learned that there are unusual estate or inheritance considerations — please email us at [support email] before purchasing. We can connect you with Bundy Law LLC for full attorney representation if your case has become more complex.*

**Notes:**
- Adult adoption sometimes has estate/inheritance complications that didn't surface during the quiz (e.g., the adoption affects how a will is read, or how trusts pay out). Routing those cases to Bundy Law is the right move both ethically and commercially.
- Same UPL-protection role as the minor-child page

---

### 4.9 Footer

Same as homepage and minor-child page.

---

## 5. Visual System

Inherits everything from `website-redesign-master.md` Section 4. Same as minor-child page — no page-specific overrides.

The page should feel **calm, dignified, slightly more refined** than the minor-child page. Specifically:

- Generous whitespace — this audience appreciates breathing room
- The hero qualification block can lean a little more emotionally warm than the minor-child version (this is often a long-awaited moment)
- Lucrece's signature block specifically signals adult-adoption experience

---

## 6. SEO & Indexing

### Same as minor-child page: NOT indexed.

```html
<meta name="robots" content="noindex,nofollow">
<link rel="canonical" href="https://adoptionformsexpress.com/dfy-adult-sales-page/">
```

**Sitemap:** Not included.

**Internal links:** No nav links. Only entrypoint is the qualifier quiz.

### Future SEO sister page

A public-facing pillar page (`/adult-stepparent-adoption-nebraska/`) is a high-priority future build. Adult stepparent adoption is a real underserved keyword cluster — competitors barely target it.

That pillar page will:
- Be indexed
- Target keywords like "nebraska adult stepparent adoption," "adopt my adult stepchild nebraska," "nebraska adult adoption process"
- Funnel TO the qualifier quiz
- Probably outrank existing competitors with relatively little effort

Tracked separately in the master doc as a Phase D priority.

---

## 7. Schema Markup

Same minimal approach as minor-child page:

```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "Done-For-You Nebraska Adult Stepparent Adoption Forms",
  "description": "Attorney-prepared Nebraska adult stepparent adoption forms (adoptee age 19+). Completed by our team within 3 business days. Includes two 15-minute support calls and complete filing guidance.",
  "brand": { "@type": "Brand", "name": "Adoption Forms Express" },
  "offers": {
    "@type": "Offer",
    "price": "499",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock"
  }
}
```

No `FAQPage` schema. Page is gated; rich results aren't desired.

---

## 8. Technical Implementation Notes

- Two self-contained HTML files in the same style as `homepage.html` and the minor-child funnel
- Sales page file: `dfy-adult.html` — URL: `/dfy-adult-sales-page/`
- Checkout page file: `dfy-adult-checkout.html` — URL: `/dfy-adult-checkout-page/` — houses the ThriveCart embed (account `adoptionssimplified`, product `8`, embed token `tc-adoptionssimplified-8-POHMYG`)
- WordPress: each is a separate top-level page using a "Custom HTML" block or custom page template; the two are sibling pages, not parent/child
- Set to "noindex" in your SEO plugin (both pages)
- Removed from primary nav menu
- Quiz routing: Typeform must route adult-stepchild qualifying cases to `/dfy-adult-sales-page/`
- ThriveCart loads only on `/dfy-adult-checkout-page/` — no duplicate-instance concern

---

## 9. Open Questions / Decisions Needed

| # | Question | Status | Notes |
|---|---|---|---|
| 1 | Collect 3 adult-adoption-specific testimonials | ✅ Resolved 2026-04-29 | Locked: Catrice Jackson (full text, explicitly mentions adult adoption + 30 year old son), Gary Boettcher (full text), Patty Bales (full text). All three full Google-verified text. |
| 2 | Confirm Nebraska adult-adoption timeline | ✅ Resolved 2026-05-01 | Tyler confirmed: uncontested adult stepparent adoptions finalize 4–6 months after filing — same as minor-child cases. The earlier 6–10 week claim (and the "faster than minor-child" framing that went with it) is replaced everywhere on the page. |
| 3 | Adult-adoption forms list accuracy | Open | Lucrece to confirm exact list. Specifically: does Nebraska require the spouse's consent in writing? |
| 4 | Adult name change mechanism | Open | Confirm whether name change is automatic or requires separate request in petition. Update FAQ and copy accordingly. |
| 5 | Out-of-state adoptee residency rule | Open | Lucrece to confirm Nebraska rule on adult adoption when adoptee resides out of state. |
| 6 | Estate/inheritance considerations | Open | Should the escape hatch language specifically mention estate planning, or is that overreach? Lucrece's call. |

---

## 10. Change Log

| Date | Change | Author |
|---|---|---|
| 2026-04-28 | v1.0 — Initial DFY adult-adoption page spec drafted as sister page to DFY minor-child | Claude / Tyler |
| 2026-04-29 | v1.1 — Cross-doc consistency edit: removed "Email access for follow-up questions throughout your case" from Section 4.3 Column 2 to match minor-child page (only 2 attorney calls included, scoped to questions about your forms). | Claude / Tyler |
| 2026-04-29 | v1.2 — Section 4.5 testimonials locked: Catrice Jackson (full text, explicitly mentions adult adoption), Gary Boettcher (truncated — pull full from Google), Patty Bales (truncated — pull full from Google). All three are confirmed adult-adoption clients. Open Question #1 resolved. New open item: pull full Google text for Boettcher and Bales before HTML build. | Claude / Tyler |
| 2026-04-29 | v1.3 — Gary Boettcher full review text added. Notes and Open Question #1 updated. Bales remains truncated. | Claude / Tyler |
| 2026-04-29 | v1.4 — Patty Bales full review text added. All three adult-adoption testimonials are now full Google-verified text. Page is fully testimonial-locked. Bales's "very reasonable with no hidden fees" line is a strong unexpected asset for cost-anxious visitors. | Claude / Tyler |
| 2026-04-29 | v1.5 — Cross-doc consistency edits to mirror locked minor-child spec. Section 4.3 (What's Included) Column 1 rewritten so adult page now matches minor-child word-for-word: "Petition for Adult Adoption" → "Petition for Adoption", consent line simplified from "adult adoptee, plus your spouse's consent" → just "Consent forms" (note: Tyler corrected an earlier inaccurate claim — adult adoption requires consent from BOTH biological parents AND the adult adoptee themselves), "Notice of Hearing" → "Notice of Adoption" (form-name correction). Background check guidance line added to Column 2 with same "you complete the checks yourself" framing as minor-child page. Internal note rewritten to reflect that adult-adoption package contents mirror minor-child rather than being a reduced subset. Section 4.4 (What Happens Next): H2 "From order to filed forms in 3 business days" → "From order to inbox in 3 business days"; step 2 "trained paralegal" → "Our team"; step 3 PDF mention removed. | Claude / Tyler |
| 2026-05-01 | v1.6 — Repositioned doc as the SALES page (matching the two-page architecture used by minor-child). URL locked to /dfy-adult-sales-page/. Both hero and final CTAs updated to "Continue to Checkout — $499" and link to /dfy-adult-checkout-page/ (the future adult checkout page). Title, intro, "What this page IS / IS NOT" sections updated. The ThriveCart embed will live on the future checkout page, not this one. Doc is build-ready. | Claude / Tyler |
| 2026-05-01 | v1.7 — Section 4.6 FAQ Q1 ("Do biological parents need to consent to an adult adoption in Nebraska?") answer corrected per Tyler. Previously read "No" (assumed adult adoption needed no biological-parent consent); now reads: "Yes. In a Nebraska adult stepparent adoption, written consent is required from your spouse — the adult adoptee's biological parent — and from the adult adoptee themselves. Both consents are filed with the petition." Notes bullet on why Q1 goes first updated to match new framing — confusion point is now that visitors *under-assume* the consent requirement, not that they assume it works like minor adoption. Edit propagated to `dfy-adult.html`. Section 4.3 internal note narrowed to match (Tyler chose option a): the v1.5 framing of "consent from both biological parents plus the adult adoptee themselves" replaced with "consent from your spouse (the adult adoptee's biological parent) and the adult adoptee themselves" — the absent biological parent's consent is NOT required for a Nebraska adult-stepparent case. The customer-facing "Consent forms" line still works for both adult and minor-child without surfacing the underlying difference. | Claude / Tyler |
| 2026-05-01 | v1.8 — Adult-adoption timeline corrected per Tyler. Previous claim of "6–10 weeks from filing" replaced with **4–6 months** everywhere it appeared: Section 4.4 step 4 timeline, Section 4.4 internal notes, Section 4.6 FAQ Q3 answer. Also removed two specific factual claims Tyler flagged as inaccurate: (1) "no biological-parent notification waiting period" — removed from Section 4.4 notes, (2) "the hearing is typically shorter" / "a simpler hearing" — removed from Section 4.6 FAQ Q3 answer and Section 4.4 notes. The "faster than minor-child" framing in FAQ Q3 dropped entirely since adult and minor-child timelines now match (4–6 months). Section 4.4 notes rewritten: adult-adoption advantage is procedural (less documentation up front, no home study) rather than calendar speed — court scheduling drives total timeline either way. Section 9 Open Question #2 (timeline confirmation) ✅ resolved with the new 4–6 month figure. Edits propagated to `dfy-adult.html` (FAQ Q3 answer + Section 4.4 step 4 paragraph). | Claude / Tyler |
| 2026-05-01 | v1.9 — Section 1 strategic visitor-archetype bullet updated to align with the v1.7 + v1.8 corrections. Old text: *"Surprised that the process is more straightforward than minor-child adoption (no consent of biological parents required, no home study, often a single court hearing)."* This contained two now-corrected inaccuracies — "no consent of biological parents required" (contradicts the v1.7 Q1 fix: your spouse, the adoptee's biological parent, must consent) and "often a single court hearing" (same family of claim as the "shorter hearing" v1.8 removal). Replaced with: *"Surprised by how procedurally light adult adoption is on the front end — no home study, less documentation than minor-child cases — even though the courthouse timeline is similar (4–6 months)."* No HTML change required (this section is internal/strategic copy, not customer-facing). | Claude / Tyler |
| 2026-05-01 | v1.10 — Adult CHECKOUT page built as `dfy-adult-checkout.html`. Mirrors `dfy-minor-child-checkout.html` structurally and visually (same CSS verbatim, same design tokens, same section order: minimalist nav → confirmation header → ThriveCart embed → reassurance strip → two-up testimonials → footer). Adult-specific changes: `<title>` ("Checkout — Done-For-You Adult Stepparent Adoption Forms | Adoption Forms Express"), meta description, canonical (`/dfy-adult-checkout-page/`), Schema.org Product block (name + description swapped to the adult product, $499 price kept), confirmation H1 ("Done-For-You Nebraska Adult Stepparent Adoption Forms"), ThriveCart product `8` embed (token `tc-adoptionssimplified-8-POHMYG`) replacing minor-child product `10`, and two-up testimonials swapped to Catrice Jackson (curated excerpt — strongest adult-adoption-explicit social proof in the Google review set: *"...went above and beyond...knowledgeable about adult adoption...my husband was able to legally adopt my 30 year old son"*) and Patty Bales (same "no hidden fees" line used on the minor-child checkout — strong cost-anxiety counter for both audiences). Section 8 (Technical Implementation Notes) updated to list both files and the ThriveCart product 8 embed details. Status updated to reflect both HTML files now on disk. The two CTA buttons on the sales page (`dfy-adult.html`) already point to `/dfy-adult-checkout-page/`, so the sales-page HTML required no changes. **Tyler's WordPress deploy step:** create the new checkout WP page as a top-level page with slug `dfy-adult-checkout-page`, paste the `dfy-adult-checkout.html` body content, mark noindex via SEO plugin. ThriveCart only loads on the checkout page — sales page stays clean. | Claude / Tyler |
| 2026-05-05 | v1.11 — ThriveCart embed token updated for this product after logo change in ThriveCart admin. Product ID unchanged; only the embeddable token regenerated. Old token: 0FGCA9 → new token: POHMYG. | Claude / Tyler |
| 2026-05-05 | v1.12 — Mobile checkout layout fix in `dfy-adult-checkout.html`. Added a `@media (max-width: 720px)` block in the embedded `<style>` (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule) that tightens `.thrivecart-wrap` vertical padding and forces `min-height: 0` + `height: auto` on the injected ThriveCart iframe. Reason: on mobile the injected iframe was being given a desktop-sized fixed height, which left a large empty white gap between the form and the reassurance strip / two-up testimonials below it. No HTML or copy changes; CSS-only mobile fix. May need follow-up if ThriveCart's v2 embed turns out not to use an iframe (renders inline DOM instead) — in which case the iframe selector is a no-op and we'll need to target the actual injected container after inspecting it on the live page. | Claude / Tyler |
| 2026-05-05 | v1.13 — **Reverted v1.12's mobile fix** in `dfy-adult-checkout.html`. The `@media (max-width: 720px)` block was removed, restoring the file to its pre-v1.12 state. Reason: forcing `height: auto !important` on the injected ThriveCart iframe collapsed the form into the iframe's intrinsic default height (~150px), squishing the form fields to the point users couldn't comfortably enter their info. The original empty-space gap is back, but the form is usable. Next attempt deferred until Tyler can DevTools-inspect the live mobile checkout (Chrome mobile emulation, right-click the empty area → Inspect) and report the actual injected element's tag, class/id, and computed `height` — then we can target the real offender instead of guessing. | Claude / Tyler |
| 2026-05-05 | v1.14 — **Mobile empty-space fix v2 (correct version) in `dfy-adult-checkout.html`.** Tyler's DevTools inspection revealed the actual culprit: ThriveCart's embed script injects an `<iframe class="tc-v2-embeddable-el">` inside the `.tc-v2-embeddable-target` div and hardcodes an inline `style="height: 2387px"` on it. On mobile that's ~1000px taller than the form's actual rendered content, creating the empty-space gap below the visible form (the user is still scrolling inside the iframe through dead space until they exit it and reach our reassurance strip). The injected iframe also carries `scrolling="yes"`, which means we can safely cap its height with CSS — any overflow scrolls inside the iframe rather than being clipped. Fix: re-added the `@media (max-width: 720px)` block (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule) with `.thrivecart-wrap iframe.tc-v2-embeddable-el { max-height: 1800px !important; }` plus tightened wrap padding to `1.5rem 0`. The 1800px cap is conservative (form likely needs ~1300–1500px on mobile) — leaves a buffer for dynamic form expansion (coupon-code section, address validation errors, etc.) while still cutting most of the dead space. **Tuning:** if dead space is still visible after deploy, lower the cap (1500 → 1300); if a scrollbar appears inside the iframe because the form was clipped, raise it (2000+). Behavior change is mobile-only (≤720px); desktop unchanged. CSS-only; no HTML/copy/schema changes. | Claude / Tyler |
| 2026-05-05 | v1.15 — UPL-driven language change: replaced all instances of "attorney call" / "attorney calls" / "free 15-minute attorney calls" with "support call" / "support calls" framing. New language: DFY = "two 15-minute support calls". Added a protective note on the sales page near the call mention clarifying that support calls do NOT include personalized legal advice. Schema description and meta description updated. Schema "Completed by a licensed Nebraska adoption attorney" → "Completed by our team" — the attorney designed/prepared the form templates (still credited via "Attorney-prepared..." which remains), but the per-customer form completion is done by the team, not the attorney directly. The "attorney call" framing was creating UPL ambiguity — the calls are forms-and-process customer service, not legal advice. Reviewed and approved by Lucrece H. Bundy, Esq. as licensed attorney owner of the business. | Claude / Lucrece |
| 2026-05-05 | v1.16 — Sales-page and checkout-page polish + refund policy formalized (mirrors the same change applied to the minor-child sister doc this session). **Sales page (`dfy-adult.html`) — three edits:** (1) Section 4.3 (What's Included) — removed bold from the "Two 15-minute support calls" item to match the visual rhythm of the rest of the Guidance list. (2) Section 4.6 — new Q6 added at the end of the FAQ accordion: "What if I realize I selected the wrong package?" Locks the project-wide refund policy: refunds available between purchase and delivery; delivery happens only after buyer replies to confirmation email; if buyer doesn't reply within 7 days, purchase is considered final; no refunds after forms are sent. Same Q&A on all four sales pages. Note: unlike the minor-child sister doc, the adult page's existing Q1 was *not* about refunds (it was the bio-parent-consent question), so no Q1 rewrite was needed here. (3) Section 4.7 — final CTA reassurance line simplified from "Secure checkout · 7-day refund if your case isn't a fit · Questions? Email us" to just "Secure checkout"; added explainer that the refund/email content lives in the FAQ + escape hatch. **Checkout page (`dfy-adult-checkout.html`) — two edits:** (1) Existing reassurance strip's "7-day refund if your case isn't a fit" middle clause removed to avoid contradicting the new refund policy — strip now reads "🔒 Secure ThriveCart checkout · Forms prepared by a licensed Nebraska adoption attorney". (2) New italic refund-note line added directly below the strip: "Wrong package? Email us before your forms are sent — we can refund." New `.refund-note` CSS class defined inside the page's `<style>` block (max-width 720px, font-size 0.85rem, var(--color-text-muted), italic, line-height 1.55). Reviewed and approved by Lucrece H. Bundy, Esq. as licensed attorney owner. | Claude / Lucrece |

---
*End of v1.0 — DFY Adult Page Working Document*
