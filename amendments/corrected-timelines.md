# Weekly Plan Amendment v2 — Corrected Timelines + No-Gym Mornings

```
APPLIES TO:    v5-1-RESTRUCTURED-WEEKLY-PLAN.md
REPLACES:      AMENDMENT-gym-schedule-option-b.md (archived)
DATE:          May 15, 2026
CHANGES:
  1. Reading time estimates corrected (active reading = 1.5-1.8x original)
  2. Morning study restored (no gym currently, 5:00-7:00 AM available)
  3. Evening walk = 30 min (not 1 hr), study starts 7:30 PM
  4. Phase 1A total corrected from 36 hrs to ~58 hrs
  5. Onboarding extends from 4 weeks to ~6 weeks
```

---

## Corrected Reading Estimates (All of Phase 1)

```
Active reading = reading + typing every example + writing a practice
script after each chapter. Real pace: ~12-15 pages/hour.

ROBUST PYTHON (was 17 hrs → now ~27 hrs):
  Ch 1-4 (Types, Annotations) ........... ~5 hrs  (was 2)
  Ch 5-7 (Enums, Dataclasses, Classes) .. ~5 hrs  (was 3)
  Ch 8-14 (Extensibility, Dependencies) . ~13 hrs (was 8)
  Ch 15-16, 20 (selective, rest defer) .. ~4 hrs  (was 4, unchanged)
  TOTAL: ~27 hrs

FLUENT PYTHON (was 19 hrs → now ~30 hrs):
  Part I: Data Structures ............... ~7 hrs  (was 4)
  Part II: Functions as Objects ......... ~5 hrs  (was 3)
  Part III: Classes and Protocols ....... ~7 hrs  (was 5)
  Part IV: Control Flow ................. ~6 hrs  (was 4)
  Part V: Metaprogramming ............... ~5 hrs  (was 3)
  TOTAL: ~30 hrs

GROKKING ALGORITHMS (was 8 hrs → now ~10 hrs):
  Implement each algorithm after reading adds ~2 hrs.

PYTEST (was 8 hrs → now ~10 hrs):
  Typing examples + writing test files adds ~2 hrs.

CLEAN CODE (stays ~7 hrs — reading-only, Java examples):
  No code-along needed. Read for principles.

3BLUE1BROWN (stays ~6.5 hrs — video, not reading):
  Watch time is fixed.

DLAI MATH COURSES 1-2 (stays ~30 hrs — course pacing is fixed):
  Video + exercises. Time is set by the platform.

PHASE 1 TOTAL: was ~95 hrs → now ~120 hrs
  Additional ~25 hrs needed.
```

---

## The Same Pattern Applies to All Later Phases

```
Apply 1.5x multiplier to any book-based reading estimate in the
curriculum. Course/video estimates are accurate as-is. Paper reading
estimates are accurate as-is (you're reading method sections, not
coding along).

PHASE 2 book reading affected:
  Mark Liu:     was 20 hrs → ~28 hrs (code-along book, every chapter builds)
  Hands-On LLMs: was 14 hrs → ~18 hrs (some coding, mostly conceptual)
  Elgendy:      was 14 hrs → ~18 hrs (selective reading + practice)
  CS231n:       was 8 hrs → ~10 hrs (assignments are already hands-on)

PHASE 3 book reading affected:
  Chip Huyen:   was 16 hrs → ~20 hrs (dense, lots of note-taking)
  VLM book:     was 16 hrs → ~20 hrs (estimate, early release)

NOT affected (videos, courses, papers, docs):
  Karpathy (15 hrs) — video, code-along time is fixed
  3Blue1Brown — video
  DLAI short courses — video
  Papers — reading, not coding
  OpenCV tutorials — docs, just-in-time
```

---

## Revised Daily Schedule (No Gym, With Walk)

```
WEEKDAYS:
  5:00 - 7:00 AM ... MORNING STUDY (2 hrs) — deep reading, books
  [7:00 - 8:00 AM .. Breakfast + get ready]
  [8:00 - 9:30 AM .. Commute]
  9:30 - 6:00 PM ... OFFICE — production code (8.5 hrs)
  [6:00 - 6:30 PM .. Commute]
  6:30 - 7:00 PM ... Walk (30 min)
  7:00 - 7:30 PM ... Freshen up + dinner (30 min)
  7:30 - 9:30 PM ... EVENING STUDY (2 hrs) — lighter material + practice
  [9:30 - 10:00 PM . Wind down, sleep]

WEEKENDS:
  26 hrs total (unchanged from v5.1 Revised)
  13 hrs Saturday, 13 hrs Sunday

WEEKLY TOTALS:
  Mornings:   2 × 5 = 10 hrs
  Office:     8.5 × 5 = 42.5 hrs
  Evenings:   2 × 5 = 10 hrs
  Weekends:   26 hrs
  TOTAL:      88.5 hrs/week (same as v5.1 Revised)
  Foundation study: 46 hrs/week
```

---

## How to Read the Weekly Plan With This Amendment

```
The v5.1 weekly plan's STRUCTURE is still correct:
  - Morning blocks: keep as-is (5:00-7:00 AM, 2 hrs)
  - Office blocks: keep as-is (production code)
  - Evening blocks: keep as-is (7:30-9:30 PM, 2 hrs)
  - Weekend blocks: keep as-is (26 hrs)

What changes: TIME ESTIMATES for reading-heavy days.

When the plan says "Robust Python Ch 1-4 — 2 hrs" in a morning slot,
you now know it's actually ~5 hrs. That means Ch 1-4 spills across
2-3 morning sessions, not one.

PRACTICAL ADJUSTMENT — just shift the content rightward:
  Week 1 morning plan says:
    Mon: Robust Python Ch 1-4        → Actually takes Mon + Tue mornings
    Tue: Robust Python Ch 5-7        → Actually takes Wed + Thu mornings
    Wed: Robust Python Ch 8-11       → Spills to Fri + Weekend
    Thu: Robust Python Ch 12-15+     → Spills to Weekend
    Fri: Grokking Ch 1-4             → Moves to Weekend

  The weekend absorbs the overflow. That's what the 26-hr weekends
  are for. If Robust Python takes the full first week of mornings
  instead of 2.5 days, the weekend picks up Grokking and starts
  Fluent Python.
```

---

## Revised Onboarding Timeline

```
With corrected estimates, Phase 1 alone needs ~120 hrs (not 95).
Phase 2 needs ~115 hrs (not 100). Phase 3A-B needs ~25 hrs (same).

Total to onboarding-complete: ~260 hrs of foundation study
  + 42.5 hrs/week office production code (separate track)

At 46 hrs/week of foundation study: 260 ÷ 46 = ~5.6 weeks

REVISED TIMELINE:
                          v5.1 Revised    With corrected estimates
  Onboarding:            Week 4           Week 6
  Target Company-ready:          Week 11          Week 14
  Full AI stack:         Week 24          Week 28-30

This is actually FINE. The original v4 plan estimated 6 weeks for
onboarding. The corrected estimates bring us back to that number.
The v5.1 plan was optimistic. Reality is: 6 weeks for onboarding
with proper active reading is honest and achievable.
```

---

## No Other Files Need to Change

```
v5-FILE1-CURRICULUM.md             ← UNCHANGED (apply 1.5x mentally to book hrs)
v5-FILE3-RESOURCE-REGISTRY.md      ← UNCHANGED
v5-1-RESTRUCTURED-WEEKLY-PLAN.md   ← READ WITH THIS AMENDMENT
learning-prompt-v3-1.md            ← UNCHANGED
.cursor/rules/*                    ← UNCHANGED
```
