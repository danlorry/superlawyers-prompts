# Chapter 3 — Research in Minutes

> Claude is a map, not a search engine. Use these prompts to orient your research before opening Westlaw or LexisNexis. Verify every citation in primary sources.

---

## Prompt 1 — The Landscape Map

**Use when:** Starting research on an unfamiliar area of law.
**Practice area:** All litigation and transactional matters.
**Verify:** Any specific case names Claude mentions despite instructions not to.

```
CONTEXT: I am a [plaintiff's/defendant's] attorney in [STATE] representing
[brief client description] in a [type of matter] case. [Key facts of the
matter in 2-3 sentences.]

TASK: Give me a research orientation — not cases, but a structured
overview of:

1. THE DOCTRINAL LANDSCAPE: What legal theories have [plaintiffs/parties]
   used in [type of matter] cases? What have [defendants/opposing parties]
   argued?

2. THE CONTESTED ISSUES: What factual and legal questions tend to
   determine outcomes in [type of matter] cases? What distinctions
   tend to be dispositive?

3. WHERE THE LAW IS: Which jurisdictions have the most developed case
   law on [legal issue]? Is there federal preemption to consider?
   What regulatory bodies are relevant?

4. THE RESEARCH AGENDA: Given my fact pattern, where should I focus
   my primary source research? What types of cases am I looking for?

FORMAT: Organized by the four topics above. Each section 3-5 paragraphs.
No case citations — I will find cases in primary sources.

CONSTRAINTS: Flag any area where you are uncertain about the current
state of the law or where your knowledge may be outdated. Flag any area
where recent developments may have changed the analysis.
```

---

## Prompt 2 — The Unsettled Questions

**Use when:** You need to go deeper on a specific contested issue after the landscape map.
**Practice area:** All litigation matters.
**Verify:** Legal framework characterizations against recent primary sources.

```
CONTEXT: Continuing from our previous conversation about [legal issue]
in [STATE/jurisdiction].

TASK: I want to go deeper on [specific issue]. Analyze:

1. CURRENT LEGAL FRAMEWORK: What is the current framework — or the
   absence of one — for determining [specific question]? What factual
   questions tend to be dispositive?

2. THE STRONGEST ARGUMENTS FOR [PLAINTIFF/MY CLIENT]:
   What arguments have succeeded or are most likely to succeed?

3. THE STRONGEST ARGUMENTS FOR [DEFENDANT/OPPOSING PARTY]:
   What arguments have succeeded or are most likely to succeed?

4. WHERE THE LAW IS MOST UNCERTAIN: What is genuinely unsettled?
   Where would a court's decision be hardest to predict?

FORMAT: Organized by the four sections above.

CONSTRAINTS: Flag uncertainty explicitly. Note if this is an area
where the law is genuinely unsettled or rapidly developing.
Flag any area where recent developments may be relevant.
```

---

## Prompt 3 — Search Terms for Primary Source Research

**Use when:** You are ready to move from Claude's orientation to Westlaw/LexisNexis.
**Practice area:** All matters.
**Verify:** Secondary sources Claude suggests before relying on them.

```
CONTEXT: Based on our conversation about [legal issue] in [jurisdiction],
I am now going to [Westlaw/LexisNexis] to find cases.

TASK: Help me build a targeted research plan:

1. SEARCH TERMS: What terms and Boolean combinations should I use
   to find the most relevant cases? What terms are commonly used
   in [type of matter] decisions?

2. KEY JURISDICTIONS TO PRIORITIZE: Which federal circuits and states
   have produced the most relevant decisions? Which should I search first?

3. SECONDARY SOURCES: What treatises, law review articles, or ALI
   Restatement sections would give me the doctrinal foundation I need?
   Approximate titles and authors if you know them — I will verify.

4. RED FLAGS TO WATCH FOR: What defenses or counterarguments should
   I specifically look for in the cases I find?

FORMAT: Numbered lists for each category. Keep it actionable.

CONSTRAINTS: For secondary sources, flag any you are uncertain about.
I will verify all of them.
```

---

## Prompt 4 — Synthesis After Primary Source Research

**Use when:** You have completed primary source research and have verified cases.
**Practice area:** All litigation matters.
**Critical:** Paste only verified cases. Add the constraint "Do not introduce additional cases or authorities."

```
CONTEXT: I have completed primary source research on [legal issue]
in [jurisdiction]. Here are the cases I found and their holdings:

[Paste verified case names, citations, and relevant holdings here]

TASK: Help me analyze this body of case law:

1. ARGUMENT STRUCTURE: Based on these holdings, what is the strongest
   argument structure for my [plaintiff/client]? What sequence of legal
   points builds the most compelling case?

2. VULNERABILITIES: What are the weakest points in my case based on
   what these courts have held? What will opposing counsel likely attack?

3. DISTINGUISHING CASES: Are there cases in this list that opposing
   counsel will rely on that I need to distinguish? How would I
   distinguish them?

4. MISSING PIECES: What types of evidence or legal arguments would
   most strengthen my position? What should I be asking my client
   that I may not have asked yet?

FORMAT: Organized by the four questions above.

CONSTRAINTS: Base your analysis only on the cases I have provided.
Do not introduce additional cases or authorities.
```
