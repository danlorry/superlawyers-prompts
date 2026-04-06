# Chapter 4 — The First Draft in Fifteen Minutes

> Claude drafts. You review. Never send a Claude-generated first draft to a client without applying the five-step review protocol in the book.

---

## Prompt 1 — The Mutual NDA

**Use when:** Drafting a standard mutual non-disclosure agreement.
**Level:** 1 — Standard form. Review time: 20-30 minutes.
**Verify:** Carve-outs, survival periods, governing law requirements.

```
CONTEXT: I am drafting a mutual NDA for two [describe parties, e.g.,
technology companies] exploring a potential [describe relationship].
Both parties may share confidential information with the other.
Governing law: [STATE]. [Any specific venue or dispute resolution preference.]

TASK: Draft a mutual NDA that includes:

CORE PROVISIONS:
- Definition of Confidential Information (broad, covering business,
  technical, financial, and personnel information; excluding standard
  carve-outs: public domain, prior knowledge, independent development,
  required disclosure)
- Obligations of receiving party: standard duty of care, need-to-know
  distribution only, no reverse engineering or competitive use
- Term: [X] years from execution; survival of obligations: [X] years
- Return/destruction on request within [X] business days
- No license granted by disclosure

SPECIFIC REQUIREMENTS:
- Mutual structure (both parties can be disclosing and receiving)
- Equitable relief provision
- No-warranty clause on accuracy of information disclosed
- Standard boilerplate: entire agreement, amendments in writing,
  severability, counterparts, no waiver

FORMAT: Complete agreement ready for review. Numbered sections.
Defined terms in caps. Signature block for two authorized
signatories per party.

CONSTRAINTS: Flag any assumption about the parties' intent that I
should confirm before finalizing. Flag any clause where [STATE] law
has specific requirements I should verify. Do not include provisions
not listed above without flagging them.
```

---

## Prompt 2 — The Service Agreement

**Use when:** Drafting a standard services agreement between two commercial parties.
**Level:** 1 — Standard form. Review time: 20-30 minutes.
**Verify:** Scope of services, liability cap amount, IP assignment, auto-renewal terms.

```
CONTEXT: I am drafting a service agreement between [SERVICE PROVIDER
description] and [CLIENT description]. The services to be provided:
[describe services]. Governing law: [STATE].

ENGAGEMENT STRUCTURE:
- Term: [X] months, [auto-renewing / not renewing] unless terminated
  on [X] days notice
- Fee: [describe fee structure — retainer/hourly/project]
- Out-of-pocket expenses: [reimbursable with prior approval above $X /
  not reimbursable]
- Termination for convenience: [either party / client only], [X] days
  written notice
- Termination for cause: material breach, [X] days cure period

IP AND CONFIDENTIALITY:
- Work product ownership: [Client / Service Provider / jointly owned]
- Pre-existing IP of Service Provider: [licensed / retained]
- Confidentiality: [mutual / one-way], [X]-year survival

LIABILITY:
- Liability cap: [describe cap — e.g., fees paid in preceding 3 months]
- Exclusion of consequential damages: [mutual / one-way]
- Indemnification: [describe scope]

FORMAT: Complete agreement, numbered sections. Include exhibit
placeholder for description of services.

CONSTRAINTS: Flag assumptions. Flag any provision where [STATE] law
has specific requirements I should verify.
```

---

## Prompt 3 — The Commercial Lease (Landlord Form)

**Use when:** Drafting a landlord-favorable commercial lease first draft.
**Level:** 2 — Complex. Review time: 60-90 minutes.
**Verify:** CAM definition, lockout rights under state law, exclusivity clause, TI allowance mechanics.

```
CONTEXT: I represent the Landlord in a commercial lease for
[describe space: size, type, location]. Governing law: [STATE].
This is a landlord-favorable first draft — we expect negotiation.

TENANT: [Describe tenant — type of business, number of locations.]

ECONOMIC TERMS:
- Base rent: $[X]/sq ft [gross/NNN], escalating [X]% annually
- [If NNN: Tenant responsible for proportionate share of taxes,
  insurance, and CAM. CAM cap: [X]% annual increase on controllable expenses.]
- Security deposit: [X] months base rent
- [Personal guarantee: yes/no. If yes, describe scope.]
- Free rent: [X days/months] for build-out
- Tenant improvement allowance: $[X]/sq ft

TERM AND OPTIONS:
- Initial term: [X] years
- Renewal options: [X] options of [X] years each, at [market rate /
  fixed escalation], [X] months advance notice
- [Termination rights: describe or "none"]

PERMITTED USE:
- [Describe permitted use specifically]
- [Exclusivity: describe or "none"]

KEY LANDLORD PROTECTIONS:
- Assignment/subletting: Landlord consent required, [reasonableness
  standard / sole discretion]
- Default: standard cross-default, acceleration, lockout per [STATE] law
- Holdover: [X]% of then-current rent, month-to-month
- Force majeure: standard, excluding rent obligations
- SNDA: standard

FORMAT: Complete landlord-form lease, numbered sections, [STATE] law.
Flag all provisions Tenant will likely negotiate.

CONSTRAINTS: Flag provisions requiring [STATE] law verification.
Do not include Tenant-favorable provisions not specifically requested.
```

---

## Prompt 4 — M&A Specific Provisions

**Use when:** Drafting specific provisions for integration into your firm's SPA template.
**Level:** 3 — Transaction. Review time: 2-3 hours with experienced M&A partner review required.
**Verify:** Against current Delaware case law. Have M&A partner review before sending.

```
CONTEXT: I am preparing the [Buyer's/Seller's] first draft of a
[stock/asset] purchase agreement for the acquisition of [describe target].
Transaction value: $[X]M. [Describe parties briefly.]
Governing law: Delaware.

TASK: Draft the following specific provisions for review.
These will be integrated into our firm's standard [SPA/APA] template.

PROVISION 1: MATERIAL ADVERSE EFFECT DEFINITION
Draft a [Buyer/Seller]-favorable MAE definition that:
- Includes standard inclusions: [list]
- Contains standard carve-outs: [list] with disproportionate-effect exception
- [Any non-standard inclusions — flag each as non-standard]

PROVISION 2: INDEMNIFICATION — [FUNDAMENTAL/GENERAL] REPS
- Survival: [indefinitely / X months]
- Subject to basket: [yes — deductible/tipping at $X / no]
- Subject to cap: [yes — $X or X% of purchase price / no]
- Obligation: dollar-for-dollar above basket

PROVISION 3: [OTHER PROVISION]
[Describe the provision and its key parameters]

FORMAT: Each provision as a standalone numbered section for
integration into the main agreement. Defined terms in caps
consistent with standard SPA conventions.

CONSTRAINTS: Flag any deviation from Delaware market standard.
Flag non-standard provisions explicitly. Do not draft provisions
not listed above.
```
