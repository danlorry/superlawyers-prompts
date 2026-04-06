# Chapter 6 — The Case Against You

> Always add the instruction "Be genuinely adversarial. Do not soften the counterarguments." Without it, Claude defaults to balanced analysis. You need the worst version of the opposing case.

---

## Prompt 1 — Pre-Filing Brief Review

**Use when:** Before submitting any significant motion or brief.
**The rule:** Run this before you file, not after you draft. Find the problems before opposing counsel does.

```
CONTEXT: I am [plaintiff's/defendant's] attorney in [describe matter
and jurisdiction]. [Describe the key facts and legal theory in
3-5 sentences.]

I have drafted a [motion for summary judgment / motion to dismiss /
appellate brief / other]. The document is pasted below.

TASK: You are opposing counsel. Build the strongest possible case
against me.

1. THE STRONGEST COUNTERARGUMENTS:
   The 3-5 most powerful arguments opposing counsel will make.
   For each:
   - The legal argument
   - The factual support in the record opposing counsel will use
   - The case law that best supports their position
   - Damage level to my filing: HIGH / MEDIUM / LOW

2. THE WEAKEST POINTS IN MY ARGUMENT:
   Where is my filing most vulnerable? What assumptions am I making
   that opposing counsel will challenge? Where is my evidence thinnest?

3. FACTUAL GAPS:
   What gaps in my client's narrative will opposing counsel exploit?
   What questions at oral argument will I struggle to answer?

4. THE BEST CASE FOR [DENIAL/DISMISSAL]:
   If you were writing the opposition, what would the central
   argument be? How would you frame it to be most persuasive?

FORMAT: Organized by the four sections above.
Be genuinely adversarial. Do not soften the counterarguments.
I need the worst version of the opposing case, not a gentle critique.

CONSTRAINTS: Base your analysis on the document as written.
If you identify a weakness that depends on facts not provided,
note what those facts are and why they matter.

[PASTE DOCUMENT HERE]
```

---

## Prompt 2 — Oral Argument Stress Test

**Use when:** Preparing for oral argument after written brief review.

```
CONTEXT: Continuing from the previous adversarial analysis.
I have a hearing in [X] weeks before [describe court/judge if known].

TASK: Prepare me for oral argument.

1. THE THREE HARDEST QUESTIONS:
   The three questions from the bench I am least prepared to answer.
   For each:
   - The question, phrased as a judge would ask it
   - Why it is difficult
   - What a strong answer looks like
   - What a weak answer looks like

2. THE CONCESSION TRAP:
   Where is opposing counsel most likely to get me to concede
   something that damages my case? What concessions sound
   reasonable but are actually significant?

3. THE REFRAME:
   How will opposing counsel try to reframe the central issue
   unfavorably? What is the best counter-framing?

4. THE FACT I AM MOST WORRIED ABOUT:
   What single fact is most damaging? How do I handle it
   when it comes up?

FORMAT: Organized by the four sections above.
Phrase questions as a judge would — precise, direct, no warning.
```

---

## Prompt 3 — Negotiation Preparation

**Use when:** Before any significant negotiation or mediation.

```
CONTEXT: I represent [client description] in a dispute with
[opposing party]. [Describe the dispute and amounts at stake in
3-4 sentences.] We are [entering mediation / negotiating directly]
[next week / on X date]. My client's target outcome: [describe].

TASK: You represent the opposing party. Build their strongest case.

1. THEIR BEST ARGUMENTS:
   The strongest arguments for a [larger settlement / different outcome].
   For each: the legal or contractual basis, the factual support,
   the calculation that supports their position.

2. MY CLIENT'S WEAKEST POINTS:
   Where is my client's position most vulnerable?
   What will opposing counsel attack first?

3. THE LEVERAGE ANALYSIS:
   What leverage does the other side have that my client may be
   underestimating? What happens to my client if this does not settle?

4. THE MEDIATOR'S PERSPECTIVE:
   How would a neutral mediator evaluate the relative strengths?
   What outcome range would a mediator likely suggest?

5. THE OPENING MOVE:
   What opening position will opposing counsel take? What is
   the strategy behind it?

FORMAT: Organized by the five sections above.
Be genuinely adversarial — I need the worst version of the opposing case.

CONSTRAINTS: Flag any area where the answer depends on facts
I have not provided.
```

---

## Prompt 4 — The Blind Spot Question

**Use when:** After any adversarial analysis. Always add this as a follow-up.

```
Of everything you have identified in this analysis:

1. What single issue most threatens the success of my
   [motion / negotiation / transaction]? If I had one day
   to address one problem, which one?

2. What question have I not asked that I should be asking?
   What am I not thinking about in this situation?

3. What are you most uncertain about in your own analysis?
   Where would additional facts most change your conclusions?
```
