# Employment Law Prompts

> High-volume practice area with significant state-specific variation. Use Claude for the federal framework and document drafting. Always verify state-specific requirements — non-compete enforceability, at-will exceptions, and wage/hour rules vary dramatically by jurisdiction.

---

## Prompt 1 — Employment Agreement Review (Employee-Side)

**Use when:** Reviewing an employment agreement on behalf of an incoming employee.
**Verify:** Non-compete enforceability in the specific state. Equity vesting terms against cap table. Any arbitration clause requirements under state law.

```
CONTEXT: I represent an employee reviewing an employment agreement
offered by [describe employer — size, industry, stage]. The employee
is a [describe role — seniority, function]. Governing law: [STATE].
The full agreement is pasted below.

TASK: Review this agreement from the employee's perspective:

1. COMPENSATION AND BENEFITS RISKS:
   - Any provisions that allow the employer to reduce compensation
     unilaterally
   - Bonus discretion language — how much discretion does the
     employer retain?
   - Equity provisions — vesting schedule, acceleration triggers,
     post-termination exercise window, clawback provisions
   - Benefits that can be modified or eliminated without consent

2. RESTRICTIVE COVENANTS:
   - Non-compete: scope, duration, geography — is this enforceable
     in [STATE]? Flag if [STATE] has specific enforceability limits.
   - Non-solicitation: customers and employees — scope and duration
   - Non-disparagement: is it mutual?
   - Confidentiality: definition of confidential information —
     is it overbroad? Does it cover pre-existing knowledge?

3. TERMINATION PROVISIONS:
   - Grounds for termination for cause — is the definition narrow
     enough to protect the employee?
   - Notice periods and severance — what does the employee receive
     on each termination scenario?
   - What happens to unvested equity on termination?

4. INTELLECTUAL PROPERTY ASSIGNMENT:
   - Scope of IP assignment — does it cover work done on personal
     time with personal equipment?
   - Any carve-outs for pre-existing IP or personal projects?
   - Does the agreement comply with [STATE] IP assignment limits
     (if applicable — flag states with statutory limits)?

5. MISSING PROTECTIONS:
   Provisions typically negotiated by employees at this level that
   are absent from this agreement.

FORMAT: Organized by the five categories. For each HIGH risk item,
include suggested negotiating language.

CONSTRAINTS: Flag any provision where [STATE] law has specific
requirements or enforceability limits I should verify.
Flag if the non-compete is likely unenforceable in [STATE].

[PASTE AGREEMENT HERE]
```

---

## Prompt 2 — Wrongful Termination Analysis

**Use when:** Evaluating a potential wrongful termination claim.
**Verify:** State-specific at-will exceptions. Statute of limitations. EEOC/DFEH filing deadlines — these are strict and vary by claim type.

```
CONTEXT: I am an employment attorney in [STATE] evaluating a
potential wrongful termination claim. My client is a [describe
employee — role, tenure, protected characteristics if relevant].
The termination occurred on [date]. Employer: [describe — size,
industry, public/private].

FACTS: [Describe the termination circumstances in detail —
what happened, what reason was given, what the client believes
the real reason was, any relevant history]

TASK: Analyze the potential claims:

1. FEDERAL CLAIMS:
   - Title VII (if discrimination claim) — protected class,
     adverse action, causation
   - ADEA (if age) — same analysis
   - ADA (if disability) — reasonable accommodation, interactive
     process, direct threat
   - FMLA retaliation — timing, protected activity, causation
   - Whistleblower claims — Sarbanes-Oxley, Dodd-Frank, False
     Claims Act if applicable

2. STATE CLAIMS IN [STATE]:
   - At-will exceptions in [STATE] — public policy, implied
     contract, covenant of good faith
   - State discrimination statute — any broader protections than
     federal?
   - State whistleblower protections
   - Wrongful discharge in violation of public policy

3. STRENGTH ASSESSMENT:
   For each viable claim:
   - Elements and how the facts map to each element
   - Strongest facts supporting the claim
   - Weakest points / what the employer will argue
   - Overall strength: STRONG / MODERATE / WEAK / SPECULATIVE

4. PROCEDURAL ISSUES:
   - EEOC charge requirement — deadline from termination date?
   - State agency filing requirement?
   - Statute of limitations for each claim?
   - Any arbitration agreement that would affect venue?

5. DAMAGES:
   - Available damages for each claim type
   - Back pay calculation starting point
   - Front pay considerations
   - Attorney's fees availability

FORMAT: Organized by the five sections above.

CONSTRAINTS: Flag any area where [STATE] law provides broader
or narrower protections than federal law. Flag any filing
deadlines that are imminent given the termination date.
```

---

## Prompt 3 — Employee Handbook Review

**Use when:** Reviewing or drafting an employee handbook for compliance.
**Verify:** NLRA Section 7 rights implications of any policy. State-specific leave requirements. State-specific pay practice requirements.

```
CONTEXT: I am reviewing an employee handbook for [describe company —
size, industry, states of operation]. The company operates in:
[list all states]. The full handbook is pasted below.

TASK: Review for legal compliance and risk:

1. POLICIES THAT MAY VIOLATE NLRA SECTION 7:
   Identify any policy that could be read to prohibit employees
   from discussing wages, working conditions, or engaging in
   concerted activity. Flag:
   - Social media policies that restrict employee speech
   - Confidentiality policies that cover compensation
   - Policies restricting communication with coworkers
   - Non-disparagement policies that apply to current employees

2. STATE-SPECIFIC COMPLIANCE GAPS:
   For each state where the company operates, identify policies
   that may not comply with state law:
   - Paid sick leave requirements
   - Paid family leave requirements
   - Meal and rest break requirements
   - Pay frequency and final paycheck requirements
   - Non-compete policy (if included) — enforceability by state

3. DISCRIMINATION AND HARASSMENT POLICY:
   - Does the policy cover all federally protected classes?
   - Does it cover additional state-protected classes for
     each operating state?
   - Is the complaint procedure adequate?
   - Does it include bystander reporting?
   - Does it address retaliation explicitly?

4. AT-WILL LANGUAGE:
   - Is at-will status clearly stated and preserved?
   - Does any progressive discipline policy create implied
     contract issues?
   - Is the disclaimer adequate?

5. MISSING POLICIES:
   Required or strongly recommended policies that are absent,
   organized by priority: LEGALLY REQUIRED / STRONGLY RECOMMENDED /
   BEST PRACTICE

FORMAT: Organized by the five categories. Flag each issue with
severity: HIGH (legal risk) / MEDIUM (compliance gap) / LOW (best practice).

CONSTRAINTS: Flag any area where you are uncertain about a specific
state's requirements — I will verify in primary sources.

[PASTE HANDBOOK HERE]
```

---

## Prompt 4 — Severance Agreement Review

**Use when:** Reviewing a severance agreement and release on behalf of a departing employee.
**Verify:** OWBPA requirements if employee is 40+. State-specific revocation periods. Whether the release is knowing and voluntary under applicable law.

```
CONTEXT: I represent a departing employee reviewing a severance
agreement and general release. Employee details: [age, tenure,
role, reason for departure]. Employer: [describe]. State: [STATE].
The full agreement is pasted below.

TASK: Review this severance agreement:

1. THE RELEASE — SCOPE AND ENFORCEABILITY:
   - What claims are being released? Is the release broad enough
     to cover all claims the employer intends to release?
   - Are there any carve-outs for vested benefits, workers'
     compensation, or EEOC charges?
   - If the employee is 40 or older: does the release comply
     with OWBPA? (21-day consideration period, 7-day revocation
     right, specific ADEA language)
   - Does [STATE] impose any additional requirements on releases?

2. CONSIDERATION:
   - What is the employee receiving that they would not otherwise
     be entitled to?
   - Is the consideration adequate for the scope of the release?
   - Are there any conditions that could void the consideration?

3. RESTRICTIVE COVENANTS:
   - Does the agreement impose or extend any non-compete,
     non-solicitation, or non-disparagement obligations?
   - Are these obligations mutual?
   - What is the duration and scope?
   - Are they enforceable in [STATE]?

4. COOPERATION OBLIGATIONS:
   - Is the employee required to cooperate in litigation?
   - At what cost to the employee? Is there compensation for time?
   - How long do cooperation obligations last?

5. NEGOTIATING OPPORTUNITIES:
   What should my client push to negotiate? For each item:
   - The ask
   - The employer's likely response
   - Priority: HIGH / MEDIUM / LOW

FORMAT: Organized by the five sections. Specific section references
throughout. Flag OWBPA issues prominently if employee is 40+.

CONSTRAINTS: Flag any [STATE]-specific requirements for valid releases.
Flag if the consideration period or revocation period is inadequate.

[PASTE AGREEMENT HERE]
```

---

## Prompt 5 — Discrimination Charge Response

**Use when:** Drafting an employer's position statement in response to an EEOC or state agency charge.
**Verify:** The specific agency's requirements for position statements. Any document preservation obligations triggered by the charge.

```
CONTEXT: I represent the employer responding to a charge of
[describe charge — discrimination type, protected class] filed
by [describe charging party — role, tenure] with the [EEOC /
state agency]. The charge alleges: [summarize the allegations].

Our client's position: [describe the employer's version of events
and the legitimate, non-discriminatory reason for the action taken]

TASK: Draft a position statement that:

1. INTRODUCTION:
   Identifies the employer, describes the business briefly,
   and provides an overview of our position

2. FACTUAL BACKGROUND:
   Chronological narrative of the relevant facts from the
   employer's perspective. Specific, detailed, and consistent
   with documentation.

3. RESPONSE TO SPECIFIC ALLEGATIONS:
   Address each allegation in the charge specifically.
   For each: what the charging party alleges, what actually
   happened, and what documentation supports our account.

4. LEGITIMATE NON-DISCRIMINATORY REASON:
   State clearly the reason for the employment action.
   Connect the reason to documentation and consistent
   application of policy.

5. COMPARATOR ANALYSIS:
   If relevant: how similarly situated employees outside
   the protected class were treated in comparable situations.

6. CONCLUSION:
   Request for dismissal with supporting summary.

FORMAT: Formal position statement format. Professional tone.
Fact-based throughout. Avoid argumentative or emotional language.

CONSTRAINTS: Do not include any information that is legally
privileged or that we do not want disclosed to the charging party —
position statements are shared with the charging party.
Flag any factual gap I need to fill before filing.
```
