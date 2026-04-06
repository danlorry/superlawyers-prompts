# Chapter 5 — Contract Analysis

> Run these prompts in sequence: first-pass risk scan, then deep dives on HIGH items, then consistency check, then gap analysis. Never skip the gap analysis.

---

## Prompt 1 — First-Pass Risk Scan

**Verify:** Claude's "market standard" characterizations against your firm's recent deal experience.

```
CONTEXT: I represent the [Seller/Buyer/Tenant/Landlord] in a
[describe agreement type]. [Describe parties briefly.]
Transaction value: $[X]M. Governing law: [STATE].
I am preparing for [describe next milestone — negotiation call, closing, etc.].

The full text of the agreement is pasted below.

TASK: Analyze this agreement from my client's perspective:

1. TOP RISKS (prioritized, highest risk first):
   For each risk item:
   - The specific provision (section reference and brief description)
   - Why it creates risk for my client
   - Whether it deviates from market standard for this transaction type
   - Severity: HIGH / MEDIUM / LOW

2. MISSING PROTECTIONS:
   Standard protections for my client's position that are absent.
   - What is typically included
   - Why it matters
   - Priority: SHOULD FIGHT FOR / NICE TO HAVE

3. INTERNAL INCONSISTENCIES:
   Conflicting provisions, defined terms used inconsistently,
   cross-references that do not resolve correctly.

4. ONE-SIDED PROVISIONS:
   Anything unusually favorable to the other party beyond
   typical leverage for a transaction of this type.

FORMAT: Organized by the four categories. Section references throughout.
For HIGH severity risks, include suggested alternative language.

CONSTRAINTS: Flag when uncertain whether a provision is market standard.
Note any area where the analysis depends on facts not provided.

[PASTE FULL AGREEMENT TEXT HERE]
```

---

## Prompt 2 — Deep Dive on a Flagged Provision

```
CONTEXT: Continuing from the previous analysis of [agreement type].
You flagged [specific provision] as HIGH severity.

TASK: Complete analysis of [specific provision]:

1. WHAT THE AGREEMENT SAYS: Summarize the key terms as drafted.

2. MARKET STANDARD COMPARISON: For a [describe transaction] of
   this size and type, what is typical? What is the normal range?

3. MY CLIENT'S EXPOSURE: What is the maximum exposure under the
   current draft? What scenarios trigger the worst outcome?

4. NEGOTIATING POSITIONS: What are the strongest arguments for
   my client to [improve/modify] this provision? What is the
   other side's likely response?

5. SUGGESTED LANGUAGE: Draft alternative language that represents
   a reasonable ask for a transaction of this type.

CONSTRAINTS: Flag where market practice varies significantly and
my client's specific situation would determine the right position.
```

---

## Prompt 3 — Consistency Check

```
CONTEXT: I am reviewing [agreement type] from [client's] perspective.
Full text pasted below.

TASK: Consistency check only — not risk assessment:

1. DEFINED TERM AUDIT:
   - Terms used but not defined
   - Terms defined but never used
   - Terms used inconsistently with their definition

2. CROSS-REFERENCE CHECK:
   - References pointing to wrong sections
   - Circular references
   - References to exhibits or schedules not attached

3. CONFLICTING PROVISIONS:
   Two provisions imposing conflicting obligations on the same issue.

FORMAT: List format. Section references for every item.

CONSTRAINTS: Structural and logical consistency only.
Risk assessment was covered separately.

[PASTE FULL AGREEMENT TEXT HERE]
```

---

## Prompt 4 — Gap Analysis

```
CONTEXT: I am reviewing [agreement type]. [Describe parties and transaction.]
Full text pasted below.

TASK: Identify what is missing — protections typically present in
a [transaction type] of this size that do not appear to be included.

For each missing item:
- What the provision is
- Why it is typically included
- Why it matters for my client specifically
- Priority: SHOULD INSIST / WORTH REQUESTING / NICE TO HAVE

Categories to check: [customize for transaction type, e.g.:]
1. Closing conditions protecting my client
2. Post-closing covenants
3. Representations from the other side
4. Indemnification for pre-closing liabilities
5. Specific performance remedies
6. [Other relevant categories]

CONSTRAINTS: Flag uncertainty about whether an absence is intentional
or an oversight.

[PASTE FULL AGREEMENT TEXT HERE]
```
