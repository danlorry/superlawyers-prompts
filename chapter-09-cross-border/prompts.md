# Chapter 7 — From Legal to Human

> Complete the legal work before running any prompt in this chapter. Claude translates finished legal products. It does not produce legal analysis.

---

## Prompt 1 — Legal Opinion to Client Letter

```
CONTEXT: I am a [practice area] attorney in [STATE].
My client is [describe client — professional background, legal
sophistication, communication style].

I have completed my legal analysis on [describe topic].
The analysis is pasted below.

TASK: Rewrite this analysis as a client letter that:

1. Opens with the bottom line — what I am recommending and why —
   in the first paragraph

2. Explains the key points in plain language with concrete examples
   where helpful

3. Presents any decision the client needs to make with a clear
   framework: what factors favor each option, what I need from
   them to finalize the recommendation

4. Ends with a specific ask: what I need from them, and by when

FORMAT: Letter format. Maximum [X] pages. No legal jargon without
immediate plain-English explanation. No citations.

CONSTRAINTS: Do not oversimplify to the point of inaccuracy.
If a nuance is legally significant, find plain language for it —
do not omit it. Flag any sentence where you simplified something
I should review for accuracy.

[PASTE LEGAL ANALYSIS HERE]
```

---

## Prompt 2 — Demand Letter Response to Non-Lawyer Client

```
CONTEXT: I represent [client description] who has received
[describe demand letter — from whom, alleging what].
My client has no legal background and is [frightened / confused /
overwhelmed].

My preliminary legal assessment: [insert your assessment —
strength of their claim, likely defenses, risk level,
recommended immediate actions].

TASK: Write a client communication that:

1. Opens by addressing the emotional reality first

2. Explains what the demand letter actually is and is not:
   - What it requires my client to do right now
   - What it does not mean
   - What the sender is trying to accomplish

3. Explains my preliminary assessment in plain language:
   - How strong their claim is, honestly
   - What the main defenses are
   - What the realistic outcomes are

4. Gives clear immediate action steps:
   - What to do right now
   - What NOT to do (especially regarding responding directly)
   - What to preserve and send me

5. Sets expectations for timeline and next steps

FORMAT: Email format. Direct and calm. Maximum 500 words.

CONSTRAINTS: Be accurate about risk. Do not over-reassure if
the situation is genuinely serious. Informed calm, not false comfort.
```

---

## Prompt 3 — Pre-Meeting Preparation Email

```
CONTEXT: My client is [describe client] preparing for
[deposition / negotiation / closing / mediation] in [X] days.
[Describe any relevant client characteristics — first time,
nervous, tends to overtalk, etc.]

TASK: Write a preparation email that:

1. Explains what [the proceeding] is and what it is for
   (2 short paragraphs maximum)

2. Gives the [X] most important rules, each as a concrete
   behavioral instruction — not "be concise" but "answer only
   the question asked, then stop talking"

3. Tells them specifically what to bring and what to wear

4. Explains what I will be doing and when I will and will not
   [object / intervene / speak]

5. Ends with my contact information and invitation to call
   with questions

FORMAT: Email format. Conversational tone. Maximum 600 words.

CONSTRAINTS: Rules must be specific enough to be actionable.
No legal jargon. Procedure only — no substance of the case.
```

---

## Prompt 4 — Client to Legal Structure (Reverse Translation)

**Use when:** Preparing for an initial consultation from a client email.

```
CONTEXT: I am a [practice area] attorney. A potential client
has sent me the email below. I am preparing for an initial
consultation.

TASK: From the client's email, extract and organize:

1. THE LEGAL CLAIMS: What claims does this fact pattern potentially
   support? For each: the claim, basic elements, which facts support
   or undermine each element.

2. KEY FACTS NEEDED: What facts are missing that I need to obtain
   in the consultation to assess the strength of potential claims?

3. THE TIMELINE: Chronological timeline of events. Flag any statute
   of limitations issues I should immediately check.

4. THE QUESTIONS TO ASK: The five most important questions for the
   initial consultation, in order of priority.

FORMAT: Organized by the four sections above.

CONSTRAINTS: Flag any area where the email is ambiguous about
legally material facts. Note if any claim has obvious threshold
problems based on what the email does say.

[PASTE CLIENT EMAIL HERE]
```

---

# Chapter 8 — The Documents That Write Themselves

> Build the review checklist before you build the template. Automation without supervision is not responsible practice.

---

## Prompt 1 — Retainer Agreement

```
RETAINER AGREEMENT TEMPLATE

DOCUMENT: Attorney-Client Fee Agreement and Retainer
GOVERNING LAW: [STATE]

STANDARD PROVISIONS:
- Scope of representation (specific to this matter only)
- Hourly rate and billing increments (0.1 hour minimum)
- Retainer deposit applied to fees earned
- Monthly invoicing, net-30 payment terms
- Right to withdraw for non-payment with reasonable notice
- Client obligations: cooperation, truthfulness, timely response
- No guarantee of outcome
- File retention and return policy
- Electronic communication consent
- Signature block for both parties

VARIABLE INFORMATION:
- Client name and address: [FILL IN]
- Attorney/firm name: [FILL IN]
- Matter description: [FILL IN — be specific about scope]
- Hourly rate: $[FILL IN]
- Retainer amount: $[FILL IN]
- Any scope exclusions: [FILL IN or "none"]
- State: [FILL IN]

OPTIONAL PROVISIONS:
- Flat fee arrangement: include if flat-fee matter [FILL IN amount and scope]
- Co-counsel disclosure: include if co-counsel involved
- Third-party payor: include if someone other than client is paying

FORMAT: Numbered sections. Plain English where possible.
Signature block with date lines. Maximum 4 pages.

CONSTRAINTS: Flag provisions requiring state bar rule verification.
Do not include provisions not listed above without flagging.
```

---

## Prompt 2 — Standard Demand Letter

```
DEMAND LETTER TEMPLATE

DOCUMENT: Pre-Litigation Demand Letter
TONE: Professional and firm. Not aggressive. Factual.

STANDARD PROVISIONS:
- Header identifying this as a demand letter from counsel
- Statement of representation
- Factual background (2-3 paragraphs)
- Legal basis for the demand
- Specific demand: amount and/or action required
- Deadline for response
- Consequence of non-compliance
- Contact information for response

VARIABLE INFORMATION:
- Client name: [FILL IN]
- Recipient name and address: [FILL IN]
- Factual background: [FILL IN]
- Legal basis: [FILL IN]
- Demand: [FILL IN — amount or specific action]
- Deadline: [FILL IN — typically 10-30 days]
- Consequence: [FILL IN — litigation, regulatory referral, etc.]
- Governing law: [FILL IN]

FORMAT: Business letter format. Re: line identifying the matter.
Maximum 2 pages. No citations in the body.

CONSTRAINTS: Flag if any legal theory requires state-specific
verification. Do not threaten criminal action to collect
a civil debt — flag if the description suggests this.
```

---

# Chapter 9 — Everywhere at Once

> Claude provides the orientation layer. Local counsel provides the verification layer. Never skip local counsel verification before advising a client on jurisdiction-specific requirements.

---

## Prompt 1 — Multi-Jurisdiction Matrix

```
CONTEXT: I am a US attorney advising [client description] on
[legal issue] that applies simultaneously in the following
jurisdictions: [list all jurisdictions].

[Describe the specific facts that trigger the multi-jurisdiction
analysis — e.g., data breach details, transaction structure,
employment situation.]

TASK: Create a multi-jurisdiction analysis matrix. For each
jurisdiction, provide:

1. KEY REQUIREMENT: What is the primary legal obligation
   in this jurisdiction for this situation?

2. DEADLINE/TIMELINE: What timeframes apply?

3. WHO IS INVOLVED: Which regulatory authority? What
   notifications are required and to whom?

4. THRESHOLD: Does my specific situation meet the threshold
   for this jurisdiction? Apply the facts I have provided.

5. KEY UNCERTAINTY: What is the main question that could
   change the analysis for this jurisdiction?

FORMAT: Table format — one row per jurisdiction, one column
per item above. After the table, a prioritized action list:
which jurisdictions require action first and why.

CONSTRAINTS: Flag any jurisdiction where your knowledge may
be outdated. Flag genuine uncertainty on threshold analysis.
This is an orientation analysis — I will verify with local
counsel before advising the client.
```

---

## Prompt 2 — Local Counsel Briefing Memo

**Use when:** Converting Claude's orientation analysis into targeted local counsel engagement.

```
CONTEXT: I have completed a preliminary multi-jurisdiction
analysis on [legal issue] (summary pasted below). I am now
preparing to engage local counsel in each jurisdiction.

TASK: For each jurisdiction in the analysis, draft a briefing
memo for local counsel that:

1. Summarizes what my preliminary analysis concluded
   for their jurisdiction (2-3 sentences)

2. Lists the specific questions I need them to confirm
   or correct — verification questions, not orientation questions

3. Identifies the specific facts most likely to be legally
   significant in their jurisdiction

4. States my timeline constraint and what I need by when

FORMAT: One memo per jurisdiction. Maximum 1 page each.
Direct questions — these are working documents, not formal correspondence.

CONSTRAINTS: Verification questions only. I do not need local counsel
to explain the framework — I need them to confirm whether my
framework is correct and analyze the specific facts.

[PASTE PRELIMINARY ANALYSIS HERE]
```
