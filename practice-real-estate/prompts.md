# Real Estate Prompts

> Relatively stable doctrinal landscape with significant state-specific variation in recording requirements, title standards, and disclosure obligations. Use Claude for framework and document review. Always verify current title standards and recording requirements in primary sources for the specific jurisdiction.

---

## Prompt 1 — Purchase Agreement Review (Buyer-Side)

**Use when:** Reviewing a residential or commercial purchase agreement on behalf of the buyer.
**Verify:** State-specific disclosure requirements. Due diligence period rules. Financing contingency mechanics under state law.

```
CONTEXT: I represent the Buyer in a [residential / commercial]
real estate transaction. Property: [describe — type, location, price].
Seller: [describe — individual / entity / bank / estate].
Governing law: [STATE]. The purchase agreement is pasted below.

TASK: Review from the Buyer's perspective:

1. DUE DILIGENCE PROTECTIONS:
   - Due diligence period: duration, what it covers, termination right
   - Inspection contingency: scope, who pays, repair negotiation process
   - Title contingency: what title defects allow Buyer to terminate?
   - Survey contingency (if applicable)
   - Environmental contingency (if commercial)
   - Is the due diligence period adequate for this transaction type?

2. FINANCING CONTINGENCY:
   - Is there a financing contingency? If yes:
     - Loan amount, rate cap, type
     - Deadline for commitment letter
     - What happens if financing fails — deposit returned or forfeited?
   - If no financing contingency: what is Buyer's exposure?

3. DEPOSIT AND EARNEST MONEY:
   - Amount and timing of deposit(s)
   - Is deposit refundable and under what conditions?
   - Who holds the deposit and in what type of account?
   - What triggers forfeiture?

4. REPRESENTATIONS AND WARRANTIES:
   - What does Seller represent about the property?
   - Are representations limited to Seller's knowledge?
   - What is the survival period after closing?
   - Are there adequate representations about:
     - Title and encumbrances
     - Permits and code compliance
     - Litigation and environmental issues
     - HOA status and assessments (if applicable)
     - Tenants and leases (if commercial)

5. MISSING BUYER PROTECTIONS:
   Standard buyer protections for a [residential/commercial]
   transaction in [STATE] that are absent.
   Priority: SHOULD INSIST / WORTH REQUESTING / NICE TO HAVE

FORMAT: Organized by the five categories. Section references throughout.
For HIGH risk items, include suggested alternative language.

CONSTRAINTS: Flag any provision that may not comply with [STATE]
real estate law. Flag any non-standard risk allocation.

[PASTE AGREEMENT HERE]
```

---

## Prompt 2 — Title Commitment Review

**Use when:** Reviewing a title commitment or preliminary title report on behalf of a buyer or lender.
**Verify:** Specific exceptions against the actual underlying documents. State title standards for what constitutes a marketable title objection.

```
CONTEXT: I am reviewing a title commitment / preliminary title report
for a [residential / commercial] property in [STATE / COUNTY].
Transaction: [describe — purchase price, buyer, seller, lender if any].
The title commitment is pasted below.

TASK: Review the title commitment:

1. SCHEDULE A — BASIC INFORMATION:
   - Is the legal description consistent with the purchase agreement?
   - Is the vested owner consistent with who is selling?
   - Is the proposed insured correctly identified?
   - Is the coverage amount adequate?

2. SCHEDULE B-I — REQUIREMENTS:
   List each requirement and flag:
   - Requirements that are standard and easily satisfied
   - Requirements that need action before closing and by whom
   - Requirements that may be difficult or impossible to satisfy
   - Any requirement that is unusual for this transaction type

3. SCHEDULE B-II — EXCEPTIONS:
   For each exception, analyze:
   - What it is (easement, covenant, lien, encumbrance)
   - Whether it materially affects the Buyer's intended use
   - Whether it should be objected to under the purchase agreement
   - Whether it can be insured over or deleted
   Priority: OBJECT / ACCEPTABLE / STANDARD

4. SPECIFIC ISSUES TO FLAG:
   - Any mechanics' liens or potential liens from recent work
   - Any boundary or survey issues suggested by the exceptions
   - Any HOA-related exceptions and what they mean for the buyer
   - Any environmental liens or notices
   - Any open permits or code violations

5. PRE-CLOSING ACTIONS:
   What needs to happen before closing to clean up title?
   Who is responsible for each item?

FORMAT: Organized by the five sections. Be specific about
exception numbers when referencing Schedule B-II items.

CONSTRAINTS: Flag any exception that requires review of the
underlying document before you can fully assess its impact.
Note that I will need to review the actual underlying documents
for any materially unusual exceptions.

[PASTE TITLE COMMITMENT HERE]
```

---

## Prompt 3 — Commercial Lease Review (Tenant-Side)

**Use when:** Reviewing a commercial lease on behalf of a tenant.
**Verify:** State-specific landlord-tenant law. Local zoning for permitted use. CAM audit rights under state law.

```
CONTEXT: I represent the Tenant in a commercial lease negotiation.
Tenant: [describe business — type, size, growth stage].
Property: [describe — type, size, location, new/existing building].
Landlord: [describe — institutional / private / developer].
Proposed term: [X] years. Base rent: $[X]/sq ft [NNN/gross].
Governing law: [STATE]. The landlord's form lease is pasted below.

TASK: Review from the Tenant's perspective:

1. ECONOMIC TERMS — RISKS AND HIDDEN COSTS:
   - Rent escalation: how does it compound over the full term?
     Calculate total rent obligation over the lease term.
   - CAM: what is included in CAM? What is excluded?
     Is there a CAM cap? Does it apply to all CAM or only
     controllable CAM? What audit rights does Tenant have?
   - Operating expense pass-throughs: what expenses can Landlord
     pass through beyond CAM?
   - What is Tenant's realistic total occupancy cost per year?

2. USE AND EXCLUSIVITY:
   - Permitted use clause: is it specific enough to protect Tenant's
     business? Is it flexible enough for business evolution?
   - Is there an exclusivity provision? If yes, how is it enforced?
     What remedies does Tenant have for violation?
   - If no exclusivity: should Tenant request one?

3. ASSIGNMENT AND SUBLETTING:
   - Can Tenant assign or sublease? Under what conditions?
   - Is Landlord consent required? What standard applies?
   - Does Landlord have a recapture right?
   - What happens on a change of control of Tenant's business?
     (Critical for startups or any business that may be acquired)

4. LANDLORD DEFAULT AND TENANT REMEDIES:
   - What constitutes Landlord default?
   - What are Tenant's remedies? Is self-help available?
   - What happens if Landlord fails to deliver possession?
   - What is the rent abatement right if the space becomes
     unusable (casualty, condemnation, Landlord interference)?

5. EXIT RIGHTS AND FLEXIBILITY:
   - Is there a termination right? Under what conditions?
   - What are the holdover consequences? Is the rate punitive?
   - Is there a contraction or expansion right?
   - What happens at the end of the term — renewal options,
     market rate determination process?

6. MISSING TENANT PROTECTIONS:
   Standard tenant protections for a [retail/office/industrial]
   lease of this size that are absent.

FORMAT: Organized by the six categories. Calculate the total
rent obligation in section 1. Flag any provision that significantly
deviates from market standard for this lease type.

CONSTRAINTS: Flag any provision where [STATE] landlord-tenant law
has specific requirements I should verify.

[PASTE LEASE HERE]
```

---

## Prompt 4 — Due Diligence Checklist (Commercial Acquisition)

**Use when:** Preparing for due diligence on a commercial property acquisition.
**Practice area:** Commercial real estate.

```
CONTEXT: My client is acquiring a [describe property type — office,
retail, industrial, multifamily] property for $[X]M.
The property: [describe — age, size, tenancy, location, condition].
Closing is targeted for [X] weeks from now.

TASK: Generate a comprehensive due diligence checklist organized
by category. For each item:
- What we need to obtain or verify
- Who typically provides it (Seller, title company, government, etc.)
- Why it matters for this specific transaction
- Priority: CRITICAL (must have before closing) / IMPORTANT /
  STANDARD

Categories to cover:

1. TITLE AND SURVEY
2. PHYSICAL CONDITION
   (including environmental, structural, mechanical, ADA)
3. ZONING AND PERMITS
4. TENANCY AND LEASES
   (for income-producing properties)
5. FINANCIAL
   (operating statements, tax bills, utility costs, CAM reconciliations)
6. LEGAL AND LITIGATION
7. INSURANCE
8. FINANCING-RELATED
   (if acquisition financing)

FORMAT: Checklist format organized by category with
priority designation for each item.

CONSTRAINTS: Flag any category where the specific property type
creates unusual due diligence requirements. Note any item where
[STATE] law creates specific requirements or disclosures.
```

---

## Prompt 5 — Easement Analysis

**Use when:** Analyzing an easement that affects a property being acquired or developed.
**Verify:** Easement terms against the actual recorded document. State law on easement scope and termination.

```
CONTEXT: I am analyzing an easement that affects [describe property].
My client is the [owner / buyer / developer] of the property.
The easement: [describe — type, who holds it, general purpose].
The full easement document is pasted below.

TASK: Analyze this easement:

1. SCOPE AND LOCATION:
   - What is the easement holder permitted to do?
   - Where exactly is the easement located on the property?
   - Is the location described with sufficient precision?
   - Are there any limitations on the easement holder's activities?

2. IMPACT ON MY CLIENT'S INTENDED USE:
   - My client intends to [describe intended use].
   - Does the easement materially interfere with that use?
   - Are there any activities my client cannot do because
     of the easement?
   - Does the easement affect the buildable area of the property?

3. MAINTENANCE AND LIABILITY:
   - Who maintains the easement area?
   - Who is liable for injuries or damage in the easement area?
   - Are there indemnification obligations?

4. TERMINATION AND MODIFICATION:
   - Under what conditions can the easement be terminated?
   - Can it be modified? By whom and how?
   - Does it run with the land — will it bind future owners?

5. RISKS AND RECOMMENDATIONS:
   - What are the primary risks this easement creates?
   - Should my client object to this easement under the
     purchase agreement?
   - Can it be insured over? Should we request title insurance
     coverage for specific risks?
   - Is any modification or clarification worth negotiating
     before closing?

FORMAT: Organized by the five sections. Specific document
references throughout.

CONSTRAINTS: Flag any provision that is ambiguous and could
lead to a dispute between the property owner and easement holder.
Note if the easement appears to have been drafted in a way
that favors the easement holder.

[PASTE EASEMENT DOCUMENT HERE]
```
