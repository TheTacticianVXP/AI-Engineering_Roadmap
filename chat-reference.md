# Chat Reference Guide
### Complete Roadmap v5.1 — Learning System

```
VERSION:    Updated for Learning Prompt v3.1 + Weekly Plan v5.1
SUPERSEDES: Previous version built against v3.0 + v5 FILE 2

KEY CHANGES FROM PREVIOUS VERSION:
  - All file references updated: v3.0 → v3.1, v5-FILE2 → v5-1-RESTRUCTURED
  - Chat 1 (Daily Learning) overhauled — now reflects the dual-exposure
    system where evening study is driven by office confusion
  - Chat 2 (Code Review) expanded to cover mini-projects extracted from
    the production codebase, not just exercise code
  - Chat 10 (Production Codebase) added — new chat for the office learning
    context introduced in v3.1 (reading, tracing, experimenting, mini-projects)
  - Chat 11 (Deadline-Driven Project Sprint) added — expedited project mode
    for when a project has a hard external deadline
  - Phase labels removed from all opening prompts — week number is sufficient,
    FILE 1 has phase labels for curriculum reference

WHAT THIS FILE IS:
  Your go-to reference for every chat you will open across this entire
  6-month journey. For each chat: what it's for, which model to use,
  which files to upload, the opening prompt, how long to run it before
  restarting, and what triggers a restart.

  At the bottom: the universal Summary Prompt — use it to close any chat.
  The summary output IS your learning log. Save every one.

HOW TO USE:
  1. Decide which chat type you need (see the 11 types below)
  2. Open a new Claude chat, select the right model
  3. Upload the listed files
  4. Paste the opening prompt, fill in the bracketed fields
  5. Work. When the restart trigger hits, run the Summary Prompt first,
     save the output, then start fresh.
```

---

## Quick Reference

| # | Chat | Model | Restart After |
|---|------|-------|---------------|
| 1 | Daily Learning (Home Study) | Sonnet 4.6 | End of each roadmap week |
| 2 | Code Review | Sonnet 4.6 | Every 8-10 code submissions |
| 3 | Project 1: Doc Digitisation | Sonnet 4. | After each milestone |
| 4 | Paper Reading | Opus 4.6 | Every 2-3 papers |
| 5 | Project 2: Multimodal RAG | Sonnet 4.6 | After M2, M4, M5 |
| 6 | Project 3: VLM Fine-Tuning | Sonnet 4.6 (M1,M2,M5) / Opus 4.6 (M3,M4) | After each milestone |
| 7 | Quick Lookup | Haiku 4.5 | After 10-15 exchanges |
| 8 | Phase Transition | Opus 4.6 | One per phase boundary |
| 9 | Open Source | Sonnet 4.6 | One per PR |
| 10 | Production Codebase | Sonnet 4.6 | End of each office week |
| 11 | Deadline-Driven Project Sprint | Sonnet 4.6 | After deadline is met |

---
---

## CHAT 1 — Daily Learning Partner (Home Study)

### Purpose
Your study companion for all foundation learning that happens outside
the office — early mornings (5-7 AM), evenings (7:30-9:30 PM), and
weekends. This is the chat you open when something from a book, course,
or video isn't clicking, or when your evening study is targeting a
specific confusion from the office that day.

The v3.1 dual-exposure mechanic matters here: your evening study is not
random — it is often *driven by what confused you at the office*. If you
traced a decorator pattern in production code and didn't understand it,
that evening you study decorators in Fluent Python. When you open this
chat in the evening, you can say "I saw X at the office, I'm now reading
Y in the book, and this part still doesn't click." Claude knows both
contexts from the uploaded files.

This chat is NOT for:
- Office production code questions — that is Chat 10
- Code review of code you have written — that is Chat 2
- Being walked through content you have not read yet
- General "teach me X" when a book covers it — read first, then ask

### What Claude tracks in this chat
- Your current rung and what that means for how it responds
- What week you are on and what the home study schedule says (from the weekly plan)
- The dual-exposure mechanic — connecting evening study to office exposure
- Concepts that are solid vs. shaky across the week

### Model
**Sonnet 4.6**

### Files to Upload
`learning-prompt-v3-1.md` + `v5-1-RESTRUCTURED-WEEKLY-PLAN.md`

### Opening Prompt
```
Files uploaded: Learning Prompt v3.1 + Restructured Weekly Plan v5.1.
Read both fully before responding. The learning prompt governs how you
interact with me. The weekly plan tells you my home study schedule —
do not ask me to summarise it.

This chat covers my HOME STUDY only: mornings, evenings, weekends.
Office production code questions go to a separate chat.

Week: [X] | Rung: [X]

[Only include if restarting from a previous chat summary:]
Carrying forward: [paste SHAKY + OPEN THREADS from your last summary]
```

### Restart Trigger
End of each roadmap week — Weeks 1, 2, 3, 4 during onboarding, then at
natural phase boundaries after. Week boundary = clean restart, even if
the chat feels short. A week-1 chat and a week-2 chat are different
contexts: different resources, different rung, different office exposure.

Secondary trigger: Claude ignores earlier context or you are re-explaining
things it should already know. Restart immediately regardless of where
you are in the week.

---

## CHAT 2 — Code Review

### Purpose
You write code. Then you bring it here. Two types of code live in this
chat under v3.1:

**Type A — Exercise and practice code:** Scripts written at home from
Robust Python chapters, Exercism exercises, Karpathy re-implementations
from memory, CS231n assignments, small scripts from course material.

**Type B — Mini-project rebuilds:** Modules you extracted from the
office codebase and rebuilt from scratch at home. For these, bring both
your code AND your COMPARISON.md notes (how your version differs from
the production approach). Claude reviews your implementation and helps
you understand why the production code made different choices.

Claude does not write code in this chat. It reviews what you wrote and
tells you what to fix yourself.

This chat is NOT for:
- Getting help writing code before it exists
- "How do I implement X" questions — Chat 1 or Chat 7
- Reviewing AI-generated code
- Reviewing production code from the office directly — Chat 10

### What Claude tracks in this chat
- Recurring patterns in your mistakes across submissions
- Whether code quality is improving week-over-week
- For mini-projects: the gap between your version and the production
  approach, and whether that gap is closing

### Model
**Sonnet 4.6**

### Files to Upload
`learning-prompt-v3-1.md`

### Opening Prompt
```
File uploaded: Learning Prompt v3.1. Read it — specifically the
Independence Ladder, Clean Code from Day 1, and Test-Driven Approach sections.
Your role: code reviewer only. You do not write code.

Week: [X] | Rung: [X]
Type: [Exercise / Mini-project rebuild]

What this code is: [one sentence]
What I was trying to demonstrate: [e.g. "type hints on every function, guard clauses"]

[For mini-project rebuilds only, also include:]
Production comparison notes: [paste your COMPARISON.md or summarise the key differences]

[paste your code]
```

### Restart Trigger
After 8-10 distinct code submissions, or roughly every 2-3 weeks —
whichever comes first. The summary at close should note recurring
patterns in your mistakes so the next Code Review chat starts with
that context.

---

## CHAT 3 — Project 1: Indian Document Digitisation

### Purpose
One chat per milestone across the 5-milestone project. Each chat covers
exactly one milestone. You bring your attempts, blockers, and design
questions. Claude reviews and challenges your approach — it does not
build the pipeline for you.

Per v5.1, Project 1 runs across Week 4 (Friday evening planning +
full weekend build). All 5 milestones are compressed into one weekend.
Move fast. Done is better than perfect at this stage.

The project: a pipeline that takes a photographed Indian document
(Aadhaar, PAN, electricity bill) and extracts structured fields using
OpenCV preprocessing, OCR (Tesseract + PaddleOCR), and a VLM extraction
layer. Wrapped in a FastAPI endpoint with tests and a GitHub README.

Milestones:
M1 — Repo setup, sample documents, annotation schema (~5 hrs)
M2 — OpenCV preprocessing pipeline (~5 hrs)
M3 — OCR layer: Tesseract + PaddleOCR + EasyOCR comparison (~5 hrs)
M4 — VLM extraction + evaluation script (~5 hrs)
M5 — FastAPI endpoint, tests, README, GitHub push (~5 hrs)

### What Claude tracks in this chat
- Current milestone scope and what done looks like
- Decisions made in previous milestones (from your carrying-forward note)
- Whether you are making design decisions yourself or outsourcing them

### Model
**Sonnet 4.6**

### Files to Upload
`learning-prompt-v3-1.md` + `v5-FILE1-CURRICULUM.md`

### Opening Prompt
```
Files uploaded: Learning Prompt v3.1 + Curriculum (FILE 1).
Project 1 spec is in FILE 1 under "Project 1: Indian Document Digitisation Pipeline."
Read both. Your role: review my work, challenge my design decisions,
help me think through blockers. Do not build anything for me.

Week: [X] | Rung: [X] | Milestone: M[X] — [name]

[Only include if restarting mid-milestone or starting M2+:]
Carrying forward: [paste SHAKY + OPEN THREADS from last milestone's summary]
```

### Restart Trigger
After each milestone is complete — 5 chats, 5 milestones. The summary
from each milestone becomes the handoff note for the next chat.

---

## CHAT 4 — Paper Reading

### Purpose
For the dense VLM and systems papers in your roadmap. You read the paper
first — abstract, introduction, method section, key figures — take your
own notes, then come here with specific questions. This is NOT "explain
this paper to me."

Papers in your roadmap, in order:
- ViT (Dosovitskiy et al., 2021) — Week 3 weekend
- CLIP (Radford et al., 2021) — Week 3 weekend
- LLaVA / LLaVA-1.5 (Liu et al., 2023) — Week 4 evening
- Qwen-VL or InternVL — Weeks 5-6
- LayoutLMv3 / Donut — Weeks 5-6
- DPO (Rafailov et al., 2023) — Weeks 10-11
- ZeRO (Rajbhandari et al., 2020) — Weeks 10-11
- FlashAttention (Dao et al., 2022) — Weeks 10-11

The rule: write your own notes on what you understood before asking
questions. If you have not read the paper, close this chat.

### What Claude tracks in this chat
- Which papers have been discussed and the architectural thread connecting them
- Your growing mental model of VLM architectures across papers
- Recurring gaps that appear across multiple papers

### Model
**Opus 4.6**
*(Dense architectural reasoning across multiple papers. Opus earns its
cost here. Sonnet handles single-concept questions; Opus handles the
cross-paper synthesis and multi-variable architectural reasoning.)*

### Files to Upload
`learning-prompt-v3-1.md`

### Opening Prompt
```
File uploaded: Learning Prompt v3.1. Read it.

I have already read this paper. I am not asking for a summary.
I have specific questions about sections I read and did not understand.

Paper: [full title] | Authors: [last name et al.] | Year: [YYYY]
Week context: [e.g. "Week 3 weekend — ViT, before moving to CLIP"]

Sections I read: [e.g. abstract, intro, Section 3 method, key figures]

My notes — what I understood (in my own words):
- [bullet]
- [bullet]
- [bullet]

My questions:
1. [specific question]
2. [specific question]
```

### Restart Trigger
After every 2-3 papers. The summary should synthesise the architectural
thread across the papers in this cluster — what each one contributed,
how they connect, what you would look for in their code implementations.

---

## CHAT 5 — Project 2: Multimodal RAG

### Purpose
Three chats covering the 5-milestone project in clusters: M1-M2 in one
chat, M3-M4 in another, M5 alone. The project builds a system where a
student can ask questions about NCERT textbook content (including diagrams)
and get answers grounded in both text and images.

Per v5.1, this project runs in Weeks 7-8 of personal time.

Milestones:
M1 — PDF ingestion, page images + text, diagram detection (~7 hrs)
M2 — VLM captioning for every diagram and figure (~7 hrs)
M3 — Vector store indexing, query function (~7 hrs)
M4 — Query interface: English/Hindi to retrieve to LLM answer (~7 hrs)
M5 — Evaluation: 50-question test set, recall@5, answer relevance, README (~7 hrs)

### What Claude tracks in this chat
- Architectural decisions made in earlier milestones
- The retrieval design (what is indexed, how queries work)
- Evaluation methodology you have committed to

### Model
**Sonnet 4.6**

### Files to Upload
`learning-prompt-v3-1.md` + `v5-FILE1-CURRICULUM.md`

### Opening Prompt
```
Files uploaded: Learning Prompt v3.1 + Curriculum (FILE 1).
Project 2 spec is in FILE 1 under "Project 2: Multimodal RAG for Indian Educational Content."
Read both. Review only — do not design the system for me.

Week: [X] | Rung: [X] | This chat covers: M[X]-M[Y]

[Only include if this is not the first Project 2 chat:]
Carrying forward: [paste SHAKY + OPEN THREADS from previous milestone summary]
```

### Restart Trigger
After M2 complete → new chat for M3-M4.
After M4 complete → new chat for M5.
Three chats total.

---

## CHAT 6 — Project 3: VLM Fine-Tuning

### Purpose
One chat per milestone across the 5-milestone project. The most
technically dense project in the roadmap. M3 (full training + debugging)
and M4 (evaluation) use Opus — the diagnostic reasoning required for NaN
losses, memory errors, and degrading performance is where it earns its cost.

Per v5.1, this project runs in Weeks 9-10 of personal time.

Milestones:
M1 — Dataset curation: 500-1000 image-QA pairs (~10 hrs) — Sonnet
M2 — Fine-tuning setup: LoRA config, 100-step verification run (~10 hrs) — Sonnet
M3 — Full training + debugging broken runs (~10 hrs) — Opus
M4 — Evaluation: automated metrics + manual eval + failure analysis (~10 hrs) — Opus
M5 — Inference optimisation + quantisation + blog post (~5 hrs) — Sonnet

### What Claude tracks in this chat
- Training config decisions made in M2 (model, LoRA rank, lr, batch size)
- Dataset characteristics that might explain model behaviour
- Loss curve history and what was tried to fix issues

### Model
**Sonnet 4.6 for M1, M2, M5 | Opus 4.6 for M3, M4**

### Files to Upload
`learning-prompt-v3-1.md` + `v5-FILE1-CURRICULUM.md`

### Opening Prompt
```
Files uploaded: Learning Prompt v3.1 + Curriculum (FILE 1).
Project 3 spec is in FILE 1 under "Project 3: Fine-Tuning a VLM for Indian Visual QA."
Read both. Review and diagnostic support only — do not rewrite my code or config.

Week: [X] | Rung: [X] | Milestone: M[X] — [name]

[Only include if M2 or later:]
Carrying forward: [paste SHAKY + OPEN THREADS from last milestone's summary]
```

### Restart Trigger
After each milestone — 5 chats total. For M3 especially: if a debugging
session ends without resolution, run the summary prompt and start a fresh
M3 chat with the summary as context rather than letting unresolved threads
accumulate across sessions.

---

## CHAT 7 — Quick Lookup

### Purpose
Fast, disposable, single-topic exchanges. Syntax questions, API flags,
quick concept checks, "which one should I use" decisions. If you can
resolve it in 1-3 exchanges, it belongs here. If it needs your roadmap
or project context, it belongs in another chat.

No files, no preamble. Just ask.

### What Claude tracks in this chat
Nothing. Disposable by design.

### Model
**Haiku 4.5**
*(Significantly cheaper and faster. If a Quick Lookup grows complex,
switch to the right chat rather than upgrading the model mid-conversation.)*

### Files to Upload
None.

### Opening Prompt
```
[Ask directly. No preamble.]
```

### Restart Trigger
After 10-15 exchanges, or when questions have shifted topic enough that
a new chat is cleaner. Do not overthink it.

---

## CHAT 8 — Phase Transition / Architecture Decisions

### Purpose
Used at two moments: (1) when you finish a major phase and are deciding
whether you are genuinely ready to move on, and (2) when you face a
significant architectural decision in a project where the trade-offs are
non-trivial.

For phase transitions: you come with an honest account of what you built,
what is solid, what is shaky. Claude assesses readiness directly — no
encouragement, no softening. One concrete stress-test before you proceed.

For architectural decisions: you describe the decision, the options, and
your current thinking. Claude helps you think through trade-offs — it
does not make the decision for you.

Per v5.1, the four natural phase boundaries are:
- End of Week 2: Phase 1 + Karpathy complete, moving to PyTorch and GenAI
- End of Week 4: Onboarding complete, moving to Sarvam track
- End of Week 8: VLM deep dive complete, moving to fine-tuning
- End of Week 11: Sarvam-ready, moving to full stack

### What Claude tracks in this chat
- The full picture of where you are across all three files
- Your self-assessment vs. what the evidence shows
- What the next phase demands and whether the current state meets it

### Model
**Opus 4.6**

### Files to Upload
`learning-prompt-v3-1.md` + `v5-FILE1-CURRICULUM.md` + `v5-1-RESTRUCTURED-WEEKLY-PLAN.md`

### Opening Prompt
```
Files uploaded: Learning Prompt v3.1 + Curriculum (FILE 1) + Weekly Plan v5.1.
Read all three. This is a phase transition review / architectural decision chat.

Completing: [week range, e.g. "Weeks 1-4, onboarding"]
Starting: [next phase or track]
Rung: [X]

What I built (concrete outputs only):
[2-4 lines — mini-projects, portfolio projects, contributions]

Confident on:
[2-3 things I can explain without notes]

Shaky on:
[1-2 honest gaps]

Assess whether I am ready to move on. Be direct, not encouraging.
Flag anything that will cause problems in the next phase.
Give me one concrete thing to stress-test before I proceed.
```

### Restart Trigger
One per transition or decision. Self-contained by nature.

---

## CHAT 9 — Open Source Contributions

### Purpose
Active from Week 5 onwards per v5.1. One chat per PR. You have found
an issue, understood the relevant codebase section yourself, and have
a proposed fix or contribution. Claude reviews your diagnosis and
approach — it does not read the codebase for you or produce the fix.

Target repos: vLLM, Hugging Face Transformers, LLaVA or InternVL (bugs
found during Project 3), PaddleOCR (Indic improvements from Project 1).
Goal: 3-5 merged PRs before applying to Sarvam.

### What Claude tracks in this chat
- Your understanding of the relevant codebase section
- Your diagnosis of the bug or proposed feature
- Where your reasoning has a gap

### Model
**Sonnet 4.6**

### Files to Upload
`learning-prompt-v3-1.md`

### Opening Prompt
```
File uploaded: Learning Prompt v3.1. Read the Independence Ladder.
I am at Rung [X] — treat me accordingly.

Repo: [name] | Issue: [title or link]

What I understand about the bug or feature:
[2-4 lines in your own words]

What I have tried or written:
[paste code snippet or describe your approach]

My question: [one sentence]
```

### Restart Trigger
One per PR. The summary becomes the record of the contribution.

---

## CHAT 10 — Production Codebase (Office Learning)

### Purpose
New in v3.1. The office is now a distinct learning context — reading
production code, tracing pipelines, experimenting, and extracting
mini-projects — that has no home in any other chat. Use this chat during
office hours or in the evening when you need to process something from
the codebase.

Use this chat for:
- Understanding a pattern or concept from production code you have been reading
- Thinking through your approach to tracing a new pipeline
- Comparing your mini-project rebuild with what the production code does
- Debugging code you wrote at the office during experimentation

**Critical confidentiality rule from v3.1:** Do not paste production
code into this chat until you have confirmed with your team lead that
it is allowed. Instead, describe the pattern or concept you are confused
about without sharing the actual code. "I saw a function that uses yield
to return items one at a time — I do not understand why they used a
generator instead of returning the full list" is always safe to ask.
Pasting the actual function with your company's variable names may not be.

If external AI is not allowed: use Ollama locally
(`ollama pull qwen2.5-coder:32b`) for all production code questions.
Use this chat only for your home-built mini-projects and patterns.

This chat is NOT for:
- Foundation study questions from books and courses — Chat 1
- Reviewing practice code you wrote at home — Chat 2
- Portfolio project work — Chats 3, 5, 6

### What Claude tracks in this chat
- Which pipelines and modules you have traced so far this week
- Mini-projects you have extracted and are working on
- Patterns from production you have seen but do not yet understand

### Model
**Sonnet 4.6**

### Files to Upload
`learning-prompt-v3-1.md`

### Opening Prompt
```
File uploaded: Learning Prompt v3.1. Read it — specifically the
Production Code Learning Protocol, Mini-Project Extraction Protocol,
and the Confidentiality section.

This chat is for my office learning context: production code patterns,
mini-project rebuilds, and codebase understanding. I will describe
patterns and concepts — I will not paste proprietary code unless my
team has confirmed external AI is allowed. When I share code it will
be either my own mini-project rebuild or a safe anonymised snippet.

Week: [X] | Rung: [X]
Current focus: [e.g. "Tracing the data preprocessing pipeline" / "Rebuilding Mini-Project #2" / "Comparing my MP #1 to the production version"]

[Only include if restarting from a previous chat summary:]
Carrying forward: [paste SHAKY + OPEN THREADS from last summary]
```

### Restart Trigger
End of each office week during onboarding (Weeks 1-4) — same cadence as
Chat 1. After onboarding, open as needed when office work raises questions
worth discussing. The weekly summary should capture: which pipelines you
traced, which mini-projects were extracted and rebuilt, what patterns you
still do not fully understand, and what office confusion drove your evening
study that week.

---

## CHAT 11 — Deadline-Driven Project Sprint

### Purpose
For when a project has a hard external deadline — a demo, a submission,
an interview, a PR that needs to merge by a specific date. This chat
runs differently from the milestone-based project chats: instead of one
milestone per chat with careful pacing, you work in compressed time-boxed
sprints and Claude's job is to help you make the right trade-off decisions
fast and unblock you quickly.

The key difference from normal project chats: Claude's role is explicitly
to help you cut scope intelligently and get to a working, demonstrable
state as fast as possible. This is not the context for learning deeply —
it is the context for shipping. The depth comes after the deadline.

When to use:
- You have a working deadline for a portfolio project
- You need a demo-ready version of something in 24-48 hours
- A specific feature or fix needs to land before a meeting or interview
- Office work has a hard deadline and you are hitting a blocker

This chat is NOT for:
- Regular project work without a deadline — use the appropriate project chat
- Outsourcing the thinking — you still own the design and code
- Getting Claude to write the implementation — it unblocks, it does not build

### What Claude tracks in this chat
- The deadline and what good enough looks like by that deadline
- What was cut and why (so the summary reflects real trade-offs made)
- Where you got unblocked and how — useful for post-deadline reflection

### Model
**Sonnet 4.6**

### Files to Upload
`learning-prompt-v3-1.md` + `v5-FILE1-CURRICULUM.md`
*(FILE 1 only needed if the sprint involves a portfolio project.
For office deadlines, just upload the learning prompt.)*

### Opening Prompt
```
File uploaded: Learning Prompt v3.1 [+ Curriculum FILE 1 if portfolio project].
Read the learning prompt — specifically the Independence Ladder.

This is a deadline-driven sprint. Normal pacing rules are adjusted:
your job is to unblock me fast and help me make scope trade-offs,
not to slow me down with review questions. You still do not write
code for me, but you can give more direct guidance than usual.

Project / task: [what you are building or fixing]
Hard deadline: [date and time, or "in X hours"]
Current state: [what exists and works right now]
Blocking issue: [what is stopping you from moving forward]
What done looks like: [the minimum that meets the deadline]

What I need right now: [unblock me on X / help me decide between A and B / review this specific piece]
```

### Restart Trigger
After the deadline is met and the sprint is over. Run the summary prompt
before closing. This is important: the summary captures what trade-offs
were made, what was cut, and what technical debt was created. That
information should feed back into the relevant project chat when you
return to the work post-deadline.

---
---

# SUMMARY PROMPT

*Paste this as the final message in any chat before you close it.*
*The output is your learning log entry. Save every one.*

**How to save:** In your `/learning-log/` folder, use the subfolder
matching the chat type. Name each file `YYYY-MM-DD-[descriptor].md`

```
learning-log/
  daily-learning/             2026-04-14-week1.md
  code-review/                2026-04-18-week1-review.md
  project-1-doc-digitisation/ 2026-04-20-M2.md
  paper-reading/              2026-04-21-ViT-CLIP.md
  project-2-multimodal-rag/   2026-05-10-M1-M2.md
  project-3-vlm-finetuning/   2026-05-25-M3-training.md
  quick-lookup/               (do not save these — disposable)
  phase-transitions/          2026-04-28-week4-to-sarvam.md
  open-source/                2026-05-15-vllm-pr-4821.md
  production-codebase/        2026-04-11-week1-office.md
  deadline-sprints/           2026-04-27-project1-demo.md
```

Over months this folder becomes your growth record — searchable,
reviewable, and the source of genuine insight into your patterns.

---

```
Generate a summary of this chat as a structured log entry.
Be specific and honest — this is a record, not a performance.

CHAT TYPE: [you fill: e.g. Daily Learning / Production Codebase / Project 3 M3]
DATE CLOSED: [you fill: YYYY-MM-DD]
WEEK: [you fill: e.g. Week 2]
RUNG AT CLOSE: [you fill: 1 / 2 / 3 / 4]

---

WHAT WE COVERED:
[3-6 bullets — what actually happened, not what was planned.
Be specific: resource names, concepts, patterns seen in code,
bugs hit, design decisions made, mini-projects worked on.]

SOLID (no need to revisit):
[2-4 bullets — things I can explain or do without notes]

SHAKY (carry forward to next chat):
[1-3 bullets — genuine gaps, things that did not click,
or things I understood here but will not remember in a week]

OPEN THREADS:
[Unresolved questions, half-finished debugging, deferred decisions,
patterns from the codebase I still do not understand.
Write "None." if the chat closed cleanly.]

EFFICIENCY NOTE:
[1-2 sentences. Honest reflection on how this chat went.
Did I over-rely on Claude? Ask questions before trying?
Did context degrade before I restarted? Did I paste code I should not have?
This field exists to surface patterns in your working style over time.]

NEXT ACTION:
[One sentence. Exactly where to pick up.
e.g. "Evening study: read Fluent Python generators — saw yield in office today."
or "Project 1 M4: VLM extraction next, Tesseract baseline is done."
or "Mini-Project #3: interface extracted Friday, build it Saturday morning."]

TAGS:
[3-6 domain or tool tags from the Knowledge Tagging System in the learning prompt.
e.g. Python, PyTorch, VLMs, Fine-Tuning, Evaluation, OpenCV, ProductionCode]
```

---

*The four [you fill] fields at the top are intentional. Filling them
yourself — even in 10 seconds — forces a moment of self-assessment that
copy-pasting cannot replicate. Everything else Claude generates.*

---
---

# RESTART DECISION GUIDE

Any one of these is sufficient reason to run the Summary Prompt and start fresh.

**Definite restart:**
- The natural boundary has been hit (week end, milestone complete, paper cluster done, PR submitted)
- Claude gives an answer that contradicts or ignores something established earlier in the same chat
- You are re-explaining your setup, rung, or week to a chat that should already have that context
- The chat is over 50 exchanges for a study or office chat, or over 30 exchanges for a code-heavy or debugging chat

**Consider restarting:**
- The topic has shifted enough that the original files are no longer the right context
- You feel like you are managing the chat's memory rather than doing the actual work

**Do not restart just because:**
- The chat is long but still working correctly
- You have not hit the natural boundary yet — finish the milestone or week first

---

# MODEL DECISION GUIDE

**Sonnet 4.6** — default for everything. Daily learning, code review, all
project milestones except M3/M4 of Project 3, production codebase, open
source, deadline sprints. Handles 85% of your interactions well.

**Opus 4.6** — when the task requires holding many interacting variables
simultaneously: paper reading (cross-paper architectural reasoning),
Project 3 M3/M4 (debugging training runs with multiple simultaneous failure
modes), and phase transition reviews (integrating your full learning state
across all three files). Do not use by default — Sonnet is not a downgrade
for most tasks. Opus earns its cost in specific, identifiable situations.

**Haiku 4.5** — Quick Lookup only. If a Quick Lookup turns complex, switch
to the right chat and model rather than escalating mid-conversation.

---

*End of document.*
*Learning Prompt: v3.1 | Weekly Plan: v5.1 | Curriculum: v5 FILE 1 (unchanged)*
*Folder: /learning-log/ with 10 subfolders (see Summary Prompt section)*
