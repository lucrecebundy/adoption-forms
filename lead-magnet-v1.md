# Lead Magnet — The Nebraska Stepparent Adoption Starter Guide

**Document type:** Project-level working document for the entire lead-magnet system (PDF + email sequence + landing page + platform setup + wiring)
**Owner:** Lucrece H. Bundy, Esq.
**Public URL (landing page):** `/starter-guide/`
**Deliverable filename (PDF):** `nebraska-stepparent-adoption-starter-guide.pdf`
**Sister docs:**
- `website-redesign-master.md` (site-wide standards)
- `homepage-redesign-v1.md` (homepage already references this asset in 4 places)
- All four product page docs (the guide funnels TO the qualifier quiz, which routes TO these products)
**Version:** 1.3
**Last updated:** May 5, 2026
**Status:** Draft — scope and structure locked; content writing pending

---

## How to Use This Document

This is the project-level working doc for the entire lead-magnet system, not just the PDF. The lead magnet has five distinct deliverables:

1. The PDF guide itself (the main asset)
2. The email nurture sequence (5–7 emails after signup)
3. The landing page at `/starter-guide/` (email capture page)
4. The email platform configuration (ConvertKit / MailerLite / etc.)
5. Wiring everything together (replace `#` stubs in homepage HTML, test the flow)

This document covers all five. As individual deliverables get built (PDF written, landing page built, etc.), they may spawn their own sister docs (e.g., `lead-magnet-email-sequence-v1.md`). For now, everything lives here.

**Sequencing:** PDF content first → email sequence → landing page → email platform setup → wiring. Reason: the PDF is the substance; everything else markets it, delivers it, or follows up on it.

---

## 1. Strategic Frame

### What this asset IS

A **top-of-funnel awareness builder** designed to capture email addresses from people who Google their way to the site but aren't ready to take the qualifier quiz yet. The guide answers their early-stage questions, builds trust, and warms them up to the paid products over the email nurture sequence that follows.

### What this asset IS NOT

- **Not a sales pitch.** The guide's primary job is to be genuinely useful, not to push the products. The CTA appears at the end (and softly throughout), not in every section.
- **Not personalized legal advice.** Despite Lucrece authoring it, the substance is general educational information about Nebraska adoption procedure. Personalized advice requires an attorney-client relationship, which the guide does not establish. (See UPL framing below.)
- **Not the qualifier quiz.** The guide does not qualify or disqualify readers — it educates them. At the end, it points them TO the qualifier quiz.
- **Not a substitute for the products.** A reader who downloads the guide should walk away knowing what their next step is (taking the quiz, then either DIY/DFY or contacting an attorney for a complex case). The guide doesn't include the actual forms.

### Strategic role in the funnel

```
Public traffic (Google, AI search, social)
    ↓
Homepage / pillar pages
    ↓ (some bounce — this captures them)
Lead magnet landing page (/starter-guide/)
    ↓ (email signup)
PDF delivered + email sequence begins
    ↓ (warmed up over 5–7 emails)
Qualifier quiz (Typeform)
    ↓
Sales page (DIY or DFY, minor or adult)
    ↓
Checkout page → ThriveCart → purchase
```

The lead magnet captures the visitor who isn't ready to take the quiz yet. Without the lead magnet, that visitor leaves the site and is gone forever. With the lead magnet, you have their email and seven days to convince them.

### Why a guide specifically (not a checklist or template)

A 1-page checklist or a single-form template feels small and underwhelming to the audience. Stepparent adoption is a substantial life event; potential buyers are doing real research. A 20-page substantive guide signals "this person actually knows what they're talking about" in a way a 2-page checklist doesn't.

Also: the guide's content can be **excerpted into future SEO pillar pages**. Writing it once gives double-duty — the lead magnet AND the foundation of public SEO content.

---

## 2. The Reader — Who Downloads This

A Nebraska resident who is:

- Considering or actively planning a stepparent adoption (minor child OR adult stepchild)
- Researching online before committing to anything
- Not yet sure whether they need an attorney, can DIY, or qualify for a stepparent adoption at all
- Moderately to highly anxious about the legal process — wants orientation, not confusion

### Stages of awareness (which the guide moves them through)

1. **Initial Google search** — "how does stepparent adoption work in Nebraska" / "stepparent adoption forms Nebraska" / "do I need a lawyer for stepparent adoption"
2. **Lands on Adoption Forms Express homepage** — sees the homepage, reads some, isn't ready to take the quiz
3. **Sees the freebie offer** — "Get the free Nebraska Adoption Guide" (homepage hero, FAQ footnote, footer)
4. **Clicks through to /starter-guide/** — reads the landing page, decides whether to give email
5. **Submits email** — gets PDF + first email
6. **Reads PDF** — comes away understanding the process, the timeline, the costs, and which scenarios qualify
7. **Email nurture begins** — over 5–7 emails, soft trust-building toward the quiz CTA
8. **Takes the quiz** — at the moment they're ready

The guide's job is to take them from stage 4 to stage 7 confidently.

---

## 3. UPL Framing — Critical Constraint

**The guide is general educational information, not legal advice.** This is non-negotiable per master doc Section 3 UPL guardrails.

### How this is enforced in the document

1. **Authorship framing.** Lucrece introduces herself in the first page and signs off in the closing page; the body is written in a neutral instructional voice ("In Nebraska, stepparent adoption requires…"). Avoid writing "I recommend…" or "you should…" in the substance — those phrases are advice, not education.
2. **Explicit disclaimer near the top.** Page 1 (after Lucrece's welcome): a clear note that the guide is general educational information about Nebraska adoption procedure, not legal advice for any specific case. Reading it does not establish an attorney-client relationship.
3. **Recurring "talk to an attorney" callouts where appropriate.** When the guide reaches a topic where individual circumstances vary significantly (contested cases, unusual consent dynamics, out-of-state issues), it should explicitly note "if your situation involves X, consult a licensed attorney" — not try to advise on it.
4. **No specific case predictions.** The guide should never include phrases like "your case will be approved" or "you'll definitely qualify if…" — only conditional, educational framings ("Nebraska courts generally consider X factors").
5. **Footer disclaimer on every page.** Same UPL footer disclaimer that appears on every web page should appear in the PDF footer.

### What's safe to include vs. unsafe

| Safe | Unsafe |
|---|---|
| "In Nebraska, stepparent adoption typically takes 4–6 months from filing." | "Your case will probably be approved within 4 months." |
| "Under Neb. Rev. Stat. § 43-104, the consent of both biological parents is generally required for adoption." | "Based on your situation, you should pursue [specific] pathway." |
| "Nebraska courts may appoint a guardian ad litem in cases involving abandonment, which is one reason these cases require attorney representation." | "If you haven't heard from the other parent in 6 months, you can use these forms." |
| "Nebraska's filing fees range from approximately $60–$90 depending on the county." | "I'll waive the filing fee for you." |
| "Most uncontested stepparent adoptions in Nebraska proceed through county court without major issues." | "Your stepparent adoption will be uncontested." |
| "Adult adoptions in Nebraska are exempt from the home-study requirement under § 43-107(1)(b)(v) unless the court orders otherwise." | "You won't need a home study for your case." |
| Case studies labeled as illustrative ("In one common scenario…") | Specific case predictions for the reader |

The body of the guide stays in the safe column. Lucrece's voice in the intro/closing can be slightly warmer ("I built this guide because…") but should never cross into specific advice for the reader.

---

## 4. Document Specifications

**Title:** The Nebraska Stepparent Adoption Starter Guide

**Subtitle:** A plain-English overview of the process, timeline, costs, and your options — written by a licensed Nebraska adoption attorney.

**Length:** ~20 pages, approximately 5,000–6,000 words. Comfortable read in one sitting.

**Format:** PDF download. Single file, designed for both desktop and mobile/tablet reading.

**Visual design tokens:** Inherit from the website's brand system (master doc Section 4):
- Fonts: Fraunces (display headers) + Manrope (body) — both have free PDF-embeddable licenses
- Colors: same warm navy (`#1F3A5F`), coral accent (`#E07856`), cream background tints
- Page layout: clean, generous margins, professional but approachable feel
- Photo (page 1): Lucrece's professional headshot, same one used in homepage signature block (`/wp-content/uploads/2026/04/497A2015-scaled.jpg`)

**File naming:** `nebraska-stepparent-adoption-starter-guide.pdf`

**Version control:** First release is v1.0. Major revisions bump to v2.0 (e.g., a substantial content update or significant legal change). Minor edits (typos, phrasing fixes) bump to v1.1, v1.2, etc. Track in this document's change log.

---

## 5. Section-by-Section Structure

The guide is structured in 11 sections plus a cover and back page. Each section's purpose, target length, and key content points are below. The actual content writing happens in the next session.

### Cover Page

**Visual treatment:**
- Title: "The Nebraska Stepparent Adoption Starter Guide" — large, Fraunces, navy
- Subtitle in smaller Manrope, muted color
- Adoption Forms Express logo
- Author byline: "By Lucrece H. Bundy, Esq."
- Optional: simple warm visual element (cream background with subtle accent)

**Length:** 1 page

---

### Section 1 — Welcome from Lucrece

**Purpose:** Establish authorial credibility and warmth in 250–350 words. The reader should finish this page knowing Lucrece is a real Nebraska attorney who genuinely cares about helping families.

**Voice:** First-person, warm, professional but approachable. Lucrece's voice.

**Key points to cover:**
- Brief introduction of Lucrece (Nebraska adoption attorney, X+ years, X+ adoptions handled)
- Why she wrote this guide ("I kept seeing the same questions from families starting this process…")
- What the reader will get from reading it (orientation, not advice)
- A note that the guide is educational, not legal advice (also formal disclaimer follows on next page)
- Soft warmth: "wherever your family is in this journey, you're not alone"

**Tone calibration:** Professional, not casual. Confident, not preachy. Honest, not performative.

**Length:** 1 page

---

### Section 2 — Important Legal Note

**Purpose:** Explicit, clear UPL disclaimer. No reader should be able to claim later that they thought the guide was personalized legal advice.

**Length:** ~150 words, half a page or full page with breathing room

**Required content:**
- This guide is general educational information about Nebraska stepparent adoption procedure
- Reading it does not establish an attorney-client relationship
- Every adoption is unique; specific cases need specific legal advice
- For your specific case, consult a licensed Nebraska adoption attorney (link to Bundy Law LLC at the end)
- The information is current as of [date], but laws change — verify any specific point with current Nebraska sources

**Voice:** Clear, direct, neutral. Not warm — this is the legal protection page.

---

### Section 3 — What Stepparent Adoption Actually Is

**Purpose:** Define the thing. Many readers don't actually know what stepparent adoption is in legal terms; they only know what they want it to do.

**Length:** ~600 words, 2–3 pages

**Key points:**
- Legal definition: stepparent adoption is the formal legal process by which a stepparent becomes the legal parent of their spouse's biological child
- What changes legally after the adoption: parental rights, inheritance, name change, decision-making authority
- What does NOT change: the relationship that already exists (the legal status catches up to the family reality)
- Brief: minor vs. adult stepparent adoption (with a note that the guide covers both)
- Why families pursue it: legal security, name unification, inheritance/estate planning, emotional formalization

**What's distinct about Nebraska:** brief note that adoption laws vary by state; this guide is specifically about Nebraska.

---

### Section 4 — When Nebraska Stepparent Adoption Can Be Done Without Full Attorney Representation

**Purpose:** Explain the three specific scenarios in which a Nebraska family can complete a stepparent adoption using forms and instructions rather than retaining a full-service attorney. **This is THE core content of the guide.**

**Critical framing:** This section is NOT a comprehensive description of Nebraska adoption law. Nebraska adoption procedure is broader and more complex than what's covered here. This section specifically explains the narrow set of circumstances in which a family realistically can use a forms-based product (like Adoption Forms Express's DIY or Done-For-You packages) instead of hiring an attorney.

**Statutory grounding:** Nebraska's adoption statutes (Neb. Rev. Stat. §§ 43-101 to 43-115) generally require that, for a child to be eligible for adoption, the parental rights of the existing parent(s) must be either terminated or relinquished. The Nebraska Supreme Court confirmed this general rule in *In re Adoption of Luke*, 263 Neb. 365 (2002), which held that "aside from the stepparent adoption scenario, the parents' parental rights must be terminated or the existing nonterminated parent or parents must relinquish in order for the child to be eligible for adoption." The stepparent adoption is the recognized statutory exception to this general termination/relinquishment rule.

**The general rule in Nebraska:** Most adoptions require attorney representation. The three scenarios below are the specific circumstances where consent rules under § 43-104 are clear enough — and uncontested enough — that a forms-based approach can work.

**Length:** ~1,200 words, 3–4 pages

**The three qualifying scenarios:**

**Scenario 1 — The other biological parent consents to the adoption**
- Statutory basis: § 43-104(1) requires written consent from both biological parents (with limited exceptions); when consent is given, the case is uncontested.
- What consent looks like: written, signed, often notarized; consent is filed with the petition.
- The "other parent fully agrees" scenario.
- Most common qualifying scenario.
- Important: agreement in spirit isn't enough. Without a signed, written consent properly executed and filed, this becomes a contested case requiring an attorney.

**Scenario 2 — The other biological parent is deceased**
- Statutory basis: § 43-104(1)(b) requires consent of "the surviving parent of a child born in lawful wedlock" — meaning when one biological parent is deceased, only the surviving parent's consent is required.
- Death certificate as proof, filed with the petition.
- The cleanest qualifying scenario operationally.
- Brief note: for adult stepparent adoptions, the adult adoptee's consent is also required under § 43-104(1)(a) (note: the statute requires consent of the minor child if over 14; adult adoptee consent flows from the broader adoption framework in § 43-101(2)).

**Scenario 3 — The other biological parent's rights have been previously terminated through a separate court action**
- Statutory basis: when parental rights have already been terminated by court order, that parent's consent is no longer required because they no longer hold parental rights.
- The other biological parent's rights were terminated in a SEPARATE, PRIOR court action (juvenile court, district court, etc.) — NOT as part of this stepparent adoption proceeding.
- Court records of the prior termination order serve as proof, filed with the petition.
- **Critical distinction:** This scenario is about a *previously completed* termination — documented by an existing court order. Terminating parental rights as PART of the stepparent adoption itself is a contested case requiring full attorney representation; that's NOT what this scenario covers.

**What is NOT in scope for these products — even if it might seem like it should be:**

This is critically important. Several scenarios that Nebraska law may technically allow as paths toward adoption are NOT appropriate for forms-based DIY/DFY products and require full attorney representation:

- **Abandonment cases.** If the other biological parent has been absent for an extended period without consent or contact, Nebraska courts will typically appoint a guardian ad litem to represent the child's interests, evaluate the abandonment claim, and protect the rights of the absent parent. This makes the case complex, fact-intensive, and procedurally demanding — not appropriate for a forms-based path. Families in this situation should work with a full-service attorney. **The qualifier quiz screens these cases out and routes them to attorney referral.**
- **Cases where you want to terminate the other parent's rights as part of the adoption.** This is a contested proceeding requiring full legal representation.
- **Out-of-state complications.** Cases where the absent parent lives in another state, where there's an existing custody order from another jurisdiction, or where the Uniform Child Custody Jurisdiction and Enforcement Act may apply.
- **Cases where the other parent's whereabouts are unknown.** Notice-by-publication procedures and related diligent search requirements (§ 43-104.14) require attorney handling.
- **Cases involving the Nebraska Indian Child Welfare Act (§ 43-1501 et seq.).** Special procedural requirements apply that are outside the scope of forms-based products.

**Closing note for this section:** "If your situation doesn't fit one of the three scenarios above — or if any of the not-in-scope situations apply to your case — you'll need to work with an attorney for your stepparent adoption. Forms-based products won't be the right fit. For complex or contested cases, Bundy Law LLC handles full attorney representation."

This is also the right place to note: **the qualifier quiz on adoptionformsexpress.com asks about your scenario and routes you to the right product if you qualify — or tells you that you'll need full attorney representation if you don't.**

---

### Section 5 — Minor Child vs. Adult Stepparent Adoption

**Purpose:** Help the reader understand which type their case is, and the key differences.

**Length:** ~500 words, 1–2 pages

**Key points:**
- Minor-child adoption: stepchild is under 19 at the time of filing
- Adult stepparent adoption: stepchild is 19+ at the time of filing
- Key procedural differences:
  - Minor-child: home study sometimes required (depends on county); biological parent consent or pathway critical
  - Adult: no home study required; both biological parent consent AND adult adoptee consent required (the adult adoptee must consent to being adopted)
- Why adults pursue stepparent adoption: name change, inheritance/estate, legal formalization of long-existing relationships
- Both pathways available through this guide and the products on the site

---

### Section 6 — Timeline Expectations

**Purpose:** Set realistic expectations for how long this will take.

**Length:** ~400 words, 1–2 pages

**Key points:**
- Total typical timeline: 4–6 months from filing to finalized decree
- Phase 1 — Preparation (you complete forms): days to a few weeks, depending on whether DIY or DFY
- Phase 2 — Filing (your county court): same-day to a few days
- Phase 3 — Waiting for a hearing date: 6–10 weeks typically, depends heavily on county court calendar
- Phase 4 — Hearing: typically 15–30 minutes; often the easiest part
- Phase 5 — After the decree: ordering certified copies, updating birth certificate (if applicable), updating other records
- "Why does it take so long?" — court calendars, mostly. Not your case being slow.
- Counties with shorter vs. longer typical timelines (general note, not exhaustive)

---

### Section 7 — Cost Breakdown

**Purpose:** Demystify what this whole thing actually costs.

**Length:** ~400 words, 1–2 pages

**Key cost categories:**
- Court filing fee: ~$60–$90, paid directly to your county court
- Home study (if your county requires it for minor-child adoptions): ~$300–$800, paid to the home-study provider
- Background check fees (if your county requires them): typically $25–$75 per adult, varies
- Certified copies of finalized decree: ~$10–$15 each, optional but commonly needed
- Updated birth certificate (if name changed): ~$15, paid to Nebraska Vital Records
- Forms preparation:
  - DIY: $299 (forms + instructions + 1 support call) — Adoption Forms Express
  - Done-For-You: $499 (forms completed for you + 2 support calls) — Adoption Forms Express
  - Full attorney representation: typically $1,500–$5,000+ — separate attorney
- Honest framing: "Most uncontested cases stay within $400–$700 total when using DIY; $600–$900 with DFY."

---

### Section 8 — Required Forms Overview

**Purpose:** Help the reader understand what forms are involved without giving the forms away (those are the paid products).

**Length:** ~400 words, 1 page

**Key points:**
- General categories of forms required for Nebraska stepparent adoption:
  - Petition for Adoption
  - Consent forms (other biological parent, adult adoptee if applicable, sometimes adult-witnessing parent)
  - Notice of Adoption
  - Decree of Adoption (proposed)
  - Background-check authorizations (for some counties / minor-child cases)
  - County-specific supporting documents
- Brief note: the forms vary slightly based on the pathway (consent vs. deceased vs. TPR)
- Brief note: the forms vary slightly based on the county
- Where the forms come from: Adoption Forms Express provides them prepared by a licensed Nebraska adoption attorney; you can also obtain them yourself from your county court clerk (with the caveat that you'll need to figure out which forms apply to your case yourself)

---

### Section 9 — DIY vs. Attorney Representation: Which Is Right for You?

**Purpose:** Honest framing of when DIY makes sense and when full attorney representation does. This builds enormous trust because it doesn't try to push everyone toward DIY.

**Length:** ~600 words, 2 pages

**Honest framework:**

**DIY makes sense if:**
- Your case is clearly uncontested (one of the three pathways with no complications)
- The other biological parent fully agrees and will sign consent
- No custody/visitation disputes ongoing
- You're comfortable reading instructions and filling out paperwork
- Your situation is straightforward enough that a 30-minute support call can resolve any confusion

**Done-For-You makes sense if:**
- All of the DIY criteria above PLUS:
- You'd rather pay $200 more to have someone else complete the forms
- You want the security of attorney-prepared completed forms vs. you completing them yourself

**Full attorney representation is needed if:**
- Your case is contested in any way
- The other biological parent is unwilling or unreachable
- There's an ongoing custody dispute
- You want to terminate parental rights as part of this proceeding (rather than as a separate prior action)
- The pathway isn't clearly one of the three covered above
- The case crosses state lines in any meaningful way
- Your situation has any unusual element you're not sure about

**Closing note:** "If you're not sure which category you're in, take the qualifier quiz at adoptionformsexpress.com — it's designed to help you figure out which path is right for you. If you don't qualify for DIY or DFY, the quiz will tell you, and you'll know to seek full representation."

---

### Section 10 — What to Expect at the Hearing

**Purpose:** Demystify the hearing — usually the most anxiety-producing part for buyers.

**Length:** ~400 words, 1–2 pages

**Key points:**
- The hearing is typically 15–30 minutes
- Where it happens: county court (varies; could be courtroom or judge's chambers)
- Who attends: the petitioner (stepparent), the spouse, the child being adopted (depends on age), sometimes witnesses
- What the judge asks (general examples — not promises):
  - Confirmation of identity and relationship
  - Confirmation of consent (where applicable)
  - For adult adoptions: questions verifying the adoption is voluntary and not for improper purposes (creditor avoidance, immigration, etc.)
  - For minor-child adoptions: questions about the child's relationship with the stepparent
- The judge generally signs the decree at or shortly after the hearing
- Most uncontested stepparent adoption hearings are warm and brief

**Tone note:** Demystify, don't dramatize. The reader should leave this section feeling less anxious, not more.

---

### Section 11 — Common Pitfalls

**Purpose:** Pure value-add. The kind of insight only an attorney with years of adoption experience would have. This is the section that converts trust into eventual purchases.

**Length:** ~600 words, 2 pages

**Pitfalls to cover:**
- Filing in the wrong county (jurisdiction matters; usually it's where the petitioner resides)
- Missing a required form for your specific pathway (e.g., forgetting the adult adoptee consent in adult adoption cases)
- Inadequate consent — verbal agreement without signed forms; consent obtained from the wrong party
- Forgetting to order certified copies after the decree
- Forgetting to update birth certificate / SSN / other records after the name change
- Going to the hearing unprepared — don't bring kids unless asked, dress professionally, arrive early
- Confusing stepparent adoption with second-parent adoption (different process, especially in same-sex couple contexts)
- Missing a required notarization (some forms must be notarized; varies by county)
- Trusting generic "adoption forms" you find online — Nebraska has specific forms and idiosyncrasies that out-of-state forms miss

**Tone:** Direct, helpful, attorney-perspective. The reader should think "wow, this person knows what they're talking about."

---

### Section 12 — Next Steps

**Purpose:** Soft CTA back to the main funnel. The guide closes by telling the reader what to do now that they're informed.

**Length:** ~250 words, 1 page

**Content:**
- Now that you understand the process, the natural next step is to find out which path is right for your specific case
- Take the qualifier quiz at adoptionformsexpress.com — 60 seconds, tells you whether DIY, DFY, or full representation fits
- If you qualify for DIY: $299 self-serve package
- If you qualify for DFY: $499 done-for-you package
- If you don't qualify (contested case): contact Bundy Law LLC for full representation

**Tone:** Soft. Not pushy. The reader has just received substantive value; the CTA should feel like a logical next step, not a sales pitch.

---

### Section 13 — Closing from Lucrece

**Purpose:** Warm sign-off. Reinforce the relationship the guide has built.

**Length:** 1 page (~200 words)

**Voice:** First-person, Lucrece's voice — same warmth as the welcome page.

**Content:**
- Thank you for reading
- Brief reflection: stepparent adoption is one of the most meaningful legal proceedings a family can pursue
- Whatever your next step is — DIY, DFY, full attorney, or just more research — the guide hopes to have helped
- An invitation: questions about the products specifically can be sent to adoptionformsexpress@gmail.com (NOT for legal advice; that's Bundy Law's territory)
- Sign-off with name, signature image (if available), professional credentials line

---

### Back Page

**Visual treatment:**
- Adoption Forms Express logo
- Footer disclaimer (same as web pages, full text)
- Copyright line
- Contact info: adoptionformsexpress.com / adoptionformsexpress@gmail.com
- Bundy Law LLC reference for legal-advice cases
- Version and date

**Length:** 1 page

---

## 6. Total Length Audit

| Section | Pages | Words |
|---|---|---|
| Cover | 1 | ~30 |
| Welcome from Lucrece | 1 | 250–350 |
| Legal Note | 1 | ~150 |
| What Stepparent Adoption Is | 2–3 | ~600 |
| The Three Qualifying Scenarios | 3–4 | ~1,200 |
| Minor vs. Adult | 1–2 | ~500 |
| Timeline Expectations | 1–2 | ~400 |
| Cost Breakdown | 1–2 | ~400 |
| Required Forms Overview | 1 | ~400 |
| DIY vs. Attorney | 2 | ~600 |
| Hearing Expectations | 1–2 | ~400 |
| Common Pitfalls | 2 | ~600 |
| Next Steps | 1 | ~250 |
| Closing from Lucrece | 1 | ~200 |
| Back Page | 1 | ~50 |
| **TOTAL** | **~20–24** | **~5,000–6,000** |

This is a substantive guide — clearly more than a pamphlet. Long enough to feel valuable; short enough to be readable in one sitting (most readers will skim, not read every word, which is fine).

---

## 6.5. Statutory Citation Inventory

Specific Nebraska Revised Statute sections the guide will reference, organized by where they appear. This inventory exists so Lucrece can verify the legal accuracy of the statutory grounding before the guide is written.

**Verified statutes (confirmed accurate by Lucrece in spec review, May 5 2026):**

| § | Subject | Where it appears in the guide |
|---|---|---|
| § 43-101 | Children eligible for adoption — establishes both minor and adult adoption pathways; carves out the stepparent adoption exception to the general termination/relinquishment rule | Section 4 (qualifying scenarios) |
| § 43-101(2) | Adult adoption — any adult child may be adopted; if petitioner is married, spouse must join the petition | Section 5 (Minor vs. Adult); Section 8 (Required Forms Overview) |
| § 43-102 | Petition requirements — county court of petitioner's residence has jurisdiction; petition must be sworn | Section 4; Section 8 |
| § 43-103 | Hearing timing — hearing held 4–8 weeks after petition filing | Section 6 (Timeline Expectations) |
| § 43-104(1) | Consent requirements — written consents required from both biological parents (in lawful wedlock) or surviving parent if one deceased | Section 4 (Scenarios 1 and 2) |
| § 43-104(1)(a) | Minor child consent — required if over 14 years of age | Section 5 (Minor vs. Adult) |
| § 43-107(1) | Adoptive home study — discretionary in stepparent adoptions | Section 7 (Cost Breakdown); Section 8 (Required Forms Overview) |
| § 43-107(1)(b)(v) | Adult adoption home study exemption — adult adoptions exempt from home-study requirement unless court orders otherwise | Section 5 (Minor vs. Adult); Section 7 (Cost Breakdown) |
| § 43-107 (background checks) | National/FBI criminal history check via Nebraska State Patrol fingerprinting; results must be delivered directly from State Patrol to courthouse (no reuse of previous checks) | Section 7 (Cost Breakdown); Section 8 (Required Forms Overview); Section 11 (Common Pitfalls — fresh background checks required) |
| § 28-718 (referenced in § 43-107) | Child Abuse Central Registry check administered by DHHS | Section 7 (Cost Breakdown); Section 8 (Required Forms Overview) |
| § 43-109 | Decree requirements — best-interests finding required; six-month residency requirement; six-month residency does NOT apply to adult adoptions | Section 5; Section 6 (Timeline) |
| § 43-109(3) | Name change as part of adoption decree — court may decree name change for adopted child (minor or adult) as petitioners request | Section 5 (Minor vs. Adult — common reason adults pursue stepparent adoption); Section 8 (Required Forms Overview); Section 11 (Common Pitfalls — name change follow-through) |
| § 43-113 | Birth certificate update — original sealed; amended record reflects adoptive parent and any name change | Section 6 (Timeline); Section 11 (Pitfalls — name change follow-through) |
| *In re Adoption of Luke*, 263 Neb. 365 (2002) | Confirms general rule that termination/relinquishment is required for non-stepparent adoptions; stepparent adoption is statutory exception | Section 4 (background framing) |

**Statutes intentionally NOT discussed in the guide (out of scope):**

| § | Subject | Why excluded |
|---|---|---|
| § 43-104(2) | 48-hour-after-birth rule for relinquishment | Applies to newborn relinquishment, not stepparent adoption of older minors |
| § 43-104.02 to § 43-104.24 | Putative father registry; biological father notification; abandonment-related procedures | Applies to contested cases, abandonment situations, and birth-parent adoptions outside stepparent scope |
| § 43-104.14 | Notice by publication for unknown biological father whereabouts | Out of scope — diligent-search procedures require attorney handling |
| § 43-1501 et seq. | Nebraska Indian Child Welfare Act | Out of scope — special procedural requirements; explicitly mentioned only as a "this guide does not cover" callout |

**Resolved questions (May 5, 2026):**

The following statutory questions were resolved by Lucrece in spec review:

1. **Name change as part of adoption.** ✅ Confirmed: a name change can be requested as part of the adoption petition under § 43-109(3), which provides that "the court may decree such change of name for the adopted child as the petitioner or petitioners may request." This applies to both minor children and adult adoptees within an adoption proceeding. Outside of an adoption proceeding, name changes for minors and adults follow separate Nebraska name-change statutes (a parent can petition for a minor's name change; an adult can petition for their own name change without an adoption). The guide should focus only on name change AS PART OF an adoption — outside-of-adoption name changes are out of scope.

2. **Background check requirements.** ✅ Confirmed: background check requirements are NOT county-by-county; they are statewide and statutorily required under § 43-107. Two background checks are required for stepparent petitioners:
   - **National/FBI criminal history check** — petitioner gets fingerprinted at Nebraska State Patrol office; State Patrol submits to FBI; results delivered directly to the courthouse where the adoption will be finalized
   - **Child Abuse Central Registry check** — administered by DHHS through their online system (§ 43-107 references § 28-718 establishing the central registry)
   
   Important operational detail: the FBI fingerprint results must be delivered by State Patrol DIRECTLY to the courthouse — petitioners cannot bring previously-completed background check results from other contexts (employment, military, etc.). This applies even if the petitioner has a recent clean check from another source.
   
   The guide should reference § 43-107 and explain both checks. The Cost Breakdown section should reflect that fingerprinting is free at the State Patrol office, but online processing fees apply (~$15–25 per check; Lucrece to confirm exact range).

3. **Adult adoptee name change.** ✅ Confirmed: adult adoptees CAN request a name change as part of the adult stepparent adoption proceeding under § 43-109(3). The guide should mention this in Section 5 (Minor vs. Adult) as a common reason adults pursue stepparent adoption.

4. **2022 LB741 amendments.** ✅ Confirmed by Lucrece: no specific provisions from the 2022 amendments need special highlighting in the guide. The current statutory citations as quoted above already reflect post-2022 law.

5. **§ 43-166 post-adoption communication agreements.** ✅ Confirmed: this is too complex a topic to add to the guide. Omitted from scope. The guide will not mention communication agreements; if a buyer's situation involves a desire for post-adoption contact between the absent biological parent and child, that's a complex case requiring full attorney representation, not a forms-based product.

**Operational note for the spec:**

Question 2's resolution surfaces an important detail for both the guide AND the product: the petitioner cannot reuse old background-check results. This affects the DIY package's instructions (the buyer must complete the background checks specifically for the adoption, not rely on existing employer/military checks) AND the DFY package's case-prep flow (the team will need to walk the buyer through getting fresh background checks).

---

## 7. CTA Architecture Within the Guide

The guide is primarily educational, but it does need to route readers back to the products. Three CTA placements throughout, in increasing visibility:

**Soft mention 1 — Section 4 (When Stepparent Adoption Can Be Done Without an Attorney):**
"The qualifier quiz on adoptionformsexpress.com asks about your scenario and routes you to the right product if you qualify — or tells you that you'll need full attorney representation if you don't."

**Soft mention 2 — Section 9 (DIY vs. Attorney):**
"If you're not sure which category you're in, take the qualifier quiz at adoptionformsexpress.com — it's designed to help you figure out which path is right for you."

**Primary CTA — Section 12 (Next Steps):**
The main CTA. "Take the qualifier quiz to find out which package fits your case."

**Sign-off mention — Section 13 (Closing from Lucrece):**
Soft, warm, optional invitation.

The guide does NOT include direct buy-links to specific product pages. The qualifier quiz is the gate, by design — same as the web funnel. Readers must take the quiz first.

---

## 8. Email Nurture Sequence (Future Spec)

After signup, the reader receives:

- Email 1 (immediately): "Your guide is here" — PDF delivery email
- Email 2 (24 hours later): "The most important question to ask yourself" — short, value-add
- Email 3 (3 days after): "What I wish more families knew about Nebraska adoption" — Lucrece's perspective, soft CTA
- Email 4 (5 days after): "DIY isn't right for everyone — and that's okay" — honest framing
- Email 5 (7 days after): "Ready to find out what path fits your case?" — direct CTA to the quiz
- Email 6 (10 days after — optional): "Last call: your free quiz access" — urgency-light final nudge
- Email 7 (14 days after — optional): "Talking to attorneys: a checklist for the families who need full representation" — value-add for the non-buyers; positions Bundy Law

**Detailed email copy is not in this doc** — it gets its own working doc when we move to that phase. But the sequence outline is locked here for planning purposes.

---

## 9. Landing Page Spec (Future)

The `/starter-guide/` landing page is its own deliverable. Brief outline:

- Stripped nav (similar to checkout pages)
- Hero: "The Nebraska Stepparent Adoption Starter Guide" + email capture form
- "What's inside" — 4–6 key things readers will learn
- Lucrece signature block (same as homepage and product pages)
- 2–3 testimonials (potentially from email-nurture-sequence subscribers who eventually purchased)
- Footer

**Detailed landing page spec is not in this doc** — it gets its own sister doc when we move to that phase. Probably named `lead-magnet-landing-page-v1.md`.

---

## 10. Email Platform — Open Decision

Per master doc Open Decision #11: ConvertKit vs. MailerLite. Need to decide before email sequence build.

**Recommendation framing for that decision:**
- ConvertKit: better for creators, more intuitive sequences, slightly more expensive
- MailerLite: better value, capable enough for this scale, free tier accommodates startup phase
- Both integrate with WordPress and ThriveCart natively

This decision is NOT blocking the PDF or the landing page — those can move forward in parallel. Lock the platform choice before email sequence build session.

---

## 11. Wiring (Final Phase)

Once PDF + email sequence + landing page + platform are all built:

1. Replace 4 stubs in homepage HTML (homepage hero, homepage final CTA, homepage FAQ footnote, footer Services link) — change `href="#"` to `href="/starter-guide/"`
2. Update master doc Section 2 (Site Architecture) — landing page status to 🔵 Built
3. Update master Open Decision #11 (email platform) — Resolved with chosen platform
4. End-to-end test: signup on landing page → confirm PDF delivery → confirm email 1 sends → confirm sequence triggers correctly

---

## 12. Open Questions / Decisions Needed

| # | Question | Status | Notes |
|---|---|---|---|
| 1 | Email platform choice | Open | ConvertKit vs. MailerLite — decide before email sequence build |
| 2 | Specific form names per pathway | Open | The forms vary slightly by pathway — Lucrece to confirm exact lists for the Required Forms Overview section |
| 3 | County-specific home study requirements | Open | The Cost Breakdown section mentions home study "if your county requires it" — Lucrece to confirm which Nebraska counties typically require it for minor-child cases |
| 4 | Cost ranges for home studies | Open | $300–$800 range listed; Lucrece to confirm or refine |
| 5 | PDF design treatment | Open | Will the PDF be designed by Lucrece/Tyler in Canva or a similar tool, or by a designer? Affects deliverable timeline |
| 6 | Lucrece's signature image | Open | Used in the closing page; need a digital signature scan or signature font |
| 7 | The guide's "current as of [date]" reference | Open | The guide should reference a "this guide is current as of [date]" line in the legal note — set the date when the PDF goes live |
| 8 | Translation/Spanish version | Open | Future consideration: a substantial Spanish-speaking audience exists in Nebraska. Possibly a v2 deliverable. |

---

## 13. Change Log

| Date | Change | Author |
|---|---|---|
| 2026-05-05 | v1.3 — **All five open statutory questions resolved.** Lucrece confirmed answers to the open questions in Section 6.5: (1) name change can be requested as part of an adoption petition under § 43-109(3) for both minor and adult adoptees; outside-of-adoption name changes are out of scope for the guide; (2) background check requirements are statewide (not county-by-county) under § 43-107 — two checks required: FBI/national criminal history check via Nebraska State Patrol fingerprinting, and Child Abuse Central Registry check via DHHS (referenced in § 28-718); FBI fingerprint results must be delivered directly from State Patrol to the courthouse (no reuse of prior checks from employment/military); (3) adult adoptees can request name change as part of adult stepparent adoption — common reason adults pursue this; (4) no specific 2022 LB741 amendments need special highlighting; current statutory citations already reflect post-2022 law; (5) § 43-166 post-adoption communication agreements explicitly OMITTED from guide scope — too complex; cases needing this require full attorney representation. Statutory Citation Inventory in Section 6.5 expanded to include § 43-107 (background checks), § 28-718 (Child Abuse Central Registry), and § 43-109(3) (name change). New operational note flagged: petitioners cannot reuse old background-check results — affects DIY package instructions and DFY case-prep flow. The spec is now ready for content writing — all legal framing locked, all statutes verified by Lucrece, no open questions remaining. | Claude / Lucrece |
| 2026-05-05 | v1.2 — **Statutory grounding + abandonment carve-out + Scenario 3 reframing.** Following Lucrece's research review, three substantive corrections were made: (1) Section 4 now grounded in specific Nebraska Revised Statute citations (§§ 43-101 to 43-115), with *In re Adoption of Luke* (263 Neb. 365, 2002) cited as the controlling Nebraska Supreme Court case confirming the stepparent adoption exception to the general termination/relinquishment rule. Each of the three qualifying scenarios now references the specific statutory subsection that authorizes it. (2) New "What is NOT in scope" subsection added to Section 4, explicitly carving out abandonment cases, contested termination cases, out-of-state cases, unknown-whereabouts cases, and ICWA cases as requiring full attorney representation. The abandonment carve-out is critical — Lucrece confirmed Nebraska courts appoint a guardian ad litem in abandonment cases, making them too complex for forms-based products. (3) Scenario 3 reframed from "rights have been terminated" to "rights have been previously terminated through a separate court action" — emphasizing that this is a *prior, completed* termination documented by court records, NOT termination as part of the current proceeding. (4) Section 3 safe/unsafe table updated with statutory examples replacing generic ones; explicit unsafe example added warning against using the forms in abandonment cases. (5) New Section 6.5 (Statutory Citation Inventory) added, tracking every statutory citation the guide will use, plus a list of intentionally-excluded statutes (e.g., § 43-104(2) which applies only to newborn relinquishment, not stepparent adoption of older minors), plus 5 open questions about additional statutes that may need to be added. The qualifier quiz was confirmed by Lucrece to already screen out abandonment cases — quiz alignment is good. | Claude / Lucrece |
| 2026-05-05 | v1.1 — **Legal accuracy correction.** Reframed Section 4 from "The Three Pathways" (which incorrectly implied this was a description of Nebraska adoption law) to "When Nebraska Stepparent Adoption Can Be Done Without Full Attorney Representation" (which correctly frames the three scenarios as the narrow product-qualifying criteria they actually are). The general rule in Nebraska is that adoptions require attorney representation; the three scenarios (consent / deceased / terminated parental rights) are the specific exceptions where a forms-based product can work. Section 4 now explicitly opens with this framing. UPL safe/unsafe table in Section 3 also updated to remove the inaccurate "three pathways" example. CTA architecture reference and table of contents reference updated to match. This correction was caught by Lucrece in spec review before any content was written — preventing the inaccuracy from propagating into 5,000+ words of guide content. | Claude / Lucrece |
| 2026-05-01 | v1.0 — Initial lead-magnet project doc drafted. Locks the strategic frame (top-of-funnel awareness builder), format (PDF + email sequence), title ("The Nebraska Stepparent Adoption Starter Guide"), audience scope (both minor-child and adult), voice (Lucrece intro/sign-off + neutral instructional body), UPL framing, full section-by-section structure (13 sections + cover + back page, ~5,000–6,000 words across ~20 pages), CTA architecture, and outlines email nurture sequence and landing page as future sister-doc deliverables. Spec is build-ready: next session writes the actual content of the PDF guide. | Claude / Lucrece |
