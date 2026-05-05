# DIY Minor-Child Stepparent Adoption — Post-Qualification Sales Page

**Document type:** Page-level working document
**Owner:** Lucrece H. Bundy / Tyler
**URLs:** `/diy-minor-sales-page/` (sales page — `diy-minor-child.html`); `/diy-minor-checkout-page/` (transactional checkout page — `diy-minor-child-checkout.html`). The two pages will be sibling top-level pages in WordPress, mirroring the DFY architecture.
**Sister docs:**
- `dfy-minor-child-page-v1.md` (the structural template — DFY minor child)
- Future `diy-adult-page-v1.md` (DIY adult equivalent)
**Version:** 1.10
**Last updated:** May 5, 2026
**Status:** 🔵 Built — `diy-minor-child.html` and `diy-minor-child-checkout.html` on disk; pending WordPress deploy

---

## How to Use This Document

This is the page-level working doc for the **DIY minor-child product** — the $299 self-serve forms package for qualifying Nebraska stepparent adoption cases involving a stepchild under 19.

**Two-page architecture (mirroring DFY minor-child):** this is the SALES page (`/diy-minor-sales-page/`) — it does the convincing. The CHECKOUT page (`/diy-minor-checkout-page/`) is a separate sibling top-level page that does the transaction with an embedded ThriveCart. Both CTA buttons on this sales page link to the checkout page. The full funnel is: Homepage → Qualifier Quiz → THIS sales page → `/diy-minor-checkout-page/` → ThriveCart processes payment.

Inherits all site-wide standards from the master doc (`website-redesign-master.md`).

This is a sister doc to `dfy-minor-child-page-v1.md`. The two minor-child sales pages share **structure** exactly; the audience-specific content differs because **DIY buyers are a fundamentally different person than DFY buyers** — different motivation, different anxieties, different value proposition. Don't treat this as a price-swap of the DFY page.

---

## 1. Strategic Frame — What This Page Is And Isn't

### What this page IS

A **post-qualification sales page** for the DIY minor-child product. The visitor:

1. Found the site
2. Took the qualifier quiz
3. Was told they qualify
4. Their stepchild is a minor (under 19)
5. Was routed here by quiz logic to learn about the DIY package and decide whether to buy

The page exists to make them feel **confident, capable, and ready** to click through to the checkout page and complete the $299 purchase.

### What this page IS NOT

- **Not an SEO page.** `<meta name="robots" content="noindex,nofollow">`. Not in the sitemap.
- **Not the checkout page.** ThriveCart embeds do NOT live on this page — they live on `/diy-minor-checkout-page/` (a separate sibling page). The two CTA buttons on this page link to that checkout page.
- **Not a comparison page.** No DFY-vs-DIY comparison table. The qualifier quiz routed this specific visitor to the DIY product; they're here to evaluate THIS product, not choose between products.
- **Not a hand-holding manual.** This is a sales page, not the actual instructions. The instructions are part of what they receive after purchase.

### Why DIY ≠ DFY (this is the most important section to read)

A DIY buyer is fundamentally different from a DFY buyer. Same legal situation, but different person. The page must speak to **this person**, not the DFY person.

| Dimension | DFY buyer | DIY buyer |
|---|---|---|
| Core motivation | "I want this handled" | "I want this done affordably, and I'm willing to do the work" |
| Primary anxiety | "Will they actually do it right?" | "Can I figure this out? What if I get stuck?" |
| Value perception | Time and stress saved | Money saved + capability gained |
| Price sensitivity | Lower (already chose premium) | Higher (price IS the reason they're here) |
| Need from product | Confidence in delivery | Confidence in their own ability to use it |
| Best testimonial | "They handled everything for us" | "It was easy to do and understand" |

**Practical implications for the page:**

1. **Don't apologize for the product being self-serve.** That's the feature, not the bug.
2. **Don't compare to DFY.** The visitor doesn't need to be reminded a more expensive option exists.
3. **Lead with capability, not absence.** "You'll have everything you need" — not "You'll have to do it yourself."
4. **Show what's actually in the package generously.** Anxiety about "will I be able to do this?" is reduced by showing the product is comprehensive — forms, step-by-step instructions, support call.
5. **Position the support call as the safety net.** Not the main event. The forms and instructions are the main event; the call is what de-risks the whole thing.

### One-line page goal

**Confirm → equip → close.**

(Compared to DFY's "Confirm → reassure → close." The middle word is the difference. DFY visitors need *reassurance*; DIY visitors need to feel *equipped*.)

---

## 2. The Visitor — Who Lands Here

A married Nebraska resident who:

- Just completed the qualifier quiz
- Their stepchild is under 19
- Was routed to the DIY option (because they indicated price sensitivity, comfort with paperwork, or simply selected "show me both options" and is now evaluating DIY first)
- Wants the cheapest legitimate path to a finalized stepparent adoption
- Is comfortable doing paperwork themselves (not necessarily an expert, just not afraid of forms)
- Has a credit card in hand or about to grab it
- Is asking themselves *"Will this actually be enough? Will I get stuck? Is this a real product or a download-and-good-luck?"*

**What they need from this page:**

- Confirmation they're in the right place
- Specific, generous detail about what's in the $299 package
- Evidence that someone like them did this and it worked
- A clear sense of what they will actually do after they buy
- A safety net (the support call) for if they get stuck

**What they do NOT need:**

- A pitch for upgrading to DFY
- Long-form attorney-credibility copy (they're already past that gate — the qualifier quiz already established credibility)
- Hand-wringing about "is DIY right for you?" (they decided already)

---

## 3. Page Structure (Top to Bottom)

```
1. Sticky nav (logo + simple Email link — no menu)
2. Hero / qualification confirmation (eyebrow + H1 + qualification recap + primary CTA)
3. What You Get (forms list + instructions + support call — generously detailed)
4. How It Works After You Order (4-step: download → review → fill out → file)
5. Trust Block (Lucrece signature + 3 testimonials — Ruby Leonard featured)
6. Pre-Purchase FAQ (DIY-specific anxieties — different from DFY's FAQ)
7. Final CTA (single, prominent — links to checkout)
8. Escape Hatch (small, discreet — for visitors who realize DIY isn't right for them)
9. Footer (with UPL disclaimer)
```

The page is the same length as the DFY minor sales page (`dfy-minor-child.html`). Same sections in the same order. **What changes section by section is the COPY**, not the structure.

---

## 4. Section-by-Section Copy

### 4.1 Sticky Nav

Identical to the DFY minor sales page nav. Logo + "Email us" link. No menu items.

```
[Logo: Adoption Forms Express]                    Need help? Email us →
```

The right-side link is `mailto:adoptionformsexpress@gmail.com`.

---

### 4.2 Hero / Qualification Confirmation

**Eyebrow (small, success green):**
✓ You qualify for the DIY minor-child package

**H1:**
Your DIY minor-child stepparent adoption package is *ready* to download.

**Subhead:**
Your case fits our DIY package for minor-child stepparent adoptions. You'll get every Nebraska form you need to adopt your stepchild, step-by-step instructions, and one 30-minute support call when questions come up — all for $299.

**Qualification recap callout box (5 items):**
✓ Married Nebraska resident
✓ Adopting your spouse's biological child
✓ Stepchild is a minor
✓ Other biological parent will consent, their rights have been terminated, or they are deceased
✓ Case is uncontested

**Primary CTA button:**
Continue to Checkout — $299
*(button links to `/diy-minor-checkout-page/`)*

**Below the CTA, small text:**
*Secure checkout · Forms delivered within 1 business day · Includes one 30-minute support call*

**Notes:**
- Hero language emphasizes capability ("set up to do this yourself, with confidence") rather than absence ("you have to do it yourself")
- The italicized *yourself* signals the differentiator from DFY without naming DFY
- Subhead immediately previews the package contents — answers the unspoken "what do I actually get?" question
- "$299" appears in subhead (concrete) and on the CTA (commitment) — visitor sees price twice in the hero, removing surprise at checkout
- "Forms delivered within 1 business day" sets accurate expectations: there's a brief operational step between payment and delivery (a confirmation email about the consent/termination/deceased state of the other biological parent — not surfaced as detail in the copy). Still faster than DFY's 3-business-day turnaround, just not literally instant.

---

### 4.3 What You Get

This section does the most heavy lifting on the page. DIY anxiety is "will I actually have enough to do this?" — show generously that they will.

**H2:** Everything you need to finalize your minor-child stepparent adoption — without an attorney handling it.

**Subhead (one short line):**
Your $299 package includes forms, step-by-step instructions, and one 30-minute support call.

**Two-column layout:**

**Column 1 — The Forms (use the same form list as DFY minor child):**
- Petition for Adoption
- Notice of Adoption
- Consent to Adoption (for biological parent consent)
- [whatever other forms are in the actual product — pull verbatim from the DFY doc Section 4.3]
- All forms are given to you, ready to fill in with your information

**Column 2 — The Guidance** (stacked layout — bold heading on its own line, description underneath):
- **Step-by-step written instructions** — for each form: what goes where, what each section means in plain English.
- **One 30-minute support call** — use it whenever you need it. Most clients use it after they've drafted the forms but before they file.
- **Filing instructions** — exactly which county to file in, what fees to expect, and how to schedule your finalization hearing.

**Below the two columns, a single reassurance line:**
*Forms drafted by a licensed Nebraska adoption attorney. Backed by 140+ five-star reviews.*

**Notes:**
- Two-column structure mirrors the DFY page's "What You Get" section exactly — keeps visual sister-page feel
- Generous detail in Column 1 reduces the "will I have what I need?" anxiety
- Column 2 makes the support structure clear: instructions handle most cases, support call handles the edge cases
- Column 2 items render with the bold heading stacked above its description (not inline with an em-dash) so the column doesn't feel chopped up next to the plain-bullet Forms list
- Final reassurance line is intentional: it reinforces that even though the visitor is doing the work themselves, they're working with attorney-prepared materials, not generic templates
- **No email-access feature is offered** — the product includes the forms, instructions, and one 30-minute support call. General contact email exists in the nav and footer (mailto:adoptionformsexpress@gmail.com) but it's not framed as a feature with a response-time promise.

---

### 4.4 How It Works After You Order

**H2:** From order to finalized adoption — at your pace.

**Subhead:**
The whole process typically takes 4–6 months in Nebraska. Here's what your part looks like.

**Four-step grid:**

**Step 1 — Quick email confirmation**
Right after checkout, we'll send a short email to confirm a few details about your case. Once you reply, we'll send all your forms and the instruction guide — typically within one business day.

**Step 2 — Read through (1–2 hours)**
Look at the forms with your spouse. The instruction guide walks you through each one. Make a list of any questions you want to ask on your support call.

**Step 3 — Fill out the forms (a few evenings, at your pace)**
Work through the forms using the instructions. There's no deadline — you can take a week or a month. When you have questions, schedule your support call.

**Step 4 — File and finalize (Nebraska timeline: 4–6 months)**
Take the completed forms to your county courthouse along with the filing fee. The instructions tell you exactly how. After filing, you'll receive a hearing date — typically 2–4 months out.

**Notes:**
- "At your pace" framing in the H2 reframes the longer effort as flexibility rather than burden
- Step 1 sets accurate post-purchase expectations: a short confirmation-email exchange before delivery, with forms typically sent within one business day. Still faster than DFY (1 day vs 3) but doesn't promise instant.
- Step 2 includes "make a list of questions" — prepares them for the support call
- Step 3 explicitly says "there's no deadline" — addresses the DIY anxiety that they'll get behind
- Step 4 is the same as DFY but with "instructions tell you exactly how" emphasized — reinforces that they're not on their own for the filing step

---

### 4.5 Trust Block

**Section header:**

**H2:** Real attorney. Real Nebraska families.

**Lucrece signature block:**

[Photo: Lucrece headshot, circular, ~80px]
URL: `https://adoptionformsexpress.com/wp-content/uploads/2026/04/497A2015-scaled.jpg`

> "I designed this DIY package for Nebraska families who are comfortable doing paperwork but want the security of attorney-prepared forms. Every form, every instruction page comes from my actual practice handling stepparent adoptions for Nebraska families. If you get stuck, your support call is your safety net."
>
> **— Lucrece H. Bundy, Esq.**
> *Licensed Nebraska adoption attorney · Nebraska Bar #25734 · 140+ five-star reviews*

**Three review cards — all Google-verified, curated for the DIY audience:**

> "She is super friendly and knowledgeable. She helped us understand and know every case scenario possible. Thank you! We ended up purchasing the DIY Adoption documents for step-parent adoption and it was so easy to do and understand. When I had questions she would answer my emails promptly. She is very professional and very helpful. We are just waiting for the final court date. Thank you so much for having this available."
> — **Ruby Leonard** (Local Guide, edited 2024)

> "The adoption process was quick and effortless. Mrs. Bundy handled everything for us. We couldn't be more happy!"
> — **Sarah Hall** (Sep 2022)

> "Bundy Law made our step-parent adoption a quick and painless process. She explained every step along the way and answered all of our questions. Would absolutely use again for our family needs."
> — **Kevin Shafer** (Jan 2022)

**Notes:**
- **Ruby Leonard goes first** — she's the only Google review in the entire 142-review set that explicitly mentions purchasing the DIY adoption documents AND specifically calls them "easy to do and understand." That's the single most powerful piece of social proof on the entire DIY page. Lead with it.
- Sarah Hall is in slot 2 because "quick and effortless" reduces the DIY-buyer anxiety that this will be a slog
- Kevin Shafer is in slot 3 with "would absolutely use again" — general satisfaction, post-purchase
- The Lucrece signature copy is intentionally different from the DFY page — it acknowledges the DIY buyer's situation directly ("comfortable doing paperwork but want the security of attorney-prepared forms") and reframes the support call as a safety net rather than a feature
- Photo styling identical to DFY page (same image, same circular crop, same size)

---

### 4.6 Pre-Purchase FAQ

The FAQ is where DIY differs most from DFY because the questions are different. DIY visitors have specific anxieties about doing-it-themselves that need to be addressed.

**H2:** A few quick answers.

**FAQ accordion (6 questions, no FAQPage schema):**

**Q1: What if I get stuck?**
You have two places to turn. First, the instructions cover the most common questions — they're written in plain English and walk through every section of every form. Second, you have one 30-minute support call — most people use it about halfway through, after they've reviewed everything but before they file. Most clients finish their forms without needing the call at all.

**Q2: How is this different from your $499 Done-For-You package?**
Done-For-You means we complete the forms for you using information you provide. DIY means you receive blank forms with detailed instructions and you fill them out yourself. Same forms, same attorney-prepared quality. The difference is who does the typing — and the price reflects that.

**Q3: Can I really do this myself? Without legal training?**
Yes — that's exactly who this product is designed for. The forms are written in plain English, the instructions explain every section, and your support call is there when you need it. Most clients tell us the hardest part was deciding to start; the actual paperwork is more straightforward than they expected.

**Q4: What if my situation changes and I need more help?**
You can upgrade to Done-For-You at any time before filing — we credit your $299 toward the $499 package. Or you can hire Lucrece directly through Bundy Law for full attorney representation.

**Q5: How long until I receive everything?**
After payment, we'll send a short email to confirm a few details about your case. Once you reply, your forms and instruction guide are typically sent within one business day.

**Q6: What if I realize I selected the wrong package?**
Right after purchase, we'll email you to confirm which scenario applies to your case and which package you ordered. We don't send your forms until you reply confirming both. If at that point you realize you bought the wrong package, just reply and let us know — we'll refund you, and you can purchase the correct one. If you don't reply to our confirmation emails within 7 days of purchase, we consider your purchase final and refunds are no longer available. After we've sent your forms, we cannot refund.

**Notes:**
- Q1 leads because "what if I get stuck?" is the central DIY anxiety. It needs to be the first question answered with concrete safety nets — instructions first, support call second.
- Q2 is the only question that mentions DFY — by name, briefly, framed as "if you'd rather we type, here's that option." Doesn't oversell DFY; just answers the question and moves on.
- Q3 names the imposter syndrome head-on. Most DIY visitors are quietly worried they're about to get in over their heads. Reassuring them with "the hardest part was deciding to start" is exactly the right note.
- Q4 is the upgrade path — important for protecting the buyer: if life happens, they're not stuck. The $299→$499 credit removes the hesitation that "what if I have to switch later?"
- Q5 sets honest expectations: there's a brief confirmation-email step before forms are delivered. The 1-business-day turnaround is still a meaningful speed advantage over DFY's 3 business days for visitors who care about getting started quickly.
- Q6 is the project-wide refund-policy single source of truth — same Q&A appears on all four sales pages.
- No FAQPage schema — same reasoning as DFY page (gated checkout-funnel page should not surface in search).

---

### 4.7 Final CTA

**H2:** Ready to *get started?*

**Below H2:**
Your $299 DIY package, with everything you need to finalize your minor-child stepparent adoption — at your pace.

**Primary CTA button:**
Continue to Checkout — $299
*(button links to `/diy-minor-checkout-page/`)*

**Below the CTA, small reassurance line:**
*Secure checkout*

**Notes:**
- "Get started?" mirrors the DFY final CTA H2 — keeps the sister-page feel
- The italicized "*get started?*" matches the H1 italics styling for consistency
- Reassurance line trimmed to a single phrase — by the time qualifying visitors reach the final CTA on a gated post-quiz page, refund/email-question messaging is friction, not reassurance. Refund mechanics live in the FAQ (Q6); the support escape hatch lives in Section 4.8. Same trim applied across all four sales pages this session.

---

### 4.8 Escape Hatch

A small, discreet section below the final CTA for visitors realizing DIY isn't right for them. Don't make this prominent — most visitors should not see this. But for the few who need it, it's a softer exit than the back button.

**Copy:**

> Realizing your situation may not be a fit for DIY? That's okay — every case is different.
>
> If you'd rather have us complete the forms for you, our [Done-For-You package](/dfy-minor-sales-page/) is $499 and we deliver completed forms within 3 business days.
>
> If your case may be contested or unusual, [email us](mailto:adoptionformsexpress@gmail.com) and we'll point you in the right direction — including referrals to Bundy Law LLC for full attorney representation.

**Notes:**
- Two soft exits: upgrade to DFY, or get a referral to full attorney representation
- The DFY link IS the only place on the page that mentions DFY by name — and only as a sympathetic alternative for visitors who realized DIY isn't right
- No buttons here — text links only. This is intentionally less visually prominent than the primary CTA above it.

---

### 4.9 Footer

Identical to homepage and DFY pages. Same UPL disclaimer, same social links, same contact info.

---

## 5. Visual System

Inherits all design tokens from `homepage.html` and `dfy-minor-child.html`:
- Fonts: Fraunces (display) + Manrope (body)
- Colors: navy primary, coral accent, cream background, success green
- Component patterns: same nav, same FAQ accordion, same testimonial cards, same Lucrece signature block, same final CTA, same footer
- The DIY page must look like a clear sister of `dfy-minor-child.html` — same visual language, only the copy differs

**Pricing visual:** wherever $299 appears, give it the same visual weight DFY's $499 has. Same font, same emphasis. Don't visually downgrade the price (a smaller font or muted color would subtly suggest the product is lesser).

---

## 6. SEO & Indexing

### Critical: this page is NOT indexed.

- `<meta name="robots" content="noindex,nofollow">` in the head
- Excluded from sitemap (configure in SEO plugin after deploy)
- Not linked from any indexed page
- Canonical: `https://adoptionformsexpress.com/diy-minor-sales-page/`
- WordPress page settings: noindex, exclude from sitemap

### Future SEO sister page

A future public-facing page (`/diy-stepparent-adoption-nebraska/` or similar) will do the SEO work for the DIY product, funneling visitors through the qualifier quiz. That page is separate from this one and not yet built.

---

## 7. Schema Markup

Single Product schema in the head:

```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "DIY Nebraska Stepparent Adoption Forms (Minor Child)",
  "description": "Attorney-prepared blank Nebraska stepparent adoption forms for minor-child cases, with step-by-step instructions and one 30-minute support call. Designed for Nebraska families completing the paperwork themselves.",
  "brand": { "@type": "Brand", "name": "Adoption Forms Express" },
  "offers": {
    "@type": "Offer",
    "price": "299",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock"
  }
}
```

**Do NOT include:**
- FAQPage schema (gated page should not surface FAQ rich results in search)
- AggregateRating (gated page; aggregate rating belongs on indexed pages like the homepage)

---

## 8. Technical Implementation Notes

- Page is built as a single self-contained HTML file in the same style as `dfy-minor-child.html`
- Same design tokens, typography, button styles, FAQ accordion logic
- File name: `diy-minor-child.html`
- Deployed to URL: `/diy-minor-sales-page/`
- WordPress: created as a new page with Blank Slate template + Custom HTML block
- WordPress page settings: noindex via SEO plugin, excluded from sitemap
- Removed from primary nav menu
- Both CTA buttons (hero + final) link to `/diy-minor-checkout-page/`

### ThriveCart embed location

This page does NOT contain the ThriveCart embed. ThriveCart lives on the separate checkout page at `/diy-minor-checkout-page/`. The CTAs on this sales page link to that checkout page.

---

## 9. Open Questions / Decisions Needed

| # | Question | Status | Resolution |
|---|---|---|---|
| 1 | Confirm exact list of forms in DIY package | Open | Pull verbatim from `dfy-minor-child-page-v1.md` Section 4.3 — DIY forms list should match DFY since both products use the same Nebraska state forms (the difference is who fills them out). |
| 2 | Background-check fee disclosure | Open | Mirror the DFY page's approach to county-specific background check fees. |
| 3 | DIY-to-DFY upgrade credit mechanism | Open | FAQ Q4 promises "we credit your $299 toward the $499 package" — confirm this is operationally feasible in ThriveCart and Bundy Law's system. May need a manual process initially. |

---

## 10. Change Log

| Date | Change | Author |
|---|---|---|
| 2026-05-01 | v1.0 — Initial DIY minor-child sales page spec drafted. Modeled on `dfy-minor-child-page-v1.md` with DIY-specific repositioning. Key differences from DFY: 5-item qualification recap (one item difference), value prop emphasizes capability + savings rather than time saved, "What You Get" emphasizes generous package detail, "How It Works" reframes 4-step process around the buyer's actions, FAQ leads with "what if I get stuck?" anxiety, Ruby Leonard featured in slot 1 of testimonials (only Google review explicitly mentioning DIY purchase), $299 pricing visually equal to DFY's $499 (no visual downgrade), upgrade-to-DFY path included in escape hatch. ThriveCart product 4 (token tc-adoptionssimplified-4-KP063D) confirmed as DIY minor-child product — embed lives on the checkout page, not this sales page. | Claude / Tyler |
| 2026-05-01 | v1.1 — Both DIY minor-child HTML files built and copy iterated to final shape. **Files built:** `diy-minor-child.html` (sales page, 1048 lines) mirrors `dfy-minor-child.html` structurally with DIY-specific copy from spec; `diy-minor-child-checkout.html` (checkout page, 455 lines) mirrors `dfy-minor-child-checkout.html` with ThriveCart product 4 embedded (token `tc-adoptionssimplified-4-KP063D`) and DIY testimonials (Ruby Leonard curated excerpt + Patty Bales). Both pages noindex; both CTAs on the sales page link to `/diy-minor-checkout-page/`. **In-session copy edits beyond v1.0 spec:** (1) Hero qualification recap: "Stepchild is under 19" → "Stepchild is a minor"; "Other biological parent will consent (or rights have been terminated)" → "Other biological parent will consent, their rights have been terminated, or they are deceased" (now mirrors homepage's three-state framing). (2) Forms last bullet: "All forms are blank, ready for you to fill in your information" → "All forms are given to you, ready to fill in with your information." (3) Guidance column restructured into bold-stacked layout (bold heading on its own line, description underneath) via new CSS rule `.included-col li strong { display: block; ... }` so the column doesn't read chopped-up next to the plain-bullet Forms list. (4) **Email access removed** — dropped "Email access" bullet from Guidance (3 items now, not 4) and removed the email-access reference from FAQ Q1 (reframed as "two places to turn"). General contact mailto links in nav/footer remain; product no longer markets ongoing email support as a feature. (5) "What Happens Next" H2 + step 3 H3: `&nbsp;` between "your" and "pace" so "pace" doesn't orphan to its own line on narrow widths. (6) **"Instant" framing replaced** across 4 spots (hero CTA note, Step 1 title + description, FAQ Q5, checkout subhead) — page now sets accurate expectations: brief confirmation-email step before delivery, with forms typically sent within one business day. Strategic notes in Sections 4.2/4.4/4.6 updated to reflect the corrected positioning (still faster than DFY's 3 business days, just not literally instant). The DIY minor-child funnel is feature-complete locally — pending WordPress deploy. | Claude / Tyler |
| 2026-05-01 | v1.2 — **Minor-child clarity pass.** The v1.1 page-identity copy was generic ("DIY package") in spots where a misrouted visitor wouldn't immediately know they'd landed on the minor-child page. Six surface-level edits make the page identity unmistakable: (1) `<title>` → "DIY Nebraska Stepparent Adoption Forms (Minor Child) — Adoption Forms Express"; (2) meta description → "The DIY Nebraska stepparent adoption package for adopting a minor stepchild…"; (3) Hero eyebrow → "✓ You qualify for the DIY minor-child package"; (4) Hero subhead → "Your case fits our DIY package for minor-child stepparent adoptions. You'll get every Nebraska form you need to adopt your stepchild…"; (5) "What's Included" H2 → "Everything you need to finalize your minor-child stepparent adoption…"; (6) Final CTA subhead → "Your $299 DIY package for minor-child stepparent adoptions, with everything you need to finalize at your pace." H1 deliberately untouched — minor-child label lives in eyebrow + subhead + section H2s where it lands without becoming repetitive. Mirrored in spec Sections 4.2, 4.3, 4.7. Schema name already specified "(Minor Child)" so no change there. Checkout page already says "Minor Child" prominently in H1 and required no change. | Claude / Tyler |
| 2026-05-01 | v1.3 — **Guidance-column layout bug fix.** v1.1 introduced a CSS rule (`.included-col li strong { display: block; ... }`) intended to stack the bold heading above the description on each Guidance bullet. The rule didn't actually achieve stacking because each `<li>` is a flex container — `<strong>` and the description text were siblings inside the flex layout, so they rendered side-by-side on one row instead of stacking. Visible result: the three Guidance items looked like crammed-together blocks, not heading-over-description pairs. Fix: wrapped each Guidance `<li>`'s content in a `<div>` so the wrapper becomes a single flex item, and inside the wrapper (a regular block-formatting context) the `<strong>` block-display rule actually stacks above the description as intended. CSS unchanged; only the markup of the three Guidance `<li>` items in `diy-minor-child.html` was restructured. Spec Section 4.3's stacked-layout description was already accurate from v1.1; this fix makes the rendered HTML match what the spec describes. | Claude / Tyler |
| 2026-05-01 | v1.4 — **Final-CTA line-break polish.** The v1.2 minor-child clarity pass made the final-CTA subhead read as an awkward two-clause sentence ("...for minor-child stepparent adoptions, with everything you need...") that wrapped unevenly when centered, creating ragged lines. Two fixes applied: (1) Subhead reworded back toward v1.1's cleaner three-beat structure with "minor-child" inserted naturally as a modifier on "stepparent adoption" (singular noun phrase): *"Your $299 DIY package, with everything you need to finalize your minor-child stepparent adoption — at your pace."* `&nbsp;` between "your" and "pace" prevents the closer from orphaning. Mirrored in spec Section 4.7. (2) CSS: added `text-wrap: balance` to `.final-cta h2`, `.final-cta p`, and `.final-cta-note` so multi-line centered text balances to equal line widths automatically instead of looking ragged. Browser support is good across Chrome/Safari/Firefox (shipped 2023–2024). | Claude / Tyler |
| 2026-05-05 | v1.5 — ThriveCart embed token updated for this product after logo change in ThriveCart admin. Product ID unchanged; only the embeddable token regenerated. Old token: TTC0UE → new token: KP063D. | Claude / Tyler |
| 2026-05-05 | v1.6 — Mobile checkout layout fix in `diy-minor-child-checkout.html`. Added a `@media (max-width: 720px)` block in the embedded `<style>` (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule) that tightens `.thrivecart-wrap` vertical padding and forces `min-height: 0` + `height: auto` on the injected ThriveCart iframe. Reason: on mobile the injected iframe was being given a desktop-sized fixed height, which left a large empty white gap between the form and the reassurance strip / two-up testimonials below it. No HTML or copy changes; CSS-only mobile fix. May need follow-up if ThriveCart's v2 embed turns out not to use an iframe (renders inline DOM instead) — in which case the iframe selector is a no-op and we'll need to target the actual injected container after inspecting it on the live page. | Claude / Tyler |
| 2026-05-05 | v1.7 — **Reverted v1.6's mobile fix** in `diy-minor-child-checkout.html`. The `@media (max-width: 720px)` block was removed, restoring the file to its pre-v1.6 state. Reason: forcing `height: auto !important` on the injected ThriveCart iframe collapsed the form into the iframe's intrinsic default height (~150px), squishing the form fields to the point users couldn't comfortably enter their info. The original empty-space gap is back, but the form is usable. Next attempt deferred until Tyler can DevTools-inspect the live mobile checkout (Chrome mobile emulation, right-click the empty area → Inspect) and report the actual injected element's tag, class/id, and computed `height` — then we can target the real offender instead of guessing. | Claude / Tyler |
| 2026-05-05 | v1.8 — **Mobile empty-space fix v2 (correct version) in `diy-minor-child-checkout.html`.** Tyler's DevTools inspection revealed the actual culprit: ThriveCart's embed script injects an `<iframe class="tc-v2-embeddable-el">` inside the `.tc-v2-embeddable-target` div and hardcodes an inline `style="height: 2387px"` on it. On mobile that's ~1000px taller than the form's actual rendered content, creating the empty-space gap below the visible form (the user is still scrolling inside the iframe through dead space until they exit it and reach our reassurance strip). The injected iframe also carries `scrolling="yes"`, which means we can safely cap its height with CSS — any overflow scrolls inside the iframe rather than being clipped. Fix: re-added the `@media (max-width: 720px)` block (just below the existing `.thrivecart-wrap .tc-v2-embeddable-target { width: 100%; }` rule) with `.thrivecart-wrap iframe.tc-v2-embeddable-el { max-height: 1800px !important; }` plus tightened wrap padding to `1.5rem 0`. The 1800px cap is conservative (form likely needs ~1300–1500px on mobile) — leaves a buffer for dynamic form expansion (coupon-code section, address validation errors, etc.) while still cutting most of the dead space. **Tuning:** if dead space is still visible after deploy, lower the cap (1500 → 1300); if a scrollbar appears inside the iframe because the form was clipped, raise it (2000+). Behavior change is mobile-only (≤720px); desktop unchanged. CSS-only; no HTML/copy/schema changes. | Claude / Tyler |
| 2026-05-05 | v1.9 — UPL-driven language change: replaced all instances of "attorney call" / "attorney calls" with "support call" / "support calls" framing across Section 4 customer copy + Section 8 schema spec + the strategic notes that referenced the call by name (Section 1 voice principles, Section 2 visitor needs, Section 3 page architecture, Section 4 internal notes). New language: DIY = "one 30-minute support call". Added a protective note on the sales page near the call mention clarifying that support calls do NOT include personalized legal advice. The "attorney call" framing was creating UPL ambiguity — the calls are forms-and-process customer service, not legal advice. Reviewed and approved by Lucrece H. Bundy, Esq. as licensed attorney owner of the business. | Claude / Lucrece |
| 2026-05-05 | v1.10 — Sales-page and checkout-page polish + refund policy formalized (mirrors the same change applied to the DFY sister docs this session). **Sales page (`diy-minor-child.html`) — two edits:** (1) Section 4.6 — new Q6 added at the end of the FAQ accordion: "What if I realize I selected the wrong package?" Locks the project-wide refund policy: refunds available between purchase and delivery; delivery happens only after buyer replies to confirmation email; if buyer doesn't reply within 7 days, purchase is considered final; no refunds after forms are sent. Same Q&A on all four sales pages. (2) Section 4.7 — final CTA reassurance line simplified from "Secure checkout · 7-day refund if your case isn't a fit · Questions? Email us" to just "Secure checkout"; the refund-line + email-link are now redundant on a gated post-quiz page where Q6 holds the canonical refund policy. **Checkout page (`diy-minor-child-checkout.html`) — two edits:** (1) Existing reassurance strip's "7-day refund if your case isn't a fit" middle clause removed to avoid contradicting the new refund policy — strip now reads "🔒 Secure ThriveCart checkout · Forms prepared by a licensed Nebraska adoption attorney". (2) New italic refund-note line added directly below the strip: "Wrong package? Email us before your forms are sent — we can refund." New `.refund-note` CSS class defined inside the page's `<style>` block (max-width 720px, font-size 0.85rem, var(--color-text-muted), italic, line-height 1.55). DIY-specific note: this product had no Q1 about case-complexity refunds (DIY Q1 is "What if I get stuck?"), so unlike the DFY minor-child sister doc, no Q1 rewrite was needed. Reviewed and approved by Lucrece H. Bundy, Esq. as licensed attorney owner. | Claude / Lucrece |
