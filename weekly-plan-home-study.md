# Alternative Plan: Full-Time Home Study (No Job)

```
USE CASE:      You are not working. Full-time study to get job-ready.
APPLIES WITH:  Curriculum file (same resources, same phases)
               Resource Registry (same vetting)
               Learning Prompt — Home Study Variant
NOTE:          No office production code. Top-down exposure comes from
               OPEN-SOURCE CODEBASE READING (see learning prompt for
               the full protocol and which repos to read per phase).
               The afternoon practice block includes codebase reading
               alongside exercises and project work.
```

---

## Daily Schedule

```
  5:00 AM         Wake up, freshen up
  5:30 - 9:30 AM  DEEP STUDY BLOCK 1 (4 hrs) — books, code-along
  [9:30 - 10:00 AM  Breakfast]
  10:00 - 1:00 PM DEEP STUDY BLOCK 2 (3 hrs) — courses, videos, assignments
  [1:00 - 2:00 PM   Lunch + rest]
  2:00 - 5:00 PM  PROJECT / PRACTICE BLOCK (3 hrs) — build things, exercises
  [5:00 - 5:30 PM   Walk]
  5:30 - 7:00 PM  STUDY BLOCK 3 (1.5 hrs) — papers, docs, lighter material
  [7:00 - 8:00 PM   Dinner + rest]
  8:00 - 9:30 PM  EVENING REVIEW (1.5 hrs) — review day's notes, Exercism,
                   plan tomorrow
  [9:30 PM         Wind down, sleep by 10 PM. 7 hrs sleep.]

DAILY TOTAL:     ~13 hrs/day

WEEKENDS:        Same structure but lighter afternoon block.
                 12 hrs/day × 2 = 24 hrs

WEEKLY TOTAL:    13 × 5 + 24 = ~89 hrs/week foundation study
                 (No office hours — all study)
```

---

## Key Difference From Office Plan

```
The office plan has dual-exposure: production code teaches you patterns
from the top, books teach you fundamentals from the bottom.

This plan replaces production code with OPEN-SOURCE CODEBASE READING
as the top-down learning channel. You compensate by:

  1. Reading one open-source codebase per phase using the 5-step
     protocol in the learning prompt (survey → trace → break →
     rebuild a module from scratch → document). This happens in
     the afternoon practice block.
     Phase 1-2: nanoGPT, micrograd (small, clean, Karpathy's code)
     Phase 2:   timm (pick one model like ViT, trace forward pass)
     Phase 3:   LLaVA (VLM training/inference code)
     Phase 4:   vLLM (serving infrastructure)

  2. Spending more time on code-along resources (Karpathy, Mark Liu,
     CS231n assignments) — these double as "production code" exposure

  3. Starting portfolio projects EARLIER (Week 5 instead of Week 6)
     because projects force you to write real code

  4. More Exercism / coding practice (3-4 per day, not 2-3) plus
     reviewing community solutions after each exercise for the code
     review exposure you'd get from colleagues

  5. Rebuilding one open-source module per week from scratch starting
     Week 3 (same as the office plan's mini-project extraction, but
     with public repos instead of proprietary code)

The afternoon block (2:00-5:00 PM) is split between:
  - Exercises and practice scripts (daily)
  - Open-source codebase reading and module rebuilds (2-3 times/week)
  - Portfolio project work (from Week 5 onward)
```

---

## Week-by-Week Plan (Corrected Estimates)

### WEEK 1: Python Foundations

```
BLOCK 1 (mornings, 20 hrs):
  Mon-Wed: Robust Python Ch 1-7 ........................ 10 hrs
  Thu-Fri: Robust Python Ch 8-12 ....................... 8 hrs
  Overflow: Robust Python Ch 13-14 ..................... 2 hrs

BLOCK 2 (mid-morning, 15 hrs):
  Mon-Tue: 3Blue1Brown Essence of LA (full) ............ 3.5 hrs
  Wed:     3Blue1Brown Essence of Calculus (full) ....... 3 hrs
  Thu-Fri: Grokking Algorithms Ch 1-8 .................. 5 hrs
  Remaining: Grokking Ch 9-11 .......................... 3.5 hrs

BLOCK 3 (afternoon practice, 15 hrs):
  EVERY DAY: Type examples from the morning's reading,
  then close the book and write a 20-40 line practice script.
  Mon-Wed: Practice scripts from Robust Python chapters  6 hrs
  Mon-Wed: 3-4 Exercism exercises per day .............. 4 hrs
  Thu:     CODEBASE READING — clone nanoGPT, survey the
           repo structure, read README, run it ......... 3 hrs
  Fri:     CODEBASE READING — trace nanoGPT model.py
           line by line, annotate every function ....... 2 hrs

BLOCK 4 (evening, 7.5 hrs):
  Read Clean Code Ch 1-6 ............................... 4 hrs
  Start pytest Ch 1-2 .................................. 3.5 hrs

EVENING REVIEW (7.5 hrs):
  Review notes, plan next day, Exercism overflow ....... 7.5 hrs

WEEK 1 TOTAL: ~65 hrs

COMPLETED:
  ✓ Robust Python Ch 1-14 (~25 hrs)
  ✓ 3Blue1Brown LA + Calculus (~6.5 hrs)
  ✓ Grokking Algorithms (~10 hrs)
  ✓ Clean Code Ch 1-6 (~4 hrs)
  ✓ pytest started (~3.5 hrs)
  ✓ ~15 Exercism exercises
  ✓ ~10 practice scripts
```

### WEEK 2: Python Depth + Math + Testing

```
BLOCK 1 (mornings, 20 hrs):
  Mon:     Robust Python Ch 15-16, 20 (finish) ......... 4 hrs
  Tue-Fri: Fluent Python Parts I-III ................... 16 hrs

BLOCK 2 (mid-morning, 15 hrs):
  Mon-Fri: DLAI Math Spec — Course 1 (full) ............ 15 hrs

BLOCK 3 (afternoon practice, 15 hrs):
  Mon-Wed: pytest Ch 3-7 (type examples, write tests) .. 7 hrs
  Thu-Fri: Practice scripts from Fluent Python ......... 5 hrs
  Daily:   Exercism exercises .......................... 3 hrs

BLOCK 4 (evening, 7.5 hrs):
  Fluent Python Parts IV-V ............................. 7.5 hrs

EVENING REVIEW (7.5 hrs):
  Clean Code Ch 7-10 (finish) ......................... 3 hrs
  Review, plan, Exercism ............................... 4.5 hrs

WEEK 2 TOTAL: ~65 hrs

COMPLETED:
  ✓ Robust Python — COMPLETE (~27 hrs total)
  ✓ Fluent Python — COMPLETE (~30 hrs total)
  ✓ pytest — COMPLETE (~10 hrs total)
  ✓ Clean Code — COMPLETE (~7 hrs total)
  ✓ Grokking Algorithms — COMPLETE (Week 1)
  ✓ 3Blue1Brown — COMPLETE (Week 1)
  ✓ DLAI Math Course 1 — COMPLETE (~15 hrs)

  ★ PHASE 1 ~80% COMPLETE by end of Week 2
```

### WEEK 3: Math Finish + PyTorch + Neural Nets

```
BLOCK 1 (mornings, 20 hrs):
  Mon-Tue: DLAI Math Course 2 .......................... 8 hrs
           (rest of Course 2 in Block 2)
  Wed-Fri: Karpathy Zero to Hero — micrograd through
           makemore 3 (code along) ..................... 12 hrs

BLOCK 2 (mid-morning, 15 hrs):
  Mon-Tue: DLAI Math Course 2 (finish) ................. 7 hrs
  Wed-Fri: Karpathy — makemore 4 + building GPT ........ 8 hrs

BLOCK 3 (afternoon practice, 15 hrs):
  Mon-Tue: Math practice — NumPy implementations of
           LA operations, gradient descent from scratch . 4 hrs
  Wed:     CODEBASE READING — experiment with nanoGPT:
           change hyperparams, break error handlers,
           try alternative approaches .................. 3 hrs
  Thu-Fri: Reimplement Karpathy exercises from memory .. 5 hrs
  Daily:   Exercism → shift to PyTorch exercises ....... 3 hrs

  WEEKEND: REBUILD — pick nanoGPT's training loop or
  micrograd's Value class. Write down the interface.
  Build your version from scratch. Compare.

BLOCK 4 (evening, 7.5 hrs):
  Karpathy — tokenization + nanoGPT source reading ..... 5 hrs
  Jay Alammar blog (Illustrated Transformer, GPT-2) .... 2.5 hrs

EVENING REVIEW (7.5 hrs):
  Review Karpathy code, annotate, plan next day ........ 7.5 hrs

WEEK 3 TOTAL: ~65 hrs

COMPLETED:
  ✓ DLAI Math Courses 1-2 — COMPLETE (~30 hrs total)
  ✓ Karpathy Zero to Hero — COMPLETE (~18 hrs with practice)
  ✓ nanoGPT source reading — COMPLETE
  ✓ Jay Alammar blog posts — COMPLETE

  ★ PHASE 1 COMPLETE. PHASE 2A COMPLETE.
```

### WEEK 4: Generative Models + Pretrained Models + CV Start

```
BLOCK 1 (mornings, 20 hrs):
  Mon-Thu: Mark Liu "Learn GenAI with PyTorch" Parts 1-4
           (code along every chapter) .................. 20 hrs

BLOCK 2 (mid-morning, 15 hrs):
  Mon-Wed: Hands-On LLMs (Alammar book) full .......... 12 hrs
  Thu-Fri: Elgendy "DL for Vision Systems" Ch 5-7 ..... 3 hrs

BLOCK 3 (afternoon practice, 15 hrs):
  Mon-Wed: Experiment with Mark Liu projects — modify
           architectures, observe results ............... 6 hrs
  Wed:     CODEBASE READING — clone timm, pick ViT model,
           trace from model def → forward pass → output  3 hrs
  Thu-Fri: Elgendy Ch 8-10 + OpenCV tutorials start .... 6 hrs

BLOCK 4 (evening, 7.5 hrs):
  ViT paper — method section ........................... 2 hrs
  DLAI "How Diffusion Models Work" ..................... 1.5 hrs
  Alammar "Illustrated Stable Diffusion" ............... 1 hr
  CS231n Assignment 1 start ............................ 3 hrs

EVENING REVIEW (7.5 hrs):
  Review, plan, light reading .......................... 7.5 hrs

WEEK 4 TOTAL: ~65 hrs

COMPLETED:
  ✓ Mark Liu GenAI with PyTorch — COMPLETE
  ✓ Hands-On LLMs — COMPLETE
  ✓ Elgendy DL for Vision Systems — COMPLETE
  ✓ OpenCV — STARTED
  ✓ ViT paper, diffusion short course — DONE

  ★ PHASE 2B + 2C COMPLETE. PHASE 2D ~60% COMPLETE.
```

### WEEK 5: CV Finish + LLM Engineering + Project 1

```
BLOCK 1 (mornings, 20 hrs):
  Mon:     CS231n Assignments 1-2 (finish) ............. 5 hrs
  Mon-Tue: OpenCV tutorials (finish) ................... 3 hrs
  Tue-Fri: Chip Huyen "AI Engineering" full ............ 12 hrs

BLOCK 2 (mid-morning, 15 hrs):
  Mon-Tue: DLAI RAG short courses (2 courses) .......... 3 hrs
  Wed:     CLIP paper — method section ................. 2 hrs
  Wed:     LLaVA paper — method section ................ 2 hrs
  Thu-Fri: DLAI VLM short courses (2 courses) .......... 3 hrs
  Thu-Fri: Labonne references (LoRA, quantization) ..... 5 hrs

BLOCK 3 (afternoon — PROJECT 1, 15 hrs):
  Mon-Fri: Build Project 1 (Document Digitisation)
    Mon: M1 — scope, collect samples, ground truth ..... 3 hrs
    Tue: M2 — OpenCV preprocessing pipeline ............ 3 hrs
    Wed: M3 — OCR comparison layer ..................... 3 hrs
    Thu: M4 — VLM extraction + evaluation .............. 3 hrs
    Fri: M5 — FastAPI + tests + README + push .......... 3 hrs

BLOCK 4 (evening, 7.5 hrs):
  DLAI "Prompt Vision Models" .......................... 1.5 hrs
  DLAI "Building Multimodal Search and RAG" ............ 1.5 hrs
  DLAI "Preprocessing Unstructured Data" ............... 1.5 hrs
  DLAI "Building Apps with Vector DBs" ................. 1.5 hrs
  Review + plan Week 6 ................................ 1.5 hrs

WEEK 5 TOTAL: ~65 hrs (+ 7.5 review)

COMPLETED:
  ✓ CS231n Assignments — COMPLETE
  ✓ OpenCV — COMPLETE
  ✓ Chip Huyen AI Engineering — COMPLETE
  ✓ RAG short courses — COMPLETE
  ✓ VLM papers (CLIP, LLaVA) — DONE
  ✓ VLM short courses — DONE
  ✓ Project 1 v1 — COMPLETE

  ★ PHASES 1-3B COMPLETE. PROJECT 1 DONE.
```

### WEEK 6: VLMs + Document AI + Project 2 Start

```
  VLM book (O'Reilly) or HF VLM tutorials ............. 20 hrs
  Document AI study (LayoutLM, Donut, PaddleOCR) ....... 10 hrs
  Additional VLM papers (LLaVA-NeXT, Qwen-VL) ......... 5 hrs
  CODEBASE READING — clone LLaVA repo, trace training
    and inference code (connects to VLM papers) ........ 5 hrs
  Project 2 (Multimodal RAG) — M1-M2 .................. 14 hrs
  Practice + review .................................... 11 hrs

  ★ PHASE 3D-3E COMPLETE. PROJECT 2 ~40% DONE.
```

### WEEKS 7-8: Projects 2-3

```
  Week 7: Project 2 finish (M3-M5) + Project 3 start (M1)  ~65 hrs
  Week 8: Project 3 (M2-M4) ...............................  ~65 hrs
```

### WEEKS 9-10: Distributed Training + Project 3-4 Finish

```
  Week 9:  Project 3 finish (M5) + Phase 4E-4G study
           + CODEBASE READING: vLLM (trace scheduler,
             PagedAttention, one request flow) .............  ~65 hrs
  Week 10: Project 4 (Serving Infrastructure) + OSS start ..  ~65 hrs

  ★ COMPETITIVE FOR VISION ML ENGINEER ROLES BY WEEK 10
```

### WEEKS 11-20: Full AI Stack (Phase 4)

```
  Weeks 11-13: Ng DL Spec (5 courses) + Reza selective ..... ~195 hrs
  Weeks 14-15: Prob/Stats + Data Analysis .................. ~130 hrs
  Weeks 16-17: Classical ML (compressed) ................... ~130 hrs
  Weeks 18-20: MLOps + Production + SQL .................... ~195 hrs

  ★ FULL AI STACK COMPLETE BY WEEK 20 (~5 months)
```

---

## Timeline Comparison

```
                      Office Plan       Home Study Plan
                      (v5.1 corrected)  (this file)
─────────────────────────────────────────────────────────
Study hrs/week:       46 (personal)     65-89 (all day)
Office hrs/week:      42.5              0
Total hrs/week:       88.5              65-89
Phase 1 complete:     Week 2            Week 2
Phase 2 complete:     Week 4            Week 4
Phase 3 complete:     Week 6            Week 5
Project-ready:        Week 6            Week 5
4 projects done:      Week 14           Week 10
Full AI stack:        Week 28-30        Week 20
─────────────────────────────────────────────────────────

The home plan is faster for pure study (no commute, no office overhead)
but LACKS production code exposure. You compensate with open-source
codebase reading (see learning prompt for the full protocol), more
code-along resources, and earlier project starts.
```
