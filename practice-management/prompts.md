# Practice Management Prompts

> These prompts address the non-legal work that consumes a significant portion of every lawyer's day: client communication, matter administration, business development, and firm operations. No legal citations needed — these are administrative and communication tasks where Claude's output quality is high and verification requirements are low.

---

## Prompt 1 — Meeting and Call Summary

**Use when:** Converting notes or a transcript from a client call or meeting into a usable summary.
**Verify:** Any action items or commitments attributed to you or your client before sending.

```
CONTEXT: I am a [practice area] attorney. I just completed a
[client call / team meeting / court hearing / deposition] on
[matter description]. My notes or transcript are pasted below.

TASK: Convert these notes into a structured summary:

1. ATTENDEES AND DATE

2. KEY DECISIONS MADE:
   List each decision clearly. Note who made it and any conditions.

3. ACTION ITEMS:
   For each action item:
   - What needs to be done
   - Who is responsible
   - Deadline (if stated or implied)

4. OPEN ISSUES:
   Questions or issues raised that were not resolved.
   What information is needed to resolve each one?

5. NEXT STEPS:
   The agreed next steps and timeline for this matter.

FORMAT: Clean memo format suitable for the matter file and
for sharing with the client. Maximum 1 page.

CONSTRAINTS: Only include what is in the notes — do not add
information or inferences. If something is unclear from the
notes, flag it rather than guessing.

[PASTE NOTES / TRANSCRIPT HERE]
```

---

## Prompt 2 — Engagement Letter

**Use when:** Drafting an engagement letter for a new client matter.
**Verify:** Fee arrangement against your conversation with the client. Scope of representation against what was discussed. State bar requirements for engagement letters in your jurisdiction.

```
CONTEXT: I am drafting an engagement letter for a new client matter.
Attorney/firm: [name]
Client: [name and entity type]
Matter: [describe the legal matter]
Fee arrangement: [hourly at $X / flat fee of $X for [scope] /
  contingency at X% / retainer of $X against hourly rate of $X]
Scope of representation: [describe specifically what is and is not included]
Governing law: [STATE]
Any client-specific terms to include: [describe or "none"]

TASK: Draft an engagement letter that:

1. Identifies the client and the specific matter clearly
2. Describes the scope of representation — what we will do
   AND what is explicitly excluded
3. Describes the fee arrangement clearly and completely
4. Describes billing practices: frequency, payment terms,
   handling of disputed bills
5. Addresses confidentiality and conflicts briefly
6. Includes file retention policy
7. Includes a statement that the client has the right to
   terminate the representation
8. Requests client signature acknowledging the terms

FORMAT: Professional letter format on firm letterhead.
Plain English where possible. Maximum 2 pages.

CONSTRAINTS: Flag any provision that requires state bar
rule verification for [STATE]. Do not include provisions
not listed above without flagging them.
```

---

## Prompt 3 — Status Report to Client

**Use when:** Providing a periodic status update to a client on an active matter.
**Verify:** All dates, deadlines, and next steps before sending.

```
CONTEXT: I am a [practice area] attorney providing a status
update to [client description] on [matter description].
Client sophistication level: [sophisticated business client /
individual with no legal background / other]

Since the last update: [describe what has happened]
Current status: [describe where things stand]
Upcoming milestones: [describe what is coming]
Action required from client: [describe or "none at this time"]
Next expected update: [date or milestone]

TASK: Write a client status update that:
1. Opens with the bottom line — where things stand in one sentence
2. Summarizes what happened since the last update
3. Explains the current status and what it means for the client
4. Identifies any action required from the client, with deadline
5. Sets expectations for next steps and timeline
6. Closes with an invitation to call with questions

FORMAT: Email format. Plain English — no legal jargon without
explanation. Maximum 400 words.

CONSTRAINTS: Do not include legal opinions or risk assessments
unless I have provided them above. This is a status update,
not a legal memorandum.
```

---

## Prompt 4 — Business Development: Practice Area Description

**Use when:** Writing website copy, bio descriptions, or pitch materials describing a practice area or specific service.

```
CONTEXT: I am writing [website copy / a pitch document / a bio
section] describing my [practice area / specific service].
Target audience: [describe — general businesses / individual
consumers / specific industry / sophisticated institutional clients]
Tone: [professional and authoritative / approachable and plain-spoken]
Key differentiators: [what makes this practice or attorney distinctive]
Key clients or matters (if public): [describe or "confidential"]
Word limit: [X] words

TASK: Write compelling, accurate copy that:
1. Describes what this practice area does in terms the target
   audience understands — not in legal jargon
2. Explains what problems it solves for clients
3. Conveys the attorney's/firm's distinctive approach or expertise
4. Includes a clear call to action

FORMAT: [Specify: website paragraph / bulleted service list / bio section]

CONSTRAINTS: No specific case results or client names unless I have
provided them above. No claims about outcomes. No comparative
statements about other firms. Flag any statement that might
require bar association review before publishing.
```

---

## Prompt 5 — Deposition Preparation Summary

**Use when:** Preparing a witness for deposition.
**Verify:** All factual content against the actual record before the deposition prep session.

```
CONTEXT: I am preparing [describe witness — role, relationship to
the case] for a deposition in [describe matter briefly].
The deposition is on [date]. Opposing counsel: [describe if known].

Key facts the witness needs to know:
[Describe the key facts from the record that are relevant to
this witness]

Areas opposing counsel will likely focus on:
[Based on discovery and the theory of the case, what will
they ask about]

Documents the witness should review:
[List the key documents]

TASK: Create a deposition preparation outline for a
[X]-hour prep session that includes:

1. WHAT A DEPOSITION IS:
   A brief, plain-English explanation of the process and purpose.
   Emphasize: it is testimony under oath, it can be used at trial,
   the witness should tell the truth.

2. THE FIVE RULES:
   The five most important behavioral rules for this witness,
   stated as specific behavioral instructions — not general advice.
   Tailor to this witness's known tendencies:
   [describe tendencies if known — talks too much, gets defensive,
   rushes to answer, etc.]

3. KEY TOPICS AND ANTICIPATED QUESTIONS:
   For each likely topic area:
   - The topic
   - The questions likely to be asked
   - The key facts the witness should know cold
   - Any documents the witness should be able to identify

4. DIFFICULT AREAS:
   The questions the witness is most likely to struggle with
   and how to handle them.

5. LOGISTICS:
   What to bring, what to wear, what happens procedurally.

FORMAT: Outline format. Behavioral rules as numbered list.
Topics as organized sections. Maximum 4 pages.

CONSTRAINTS: Do not include any privileged attorney-client
communications or work product in this document —
it may need to be produced if requested.
```

---

## Prompt 6 — Billing Narrative Review and Improvement

**Use when:** Reviewing time entries for clarity and defensibility before billing.
**Verify:** Accuracy of time entries against your actual work. Compliance with client billing guidelines if applicable.

```
CONTEXT: I am reviewing time entries for [client / matter] before
sending the invoice. The client is [describe — sophisticated /
price-sensitive / has specific billing guidelines].
The time entries are pasted below.

TASK: Review and improve these time entries:

1. FLAG ENTRIES THAT ARE:
   - Too vague to be defensible ("Review documents" — which documents?)
   - Too long for the described task — may invite pushback
   - Duplicative of other entries on the same day
   - Using block billing (multiple tasks in one entry without
     time allocation) — flag if client guidelines prohibit this

2. REWRITE FLAGGED ENTRIES:
   For each flagged entry, provide a rewritten version that is:
   - Specific about what was done
   - Describes the purpose/relevance to the matter
   - Defensible if the client questions it

3. SUMMARY:
   Total hours, total amount, and any overall billing patterns
   worth noting before sending.

FORMAT: List the flagged entries with original and suggested
rewrite. Keep rewrites concise — 1-2 sentences maximum.

CONSTRAINTS: I will review all rewrites before they appear
on the invoice. Do not change time amounts — only the narrative.
Do not add information that is not in the original entry.

[PASTE TIME ENTRIES HERE]
```
