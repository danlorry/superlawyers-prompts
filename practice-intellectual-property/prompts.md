# Intellectual Property Prompts

> Claude's training on IP law is generally strong for US federal framework (patent, trademark, copyright) and major international treaties. Less reliable on country-specific prosecution procedures and recent USPTO/EUIPO rule changes. Always verify current examination guidelines and fee schedules in primary sources.

---

## Prompt 1 — Trademark Clearance Analysis

**Use when:** Conducting preliminary trademark clearance before filing or before a client commits to a brand.
**Verify:** Actual USPTO database search results — Claude cannot search TESS. Phonetic equivalents and design marks. Common law usage search results.

```
CONTEXT: My client wants to use the mark [MARK] for [describe
goods/services in detail — be specific about the class and
nature of the goods/services]. The mark will be used in:
[US only / US and [countries]]. Industry: [describe].

I have run a preliminary USPTO TESS search and found the
following potentially conflicting marks: [paste the search
results or describe the conflicts found].

TASK: Analyze the trademark clearance issues:

1. LIKELIHOOD OF CONFUSION ANALYSIS:
   For each potentially conflicting mark identified:
   - Similarity of the marks (sight, sound, meaning)
   - Similarity of the goods/services
   - Channels of trade and consumer sophistication
   - Strength of the cited mark (inherent and acquired distinctiveness)
   - Overall likelihood of confusion: HIGH / MEDIUM / LOW
   - Recommended action: AVOID / PROCEED WITH CAUTION / CLEAR

2. STRENGTH OF MY CLIENT'S MARK:
   - Where does [MARK] fall on the distinctiveness spectrum?
     (Fanciful, arbitrary, suggestive, descriptive, generic)
   - If descriptive: is there acquired distinctiveness (secondary meaning)?
   - What scope of protection would the mark likely receive?

3. FILING STRATEGY:
   - Which international class(es) should the application cover?
   - Should the client file on an intent-to-use or use-in-commerce basis?
   - Are there related marks or variations the client should also file?
   - Priority considerations: any reason to file quickly?

4. RISKS REMAINING:
   - What risks remain even if USPTO clears the mark?
   - Common law users who don't appear in the USPTO database
   - State registrations
   - Social media / domain name conflicts
   - International conflicts if the client operates globally

5. RECOMMENDATION:
   Overall clearance recommendation: PROCEED / PROCEED WITH
   MODIFICATIONS / DO NOT PROCEED. Explain the reasoning.

FORMAT: Organized by the five sections. For each conflict in
section 1, provide a specific likelihood of confusion analysis —
not just a conclusion.

CONSTRAINTS: This analysis is based on the search results I have
provided. It does not substitute for a comprehensive clearance
search including common law. Flag any area where additional
searching is needed before advising the client to proceed.
```

---

## Prompt 2 — Copyright Infringement Analysis

**Use when:** Evaluating whether a client's work infringes a third-party copyright, or whether a third party has infringed the client's copyright.
**Verify:** Registration status and date against USCO records. Any licensing history between the parties.

```
CONTEXT: I am analyzing a potential copyright dispute.
[My client is the alleged infringer / My client is the copyright owner.]

The allegedly infringed work: [describe — type of work, date
created, registration status if known, key creative elements]

The allegedly infringing work: [describe — type of work, date
created, how it relates to the original]

Relationship between the parties: [any licensing history, prior
relationship, how the alleged infringer may have accessed the work]

TASK: Analyze the copyright infringement claim:

1. COPYRIGHTABILITY OF THE ORIGINAL WORK:
   - Is the original work copyrightable?
     (Original, creative, fixed in tangible medium)
   - What elements are protectable vs. unprotectable?
     (Ideas, facts, scènes à faire, public domain elements)
   - How strong is the copyright in the protectable elements?

2. OWNERSHIP AND REGISTRATION:
   - Who owns the copyright? Any work-for-hire issues?
   - Is the work registered? Registration date vs. infringement date?
     (Registration before infringement = statutory damages and
     attorney fees available)
   - Any transfers or licenses that affect ownership?

3. INFRINGEMENT ANALYSIS:
   - Copying: is there evidence of access + substantial similarity?
   - Substantial similarity: compare the protectable elements only.
     Apply the appropriate test for this type of work.
   - Is the copying of protectable expression or only unprotectable
     elements (ideas, facts, style)?

4. DEFENSES:
   - Fair use: analyze all four factors for this specific use
     (purpose and character, nature of work, amount taken,
     market effect)
   - License: any express or implied license?
   - Independent creation: is there evidence of it?
   - Statute of limitations: is the claim timely?
     (3 years from discovery)

5. DAMAGES AND REMEDIES:
   - If registered before infringement: statutory damages
     ($750–$30,000; up to $150,000 for willful)
   - If not registered before infringement: actual damages only
   - Attorney's fees: available only if registered before infringement
   - Injunctive relief: likelihood, scope

FORMAT: Organized by the five sections. Be specific about which
elements are and are not protectable in section 1.

CONSTRAINTS: Fair use analysis is highly fact-specific and
unpredictable — present the analysis as a framework, not a
guaranteed outcome. Flag if registration status needs to be
verified against USCO records.
```

---

## Prompt 3 — IP License Agreement Review

**Use when:** Reviewing an IP license agreement (patent, trademark, copyright, or technology).
**Verify:** Scope of IP covered against the actual IP portfolio. Any field-of-use restrictions against the client's business plan. Royalty calculation mechanics.

```
CONTEXT: I represent the [Licensor / Licensee] in an IP license
agreement. IP being licensed: [describe — patents, trademark,
copyright, trade secrets, software]. Purpose: [describe intended use].
Industry: [describe]. Governing law: [STATE].
The agreement is pasted below.

TASK: Review from my client's perspective:

1. SCOPE OF THE LICENSE:
   - What IP is licensed? Is the definition broad enough for
     my client's needs?
   - Exclusivity: exclusive, sole, or non-exclusive? In what
     field of use? In what territory?
   - Sublicensing: can my client sublicense? Under what conditions?
   - Improvements: who owns improvements to the licensed IP?
     Is there a grant-back obligation? Flag if grant-back is
     exclusive — this is heavily disfavored for the licensee.

2. FINANCIAL TERMS:
   - Royalty structure: running royalties, milestone payments,
     upfront fee?
   - Royalty base: net sales? Gross revenue? How is the base
     defined? What deductions are allowed?
   - Minimum royalties: are there minimums that could trigger
     termination if not met?
   - Audit rights: can my client audit the royalty calculations?
     Frequency, notice, and cost allocation?

3. REPRESENTATIONS AND WARRANTIES:
   - Does [Licensor] warrant that it owns the IP and has the
     right to license it?
   - Is there a warranty of non-infringement?
   - What happens if a third party claims the licensed IP
     infringes their rights? Who defends? Who pays?
   - Are the warranties adequate for my client's reliance on
     the licensed IP?

4. TERM AND TERMINATION:
   - How long is the license? Is it tied to patent life?
   - What triggers termination? Is there a cure period?
   - What happens to sublicenses on termination?
   - What transition rights exist after termination?

5. MISSING PROVISIONS AND RED FLAGS:
   - Any provision that is unusual or one-sided for a license
     of this type?
   - Any important provision that is absent?
   - If the licensed IP is patents: is there a patent challenge
     clause? (Licensee's right to challenge validity)

FORMAT: Organized by the five sections. Flag any grant-back
obligation prominently — these can significantly affect
the licensee's business.

CONSTRAINTS: Flag any provision that would restrict my client's
ability to develop competing products or challenge the validity
of the licensed IP.

[PASTE AGREEMENT HERE]
```

---

## Prompt 4 — Trade Secret Protection Audit

**Use when:** Advising a company on protecting its trade secrets, or evaluating the strength of a trade secret claim.
**Verify:** State trade secret law (UTSA vs. DTSA differences). Any specific industry regulations on confidential information.

```
CONTEXT: I am advising [Company] on its trade secret protection.
The company's key confidential information includes:
[describe the trade secrets — formulas, processes, customer lists,
software, business strategies, etc.]

Current protection measures in place (describe what the client
has told you): [describe]

TASK: Assess the company's trade secret protection:

1. WHAT QUALIFIES AS A TRADE SECRET:
   For each category of information the client identifies:
   - Does it qualify as a trade secret under the DTSA?
     (Value from secrecy, reasonable steps to maintain secrecy)
   - How valuable is the secret? What would a competitor pay for it?
   - How easily could it be reverse-engineered or independently developed?

2. CURRENT PROTECTION GAPS:
   Evaluate whether the company has taken "reasonable measures"
   to protect each category of trade secret:
   - Physical security
   - Digital access controls
   - Employee agreements (NDA, IP assignment)
   - Contractor and vendor agreements
   - Need-to-know access controls
   - Exit procedures for departing employees

3. RECOMMENDED IMPROVEMENTS:
   For each gap identified, what specific steps should the
   company take? Prioritize by: CRITICAL / IMPORTANT / BEST PRACTICE

4. EMPLOYEE DEPARTURE PROTOCOL:
   What should the company do when an employee with access
   to trade secrets departs?
   - Exit interview process
   - Device and access termination
   - Return of company property
   - Reminder of ongoing obligations
   - Monitoring for potential misappropriation

5. IF A THEFT HAS OCCURRED:
   If the client suspects a former employee or competitor
   has taken trade secrets:
   - What evidence should be preserved immediately?
   - What are the available remedies under the DTSA and state law?
   - What is the statute of limitations?
   - Is a TRO/preliminary injunction appropriate?

FORMAT: Organized by the five sections. Be specific about gaps
in section 2 — vague recommendations are not useful.

CONSTRAINTS: The DTSA preempts some but not all state law claims —
flag where state law may provide additional protections.
Flag if any of the client's "trade secrets" may not qualify
for protection.
```
