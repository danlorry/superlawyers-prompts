# Startup and Venture Prompts

> Fast-moving area where market standard evolves quickly. Claude's training on NVCA model documents and standard Silicon Valley terms is generally reliable. Verify current market terms for round size and investor type — what was standard in 2022 may not be standard now.

---

## Prompt 1 — Term Sheet Analysis (Founder-Side)

**Use when:** Reviewing a VC term sheet on behalf of a founder.
**Verify:** Current market terms for round size and stage. Liquidation preference math against the specific cap table. Any unusual control provisions.

```
CONTEXT: I represent the founder of a [describe company — stage,
industry, ARR/traction]. The company is raising a Series [A/B/Seed]
of $[X]M. The lead investor is [describe — tier-1 VC, strategic,
corporate]. The term sheet is pasted below.

TASK: Analyze this term sheet from the founder's perspective:

1. ECONOMICS — WHAT THE FOUNDER IS REALLY GIVING UP:
   - Pre-money valuation and resulting ownership dilution
   - Option pool: is a new option pool required pre-closing?
     What is the dilutive impact if so?
   - Liquidation preference: participating or non-participating?
     Multiple? Run the math: at what exit price does the preference
     matter vs. a straight pro-rata split?
   - Anti-dilution: weighted average or full ratchet?
     Broad-based or narrow-based weighted average?
     Flag if full ratchet — this is founder-unfavorable.

2. CONTROL — WHAT THE INVESTOR CAN BLOCK:
   - Board composition: who controls the board?
   - Protective provisions (investor veto rights): list every
     action that requires investor approval. Flag any that are
     broader than NVCA market standard.
   - Drag-along: who can trigger it? What threshold?
     Are founders protected?
   - Information rights: what must be provided and how often?

3. FOUNDER PROTECTIONS — WHAT IS MISSING:
   - Is there a pay-to-play provision? How does it work?
   - Are there founder vesting acceleration provisions
     (single trigger, double trigger)?
   - Is there a right of first refusal on founder share sales?
   - Are founder shares subject to co-sale rights?
   - Any provisions that could force founders out?

4. RED FLAGS — NON-STANDARD TERMS:
   Identify any provision that deviates significantly from
   NVCA model documents or current market standard for a
   Series [A/B/Seed] of this size. For each:
   - What it says
   - Why it is non-standard
   - What the founder should push back on

5. NEGOTIATING PRIORITIES:
   If the founder can only change three things, what should they be?
   Rank by impact on founder outcomes in realistic exit scenarios.

FORMAT: Organized by the five sections. Run actual liquidation
preference math in section 1 using the valuation in the term sheet.
Flag RED FLAGS prominently.

CONSTRAINTS: Base market standard comparisons on NVCA model documents
and typical Series [A/B/Seed] terms. Flag any area where current
market may have shifted from historical norms.

[PASTE TERM SHEET HERE]
```

---

## Prompt 2 — Shareholders Agreement / Founders Agreement Review

**Use when:** Reviewing or drafting a founders' agreement or shareholders agreement at company formation.
**Verify:** IP assignment completeness. Vesting terms against the founders' actual situation. State corporate law requirements.

```
CONTEXT: I am reviewing a founders' agreement / shareholders agreement
for a [Delaware C-corp / LLC] being formed by [X] founders.
The founders: [describe each founder's role, contribution, and
proposed equity split]. The company is pre-revenue and pre-funding.
The agreement is pasted below [or: please draft one based on
the parameters below].

[IF REVIEWING — paste agreement]
[IF DRAFTING — provide these parameters:]
- Founders and equity splits: [list]
- Vesting: [proposed schedule]
- Decision-making: [unanimous / majority / designated roles]
- IP assignment: [describe each founder's relevant prior IP]
- Transfer restrictions: [describe]

TASK: [Review / Draft] this agreement:

1. EQUITY AND VESTING:
   - Is the equity split documented clearly?
   - Vesting schedule: standard 4-year / 1-year cliff?
     Any acceleration provisions?
   - Is there a mechanism to address a founder departure before
     vesting is complete? (Repurchase right, good leaver/bad leaver)
   - What happens to unvested shares if a founder is terminated
     vs. resigns vs. dies?

2. DECISION-MAKING AND DEADLOCKS:
   - What decisions require unanimous consent?
   - What decisions can be made by majority?
   - Is there a deadlock resolution mechanism?
   - Who has authority to bind the company day-to-day?

3. IP ASSIGNMENT:
   - Does every founder assign all relevant IP to the company?
   - Is prior IP that the founder is NOT assigning clearly
     carved out and described?
   - Is the assignment broad enough to cover work done before
     formal company formation?
   - Does it survive the agreement?

4. TRANSFER RESTRICTIONS:
   - Right of first refusal on founder share transfers
   - Co-sale rights (tag-along)
   - Drag-along rights — threshold and mechanics
   - Lock-up period before any transfers are permitted

5. DEPARTURE SCENARIOS:
   For each likely departure scenario, what happens?
   - Voluntary resignation
   - Termination for cause
   - Termination without cause
   - Death or disability
   - Acquisition of the company

FORMAT: Organized by the five sections. For any missing provision,
flag whether it is CRITICAL / IMPORTANT / STANDARD to include.

CONSTRAINTS: Flag any provision that creates risk if the company
raises institutional funding — investors will review this document
and flag anything non-standard.
```

---

## Prompt 3 — SAFE / Convertible Note Analysis

**Use when:** Reviewing a SAFE or convertible note from either investor or company perspective.
**Verify:** Current YC SAFE terms if using a YC-form SAFE. Cap and discount math against the anticipated Series A valuation.

```
CONTEXT: I represent the [Company / Investor] in connection with
a [SAFE / convertible note] investment. Amount: $[X].
[If SAFE:] Valuation cap: $[X]M. Discount: [X]%. [MFN / no MFN].
[If note:] Interest rate: [X]%. Maturity: [X] months.
Conversion discount: [X]%. Valuation cap: $[X]M.
Document pasted below.

TASK: Analyze this [SAFE / note]:

1. CONVERSION MECHANICS:
   - When does it convert? What triggers conversion?
   - How is the conversion price calculated?
     Walk through the math with the cap and discount:
     At what Series A valuation does the cap apply vs. the discount?
   - What happens on a change of control before conversion?
   - What happens at maturity (for notes) if no conversion event?

2. ECONOMICS FOR THE INVESTOR:
   - What is the effective pre-money valuation the investor is
     paying if the next round is at $[X]M?
   - What ownership percentage results from conversion at
     various Series A valuations: $[X]M, $[X]M, $[X]M?
   - Is the MFN provision meaningful given the company's
     current funding stage?

3. ECONOMICS FOR THE COMPANY:
   - What is the dilutive impact at various outcomes?
   - Are there any provisions that create unexpected dilution
     (e.g., option pool requirements at conversion)?
   - If multiple SAFEs/notes: how do they interact?

4. RISKS FOR [COMPANY / INVESTOR]:
   - What scenarios create problems for my client?
   - Any provisions that are non-standard vs. YC form SAFE
     or standard convertible note terms?

5. NEGOTIATING POINTS:
   If my client could change two or three terms, what would
   have the most impact on their economics or risk profile?

FORMAT: Organized by the five sections. Show the conversion
math explicitly in sections 1 and 2 using real numbers.

CONSTRAINTS: Compare to YC standard SAFE form where applicable.
Flag any deviation from standard terms.

[PASTE DOCUMENT HERE]
```

---

## Prompt 4 — IP Assignment and Work-for-Hire Audit

**Use when:** Conducting IP due diligence on a startup before an investment or acquisition.
**Verify:** Employment agreements and contractor agreements against the actual IP created. Any open source license obligations.

```
CONTEXT: I am conducting IP due diligence on [Company] in connection
with a [Series A investment / acquisition]. The company's core IP is:
[describe — software, patents, trade secrets, content].
The company has [X] employees and has used [X] contractors.

I have reviewed the following documents:
[List what you have: employment agreements, contractor agreements,
IP assignment agreements, any patent filings, etc.]

The key documents are pasted below.

TASK: Assess the completeness of the company's IP ownership:

1. EMPLOYEE IP ASSIGNMENT:
   - Do all employment agreements contain adequate IP assignment
     provisions?
   - Are there any employees who worked on core IP before their
     employment agreement was signed?
   - Are there any employees in states with IP assignment limits
     (CA, WA, MN, IL, NC, DE) whose agreements may not be
     fully enforceable?
   - Are there any employees who have not signed an IP assignment?

2. CONTRACTOR IP ASSIGNMENT:
   - Do all contractor agreements contain work-for-hire language
     AND a backup IP assignment?
     (Work-for-hire alone is not sufficient for software)
   - Are there contractors who contributed to core IP without
     a written agreement?
   - Are there contractors in other countries where the IP
     assignment analysis differs?

3. FOUNDER IP:
   - Have all founders assigned their pre-formation IP to the company?
   - Is the assignment of pre-formation IP adequately documented?
   - Are there any founder IP disputes or competing claims?

4. OPEN SOURCE:
   - Has the company used any open source components in its core product?
   - What licenses apply? (GPL / LGPL / MIT / Apache)
   - Do any copyleft licenses (GPL) create an obligation to
     open-source the company's proprietary code?

5. GAPS AND REMEDIATION:
   List every IP ownership gap identified. For each:
   - The risk it creates
   - Whether it can be remediated before closing
   - How to remediate it (what documents are needed)
   - Severity: DEAL-BREAKER / SIGNIFICANT / MANAGEABLE

FORMAT: Organized by the five sections. Be specific about which
employees or contractors create which gaps.

CONSTRAINTS: Flag any gap that a sophisticated investor or acquirer
would treat as a material issue. Note any area where I need to
review the actual underlying documents.

[PASTE RELEVANT DOCUMENTS HERE]
```

---

## Prompt 5 — Equity Compensation Plan Review

**Use when:** Reviewing or advising on a startup's equity compensation plan and option grants.
**Verify:** 409A valuation currency. ISO vs. NSO treatment under current tax law. State securities law compliance for option grants.

```
CONTEXT: I am advising [Company] on its equity compensation plan.
Company stage: [describe — pre-seed, seed, Series A, etc.].
Current 409A valuation: $[X] per share (dated [date]).
Common stock outstanding: [X] shares. Option pool: [X] shares.

TASK: Review the equity compensation structure:

1. PLAN MECHANICS:
   - Is the option pool size adequate for the company's
     hiring plans for the next [12-18] months?
   - Is the exercise price set at or above the current 409A FMV?
     Flag if the 409A is more than 12 months old — may need refresh.
   - Standard 4-year vesting / 1-year cliff: is it in place?
   - Post-termination exercise window: 90 days is standard.
     Flag if shorter (bad for employees) or longer (tax implications).

2. ISO vs. NSO ANALYSIS:
   - Are grants structured as ISOs where possible?
   - ISO eligibility: employees only (not contractors or board members)
   - ISO $100,000 annual limit: are any grants exceeding this limit?
   - Early exercise (83(b) election): is it available? Is it
     advisable for founders and early employees?

3. ACCELERATION PROVISIONS:
   - Is there single-trigger acceleration? (Change of control alone)
   - Is there double-trigger acceleration? (Change of control +
     termination)
   - Who has acceleration and at what percentage?
   - Flag: single-trigger full acceleration is often a deal issue
     in acquisitions.

4. EQUITY GRANT PROCESS:
   - Are grants being approved by the board before they are
     communicated to employees?
   - Is the company maintaining a proper cap table with all grants?
   - Are grant agreements being signed before employees begin
     vesting?
   - Any grants that were promised but not documented?

5. ISSUES TO ADDRESS BEFORE NEXT ROUND:
   What equity compensation issues should be cleaned up before
   the company raises its next institutional round?
   Priority: MUST FIX / SHOULD FIX / OPTIONAL

FORMAT: Organized by the five sections. Flag any tax or securities
law issue prominently.

CONSTRAINTS: Flag any area where I should involve a tax advisor.
Note that option grant advice has significant tax implications
and this analysis is a starting point for a fuller review.
```
