# Weekly Plan: Office Onboarding + Home Study
## Production Code at Office + Foundations at Home

```
USE CASE:       You have a job. Office hours = production code.
                Foundation study = mornings, evenings, weekends.
COMPANION:      Curriculum file (same resources, corrected time estimates)
                Resource Registry (same vetting)
                Learning Prompt v3.1

NOTE ON TIME ESTIMATES:
  All book reading times reflect ACTIVE READING: reading + typing
  every code example + writing a practice script after each chapter.
  Video/course/paper times are accurate as-is.
```

---

## Restructured Time Budget

```
DAILY SCHEDULE (WEEKDAYS):

  5:00 AM - 7:00 AM .... FOUNDATION STUDY (2 hrs realistic)
    Books, courses, videos from the Roadmap v5 curriculum.
    You lose ~30 min to waking up, coffee, settling in.
    The 5:00-7:00 block is your PROTECTED deep reading time.
    At 7:00 you stop, eat breakfast, get changed, leave.

  [7:00 AM - 9:30 AM ... Breakfast + get ready + commute]

  9:30 AM - 6:00 PM .... PRODUCTION CODE at office (8.5 hrs)
    Read the team's codebase. Understand it. Experiment.
    Break things on purpose. Rebuild parts from scratch.
    Extract mini-projects. Integrate changes.
    NO BOOK READING during office hours.

  [6:00 PM - 7:30 PM ... Commute + freshen up + dinner]

  7:30 PM - 9:30 PM .... FOUNDATION STUDY + PRACTICE (2 hrs)
    You're tired. This block is for LIGHTER material:
    → Videos (3Blue1Brown, Karpathy, DLAI short courses)
    → Targeted lookups based on what confused you at office
    → 15-20 min coding practice (Exercism)
    → NOT deep book reading — save that for mornings/weekends

WEEKENDS (this is where the real volume happens):
  Saturday: 12-14 hrs deep foundation study + portfolio projects
    5:00 AM - 12:00 PM ... Deep study block (7 hrs with breaks)
    [12:00 - 1:00 PM lunch]
    1:00 PM - 7:00 PM .... Projects + continued study (6 hrs)
    [Evening off or light review]

  Sunday: 12-14 hrs deep foundation study + portfolio projects
    Same structure as Saturday. Slightly lighter if needed.
    Last hour: review the week, plan the next week.

  Total weekend: ~26 hrs

WEEKLY TOTALS:
  Mornings:   2 × 5 = 10 hrs ....... foundation study (deep reading)
  Office:     8.5 × 5 = 42.5 hrs ... production code
  Evenings:   2 × 5 = 10 hrs ....... light study + practice
  Weekends:   26 hrs ............... deep study + projects
  ─────────────────────────────────────
  TOTAL:      ~88.5 hrs/week

  Foundation study:    ~46 hrs/week (mornings + evenings + weekends)
  Production code:     ~42.5 hrs/week (office)

  The weekends carry the foundation study. Weekday mornings and
  evenings are supplementary — important but not the main engine.
  If a weekday evening is a total wash (you're exhausted), the
  weekend absorbs it. If a morning is disrupted, same thing.
  The weekends are non-negotiable.
```

---

## Why This Is Better: The Dual-Exposure Effect

```
OLD PLAN (v5):
  Week 1 office: Read Robust Python all day. Read Grokking all day.
  Week 2 office: Watch DLAI Math all day.
  → You read for 2 weeks before touching real code.
  → By Week 3 you've forgotten half of what you read.
  → No connection between theory and practice.

NEW PLAN (v5.1):
  Week 1 morning: Read Robust Python Ch 1-4 (type hints, annotations)
  Week 1 office:  Open team's codebase. See type hints EVERYWHERE.
                  "Oh, THAT'S what the book was talking about."
                  Trace a pipeline. See decorators, dataclasses, generators.
                  Get confused. Write down what confused you.
  Week 1 evening: Read Robust Python Ch 5-7 (the exact things that
                  confused you at the office that day).
  → Theory and practice reinforce each other DAILY.
  → Confusion at the office drives targeted evening study.
  → Evening study makes the next day at the office more productive.
```

---

## WEEK 1: Python + Math Intuition + First Codebase Contact

### Early Mornings (Mon-Fri, 10 hrs)

```
  Mon 5:00-7:00: Robust Python Ch 1-2 (types, annotations) ..... 2 hrs
  Tue 5:00-7:00: Robust Python Ch 3-4 .......................... 2 hrs
  Wed 5:00-7:00: Robust Python Ch 5-6 (enums, dataclasses) ..... 2 hrs
  Thu 5:00-7:00: Robust Python Ch 7 (classes) .................. 2 hrs
  Fri 5:00-7:00: Robust Python Ch 8-9 (extensibility) .......... 2 hrs

  Note: Robust Python Ch 1-14 = ~23 hrs. At 2 hrs/morning you cover
  ~10 hrs in Week 1 mornings. The rest continues into Week 2 mornings
  and Weekend 1. This is normal — weekends absorb the overflow.
```

### Office Time (Mon-Fri, 42.5 hrs) — PRODUCTION CODE

```
  Mon (8.5 hrs): TOP-DOWN SURVEY
    - Get access to the team's main project repository
    - Read the README and any architecture/design docs
    - Map the directory structure on paper or whiteboard
    - Run the project. See what it does end-to-end.
    - Identify: what language? What framework? What libraries?
    - Write a 1-page "what I think this project does" summary

  Tue (8.5 hrs): TRACE PIPELINE #1
    - Pick the main flow (e.g., a request → response pipeline)
    - Start at the entry point. Follow it file by file.
    - For every function/class: read it, guess what it does,
      look up unfamiliar libraries in their official docs.
    - Add YOUR understanding as comments (don't commit these)
    - Note every pattern you don't recognise:
      "What is this @decorator doing?"
      "Why are they using yield here?"
      "What is this config pattern?"
    - These notes drive your evening study tonight.

  Wed (8.5 hrs): TRACE PIPELINE #1 continued + EXPERIMENT
    - Finish tracing the first pipeline
    - Start experimenting:
      → Add print statements at every step. Run it. Read output.
      → Change a parameter. What happens?
      → Remove an error handler. What breaks? What error message?
      → Try an alternative approach to one small function.
    - Write a 1-page summary: "How Pipeline #1 works"

  Thu (8.5 hrs): TRACE PIPELINE #2 + DEEP DIVE
    - Pick a second flow or module
    - Trace it the same way
    - Deep dive into 2-3 functions you find interesting:
      → Understand every line
      → Look up every library call in the docs
      → Ask yourself: "Could I write this from scratch?"
      → If no: identify exactly which part you couldn't write

  Fri (8.5 hrs): EXTRACT MINI-PROJECT #1
    - Identify one self-contained piece (e.g., data preprocessing,
      a utility module, an API endpoint)
    - Write down its INTERFACE: what goes in, what comes out
    - DO NOT copy the code. Just the interface definition.
    - You will rebuild this from scratch at home this weekend.
    - Spend remaining time continuing to explore the codebase.
```

### Evenings (Mon-Fri, 10 hrs)

```
  Mon 7:30-9:30: 3Blue1Brown Essence of LA — videos 1-8 ....... 2 hrs
                  (videos are ideal evening content — visual, low effort)

  Tue 7:30-9:30: 3Blue1Brown Essence of LA — videos 9-16 ...... 2 hrs

  Wed 7:30-9:30: TARGETED STUDY based on office confusion:
                  Look up every pattern you noted at the office.
                  If you saw decorators → note for weekend Fluent Python
                  If you saw pytest → read pytest Ch 1-2 ......... 1.5 hrs
                  Exercism: 2 easy Python exercises .............. 0.5 hrs

  Thu 7:30-9:30: 3Blue1Brown Essence of Calculus — videos 1-6 .. 1.5 hrs
                  Exercism: 2 easy Python exercises .............. 0.5 hrs

  Fri 7:30-9:30: 3Blue1Brown Essence of Calculus — videos 7-12 . 1.5 hrs
                  Exercism: 2 easy Python exercises .............. 0.5 hrs
```

### Weekend (26 hrs)

```
  Saturday (13 hrs):
    5:00-8:00:  Robust Python Ch 10-12 ........................ 3 hrs
    8:00-8:30:  Breakfast break
    8:30-12:30: Robust Python Ch 13-14 + Ch 15-16, 20 (finish) 4 hrs
    12:30-1:30: Lunch
    1:30-5:30:  Grokking Algorithms Ch 1-8 .................... 4 hrs
    5:30-7:30:  BUILD MINI-PROJECT #1 from scratch at home:
                Use only the interface definition from Friday.
                DO NOT look at the production code. ............. 2 hrs

  Sunday (13 hrs):
    5:00-9:00:  Grokking Algorithms Ch 9-11 (finish, ~2 hrs)
                + DLAI Math Spec — Course 1, Weeks 1-2 ......... 4 hrs
    9:00-9:30:  Breakfast break
    9:30-1:30:  DLAI Math Spec — Course 1, Weeks 3-4 +
                Course 2, Weeks 1-2 ............................ 4 hrs
    1:30-2:30:  Lunch
    2:30-5:30:  Continue Mini-Project #1 or finish it.
                Write COMPARISON.md if done. .................... 3 hrs
    5:30-7:30:  Clean Code Ch 1-6 .............................. 2 hrs
```

### Week 1 Checkpoint

```
  FOUNDATION STUDY COMPLETED:
    ✓ Robust Python — COMPLETE (~27 hrs across mornings + weekend)
    ✓ 3Blue1Brown LA + Calculus — COMPLETE (6.5 hrs across evenings)
    ✓ Grokking Algorithms — COMPLETE (~10 hrs, weekend)
    ✓ DLAI Math Course 1 — COMPLETE + Course 2 STARTED (weekend)
    ✓ Clean Code Ch 1-6 — DONE (weekend)
    ✓ Exercism: ~6 exercises done (evenings)
    ✓ Mini-Project #1 — v1 built from scratch

    NOT YET DONE (carries into Week 2):
    → Fluent Python (starts Week 2)
    → DLAI Math Course 2 (finish Week 2)
    → pytest (starts Week 2)

  PRODUCTION CODE COMPLETED:
    ✓ Codebase survey — understand project structure
    ✓ Pipeline #1 traced end-to-end
    ✓ Pipeline #2 traced
    ✓ Experimentation: changed params, broke things, observed errors
    ✓ Mini-Project #1 interface extracted

  HOURS: ~88 hrs (10 morning + 42.5 office + 10 evening + 26 weekend)
```

---

## WEEK 2: Math + Python Depth + Deeper Code Exploration

### Early Mornings (10 hrs)

```
  Mon 5:00-7:00: DLAI Math Course 2 — Weeks 3-4 (finish) ....... 2 hrs
  Tue 5:00-7:00: Fluent Python Part I (Data Structures) start .. 2 hrs
  Wed 5:00-7:00: Fluent Python Part I continued ................ 2 hrs
  Thu 5:00-7:00: Fluent Python Part II (Functions) ............. 2 hrs
  Fri 5:00-7:00: Fluent Python Part II continued ............... 2 hrs

  Note: Fluent Python = ~30 hrs total. You'll cover ~10 hrs in Week 2
  mornings. The rest continues on Weekend 2.
```

### Office Time (42.5 hrs) — PRODUCTION CODE

```
  Mon (8.5 hrs): BRING BACK Mini-Project #1
    - Compare your version with the production code
    - Note every difference. For each: WHY is theirs different?
    - Ask colleagues about patterns you don't understand
    - Continue exploring new parts of the codebase

  Tue (8.5 hrs): DEEP DIVE into a second module
    - Pick something more complex (e.g., the ML pipeline,
      the data processing layer, the API layer)
    - Trace it. Understand every function.
    - Experiment: break it, fix it, try alternatives.

  Wed (8.5 hrs): EXTRACT Mini-Project #2
    - Pick a different module than MP #1
    - Write down the interface
    - Start rebuilding AT THE OFFICE this time (you have more
      comfort with coding now — try it in real time)

  Thu (8.5 hrs): Continue Mini-Project #2 at office
    - Finish your version. Run it. Test it.
    - Compare with production version immediately.
    - Start making small changes to the REAL codebase:
      improve an error message, add a docstring, write a test

  Fri (8.5 hrs): FIRST REAL CONTRIBUTION attempt
    - Pick the smallest possible improvement to the codebase
    - Implement it. Write a test for it. Submit for review.
    - If team uses git: learn the branch → commit → PR workflow
    - Extract Mini-Project #3 interface for the weekend
```

### Evenings (10 hrs)

```
  Mon 7:30-9:30: pytest Ch 1-3 (getting started, fixtures) ..... 2 hrs
  Tue 7:30-9:30: pytest Ch 4-6 (parametrize, markers, mocking) . 2 hrs
  Wed 7:30-9:30: pytest Ch 7+ (plugins, CI) .................... 2 hrs
  Thu 7:30-9:30: Clean Code Ch 7-10 (finish) ................... 2 hrs
  Fri 7:30-9:30: Jay Alammar blog — Illustrated Transformer +
                  Illustrated GPT-2 ............................. 2 hrs
```

### Weekend (26 hrs)

```
  Saturday (13 hrs):
    5:00-8:00:  Fluent Python Part III (Classes, Protocols) .... 3 hrs
    8:00-8:30:  Breakfast
    8:30-12:30: Fluent Python Part IV (Control Flow —
                generators, iterators, async) .................. 4 hrs
    12:30-1:30: Lunch
    1:30-5:30:  Fluent Python Part V (Metaprogramming, ~2 hrs)
                + Karpathy micrograd video — code along ........ 4 hrs
    5:30-7:30:  Build Mini-Project #3 from scratch ............. 2 hrs

  Sunday (13 hrs):
    5:00-9:00:  Karpathy — makemore 1 + 2 (code along) ........ 4 hrs
    9:00-9:30:  Breakfast
    9:30-12:30: Karpathy — makemore 3 + 4 ..................... 3 hrs
    12:30-1:30: Lunch
    1:30-4:30:  Karpathy — building GPT from scratch ........... 3 hrs
    4:30-7:30:  Karpathy — GPT continued + tokenization +
                nanoGPT source reading ......................... 3 hrs
```

### Week 2 Checkpoint — PHASE 1 COMPLETE + KARPATHY COMPLETE

```
  FOUNDATION STUDY:
    ✓ Robust Python — COMPLETE (Week 1)
    ✓ Fluent Python — COMPLETE (~30 hrs across Week 2 mornings + weekend)
    ✓ 3Blue1Brown LA + Calculus — COMPLETE (Week 1 evenings)
    ✓ Grokking Algorithms — COMPLETE (Week 1 weekend)
    ✓ DLAI Math Courses 1-2 — COMPLETE (across Weekends 1-2)
    ✓ pytest — COMPLETE (~10 hrs, Week 2 evenings)
    ✓ Clean Code — COMPLETE (Week 1 weekend + Week 2 evenings)
    ✓ Karpathy Zero to Hero — COMPLETE (~18 hrs, Weekend 2)
    ✓ nanoGPT source reading — COMPLETE (Weekend 2)
    ✓ Jay Alammar blog posts — COMPLETE (Week 2 evening)

  PRODUCTION CODE:
    ✓ 3+ mini-projects extracted and rebuilt from scratch
    ✓ Full understanding of 2+ pipelines
    ✓ First real contributions submitted
    ✓ Comfortable navigating the codebase

  RUNNING TOTAL: ~176 hrs (88 × 2 weeks)

  ★ Phase 1 COMPLETE + Phase 2A COMPLETE by end of Week 2.
```

---

## WEEK 3: PyTorch + Generative Models + Office Experimentation

### Early Mornings (10 hrs)

```
  Mon 5:00-7:00: Mark Liu Ch 1-2 (GenAI intro, DL with PyTorch) 2 hrs
  Tue 5:00-7:00: Mark Liu Ch 3-4 (DL continued, GANs) ......... 2 hrs
  Wed 5:00-7:00: Mark Liu Ch 5-6 (CycleGAN, VAEs) ............. 2 hrs
  Thu 5:00-7:00: Mark Liu Ch 7-8 (image gen finish, RNNs) ...... 2 hrs
  Fri 5:00-7:00: Mark Liu Ch 9-10 (attention, Transformer) ..... 2 hrs

  Note: Mark Liu = ~28 hrs total. You'll cover ~10 hrs in mornings.
  Remaining ~18 hrs continues in evenings + Weekend 3.
```

### Office Time (42.5 hrs)

```
  Mon-Wed: Continue codebase exploration + experiments
    - Trace more complex modules
    - Break more things on purpose
    - Try alternative implementations
    - Extract Mini-Projects #4 and #5

  Thu-Fri: Start contributing more actively
    - Pick 2-3 small improvements
    - Write tests for untested functions
    - Improve error handling or logging
    - Ask team for a small task you can own
```

### Evenings (10 hrs)

```
  Mon 7:30-9:30: Mark Liu Ch 11-12 (GPT, text generation) ...... 2 hrs
  Tue 7:30-9:30: Mark Liu Ch 13-14 (music gen, diffusion) ...... 2 hrs
  Wed 7:30-9:30: Mark Liu Ch 15-16 (diffusion cont, LangChain) . 2 hrs
  Thu 7:30-9:30: Hands-On LLMs (Alammar book) Ch 1-2 .......... 2 hrs
  Fri 7:30-9:30: Hands-On LLMs Ch 3-4 ......................... 2 hrs
```

### Weekend (26 hrs)

```
  Saturday (13 hrs):
    5:00-8:00:  Hands-On LLMs Ch 5-8 .......................... 3 hrs
    8:00-8:30:  Breakfast
    8:30-12:30: Hands-On LLMs Ch 9-end (finish, ~18 hrs total) 3 hrs
                ViT paper — abstract + method section .......... 1 hr ★
    12:30-1:30: Lunch
    1:30-5:30:  Elgendy "DL for Vision Systems" Ch 5-6
                (CNN architectures, transfer learning) ......... 4 hrs
    5:30-7:30:  Elgendy Ch 7 (object detection: YOLO, R-CNN) .. 2 hrs

  Sunday (13 hrs):
    5:00-9:00:  Elgendy Ch 8-10 (GANs, style transfer,
                visual embeddings) — selective .................. 4 hrs
    9:00-9:30:  Breakfast
    9:30-12:30: CS231n Assignment 1 (image classif, kNN) ....... 3 hrs
    12:30-1:30: Lunch
    1:30-4:30:  CS231n Assignment 2 (batch norm, dropout, CNNs)  3 hrs
    4:30-7:30:  OpenCV tutorials — core operations + practice .. 3 hrs
```

---

## WEEK 4: LLM Engineering + VLM Papers + Project Planning

### Early Mornings (10 hrs)

```
  Mon 5:00-7:00: Chip Huyen "AI Engineering" Ch 1-2 ........... 2 hrs
  Tue 5:00-7:00: Chip Huyen Ch 3 (evaluation methodology) ..... 2 hrs
  Wed 5:00-7:00: Chip Huyen Ch 4-5 (eval systems, prompt eng) . 2 hrs
  Thu 5:00-7:00: Chip Huyen Ch 6 (RAG and Agents) ............. 2 hrs
  Fri 5:00-7:00: Chip Huyen Ch 7 (fine-tuning, LoRA) .......... 2 hrs

  Note: Chip Huyen = ~20 hrs total. You'll cover ~10 hrs in mornings.
  Remaining chapters (8-10) continue in evenings + Weekend 4.
```

### Office Time (42.5 hrs)

```
  Mon-Fri: FULL PRODUCTION CODE WORK
    By Week 4, you should be actively contributing:
    - Own a small feature or improvement
    - Write tests for existing untested code
    - Improve error handling in a module you understand well
    - Pair with a colleague on a task
    - Extract Mini-Projects #6 and #7 from new parts of codebase
    - If team works with ML/LLM pipelines: trace the ML-specific
      code and experiment with it (this directly supports your
      Chip Huyen reading from mornings)
```

### Evenings (10 hrs)

```
  Mon 7:30-9:30: Chip Huyen Ch 8-9 (dataset eng, inference) ... 2 hrs
  Tue 7:30-9:30: Chip Huyen Ch 10 (architecture, feedback) .... 1 hr
                  DLAI "How Diffusion Models Work" ............. 1 hr ★
  Wed 7:30-9:30: CLIP paper — method section .................. 1.5 hrs ★
                  Alammar "Illustrated Stable Diffusion" ....... 0.5 hrs ★
  Thu 7:30-9:30: LLaVA paper — method section ................. 1.5 hrs ★
                  DLAI "Prompt Vision Models" .................. 0.5 hrs ★
  Fri 7:30-9:30: DLAI "Building Multimodal Search and RAG" .... 1.5 hrs ★
                  Project 1 planning — set up repo, define scope 0.5 hrs
```

### Weekend (26 hrs)

```
  Saturday (13 hrs):
    5:00-8:00:  DLAI "Building and Evaluating Advanced RAG" ... 1.5 hrs
                DLAI "Preprocessing Unstructured Data" ........ 1.5 hrs
    8:00-8:30:  Breakfast
    8:30-12:30: Labonne refs — LoRA insights, quantization .... 2 hrs
                DLAI "Building Apps with Vector DBs" .......... 1.5 hrs
                Project 1 — M1 (scope, collect samples) ....... 1 hr
    12:30-1:30: Lunch
    1:30-5:30:  Project 1 — M1 finish + M2 (OpenCV
                preprocessing pipeline) ....................... 4 hrs
    5:30-7:30:  Project 1 — M3 start (OCR layer) .............. 2 hrs

  Sunday (13 hrs):
    5:00-9:00:  Project 1 — M3 finish + M4 (VLM extraction +
                evaluation script against ground truth) ........ 4 hrs
    9:00-9:30:  Breakfast
    9:30-1:30:  Project 1 — M5 (FastAPI + tests + README +
                push to GitHub) ............................... 4 hrs
    1:30-2:30:  Lunch
    2:30-5:30:  VLM book (O'Reilly early release) Ch 1-2 OR
                HF VLM tutorials if book incomplete ............ 3 hrs ★
    5:30-7:30:  Review Week 4. Update all skill levels.
                Plan the post-onboarding track. ................ 2 hrs
```

### Week 4 Checkpoint

```
  FOUNDATION STUDY:
    ✓ Phase 1 — COMPLETE (Python, math, testing, DSA)
    ✓ Karpathy Zero to Hero — COMPLETE (Weekend 2)
    ✓ Mark Liu GenAI with PyTorch — COMPLETE (Week 3)
    ✓ Hands-On LLMs — COMPLETE (Week 3)
    ✓ Elgendy DL for Vision Systems — COMPLETE (Weekend 3)
    ✓ CS231n Assignments 1-2 — COMPLETE (Weekend 3)
    ✓ OpenCV — DONE (Weekend 3)
    ✓ Chip Huyen AI Engineering — COMPLETE (Week 4)
    ✓ RAG short courses — COMPLETE (Weekend 4)
    ✓ VLM papers (ViT, CLIP, LLaVA) — DONE ★
    ✓ VLM short courses — DONE ★
    ✓ VLM book — STARTED (Weekend 4 Sunday) ★
    ✓ Project 1 — v1 COMPLETE (Weekend 4)

  NOT YET DONE (continues Weeks 5-6):
    → VLM book — finish
    → Document AI study (LayoutLM, Donut, PaddleOCR)
    → Additional VLM papers
    → Labonne deep-dive references

  PRODUCTION CODE:
    ✓ 5+ mini-projects extracted and rebuilt
    ✓ Multiple real contributions submitted
    ✓ Comfortable reading and modifying production code
    ✓ Understand team's architecture and patterns

  RUNNING TOTAL: ~352 hrs (88 × 4 weeks)

  ★ CORE ONBOARDING COMPLETE IN 4 WEEKS.
  ★ VLM specialisation continues in Weeks 5-6.
  ★ You can start contributing to office projects now.
```

---

## WEEKS 5-6: Onboarding Overflow + VLM Specialisation

```
Weeks 5-6 are transitional: you're starting to contribute at the
office while finishing your foundation study at home.

Personal study time: ~46 hrs/week
  Mornings: 2 × 5 = 10 hrs
  Evenings: 2 × 5 = 10 hrs
  Weekends: 26 hrs

  Week 5: VLM book finish + Document AI (LayoutLM, Donut,
           PaddleOCR) + additional VLM papers ............ ~46 hrs
  Week 6: Project 2 start (Multimodal RAG) M1-M2 +
           remaining Labonne references .................. ~46 hrs
```

---

## WEEKS 7-14: Specialisation Track (Personal Time)

```
Personal study time: ~46 hrs/week

At 46 hrs/week:
  Weeks 7-8:   Project 2 finish (M3-M5) ................ ~40 hrs
  Weeks 9-11:  Project 3 (VLM Fine-Tuning) ............. ~45 hrs
  Weeks 12-13: Phase 4E-4G study (distributed training,
               inference opt, RLHF/DPO) ................ ~35 hrs
  Week 14:     Project 4 (Serving Infrastructure) ....... ~25 hrs

  ★ PORTFOLIO-READY BY WEEK 14

  Open Source contributions: ongoing from Week 7+
```

---

## WEEKS 15-28: Full AI Stack (Personal Time)

```
Same 46 hrs/week personal time.

  Weeks 15-17: Ng DL Spec Courses 1-3 + Reza Ch 7-8 .... ~60 hrs
  Weeks 18-19: Ng DL Spec Courses 4-5 + Reza Ch 10-14 .. ~55 hrs
  Weeks 20-21: Prob/Stats + Data Analysis ............... ~34 hrs
  Weeks 22-23: Classical ML (Ng ML Spec C1 + Géron) ..... ~37 hrs
  Weeks 24-28: MLOps + Production (DMLS + DLAI + Reddi) . ~73 hrs
  SQL + remaining: fits into gaps ...................... ~20 hrs

  ★ FULL STACK COMPLETE BY WEEK 28 (~7 months total)
```

---

## COMPLETE TIMELINE

```
  Core onboarding (Phases 1-3A):    Week 4
  VLM specialisation complete:      Week 6
  4 portfolio projects done:        Week 14
  Full AI stack complete:           Week 28 (~7 months)

  Weekly hours: 88 (10 morning + 42.5 office + 10 evening + 26 weekend)
  Foundation study: 46 hrs/week
  Production code:  42.5 hrs/week

  WHY THIS WORKS:
  1. 26-hr weekends carry the bulk of foundation study
  2. Production code from Day 1 (dual-exposure with evening study)
  3. Realistic reading estimates (active reading, not skimming)
  4. Weekday mornings and evenings are supplementary, not primary
```
