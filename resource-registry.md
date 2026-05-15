# Complete Roadmap v5.0 — FILE 3 of 3: RESOURCE REGISTRY

```
COMPANION TO:    FILE 1 (Curriculum), FILE 2 (Weekly Execution Plan)
LAST UPDATED:    April 4, 2026

Every resource in this roadmap has been vetted. This file contains:
  - All primary resources with ratings and vetting status
  - All reference resources
  - All free resources
  - All papers
  - Consolidated reading plans for multi-phase books
  - What was removed and why
```

---

## O'Reilly Platform Books

```
#   TITLE                                    AUTHOR              YEAR  RATING          PHASE   STATUS
──  ─────────────────────────────────────    ──────────────────  ────  ──────────────  ──────  ──────────────
1   Robust Python                            Viafore             2021  GR 4.31/5       1A      ✅ Vetted
2   Fluent Python (2nd Ed)                   Ramalho             2022  GR 4.62/5       1A      ✅ Vetted
3   Python Testing with pytest (2nd Ed)      Okken               2022  GR 4.35/5       1C      ✅ Vetted
4   Clean Code                               Martin              2008  GR 4.37/5       1C      ✅ Vetted
5   Grokking Algorithms                      Bhargava            2016  GR 4.41/5       1D      ✅ Vetted
6   Learn Generative AI with PyTorch         Liu                 2024  Manning pos.    2B      ✅ Vetted
7   Hands-On Large Language Models           Alammar/Grootendorst 2024 AM 4.7 GR 4.33 2C      ✅ Vetted
8   Deep Learning for Vision Systems         Elgendy             2020  AM 4.5 GR 4.28 2D      ✅ REPLACEMENT
9   AI Engineering                           Chip Huyen          2025  AM 4.7 GR 4.43 3A      ✅ Vetted
10  Vision Language Models                   (O'Reilly early)    2025  No reviews yet  3D      ⚠️ Provisional
11  NLP with Transformers                    Tunstall et al.     2022  GR 4.39/5       Ref     ✅ Vetted
12  Hands-On Machine Learning (3rd Ed)       Géron               2022  GR 4.57/5       4C Ref  ✅ Vetted
13  Designing ML Systems                     Chip Huyen          2022  AM 4.6 GR 4.26 4F      ✅ Vetted
14  Python for Data Analysis (3rd Ed)        McKinney            2022  GR 4.15/5       4A      ✅ Vetted
15  Learning SQL (3rd Ed)                    Beaulieu            2020  GR 3.95/5       4B      ✅ Vetted
16  ML and AI: Concepts, Algorithms, Models  Rawassizadeh        2024  Limited reviews 4A/4D   ✅ Kept (request)
17  ML System Design Interview               Aminian/Xu          2022  GR 4.15/5       4H Opt  ✅ Vetted
18  AI Agents with MCP                       Stratis             2025  Limited reviews 3C Ref  ⚠️ New

REMOVED:
──  ─────────────────────────────────────    ──────────────────  ────  ──────────────  ──────  ──────────────
X   Modern CV with PyTorch (2nd Ed)          Ayyadevara/Reddy    2024  OR 2.0/5        2D      ❌ REMOVED
    Reason: All 3 O'Reilly reviews flagged broken code, possibly
    AI-generated, and poor explanations. Replaced with Elgendy (#8)
    + CS231n assignments.
```

---

## DeepLearning.AI Courses

```
#   TITLE                                    TYPE     HOURS  PHASE   STATUS
──  ─────────────────────────────────────    ──────   ─────  ──────  ──────
1   Math for ML & DS — Course 1 (LA)         Spec     ~15    1B      ✅
2   Math for ML & DS — Course 2 (Calc)       Spec     ~15    1B      ✅
3   Math for ML & DS — Course 3 (Prob/Stats) Spec     ~15    4A      ✅
4   ML Specialization — Course 1 only        Spec     ~30    4C      ✅
5   Deep Learning Specialization (5 courses) Spec     ~80    4D      ✅
6   MLOps Specialization (4 courses)         Spec     ~40    4F      ✅
7   How Diffusion Models Work                Short    ~1.5   2D ★    ✅
8   Prompt Vision Models                     Short    ~1.5   3D ★    ✅
9   Building Multimodal Search and RAG       Short    ~1.5   3D ★    ✅
10  Preprocessing Unstructured Data for LLMs Short    ~1.5   3E      ✅
11  Building Applications with Vector DBs    Short    ~1.5   3E      ✅
12  RLHF                                     Short    ~1.5   4G ★    ✅
13  Building and Evaluating Advanced RAG     Short    ~1.5   3B      ✅
14  Generative AI with LLMs                  Course   ~16    3A Ref  ✅

★ = Sarvam-specific addition
```

---

## Free Resources

```
#   RESOURCE                                  TYPE         PHASE      STATUS
──  ─────────────────────────────────────     ──────────   ─────────  ──────────────
1   Karpathy: Neural Networks Zero to Hero    YouTube      2A         ✅ Irreplaceable
2   3Blue1Brown: Essence of Linear Algebra    YouTube      1B         ✅
3   3Blue1Brown: Essence of Calculus          YouTube      1B         ✅
4   3Blue1Brown: Visual intro to Transformers YouTube      3A Ref     ✅
5   Jay Alammar blog (jalammar.github.io)     Blog         2C/2D      ✅
6   Lilian Weng blog (lilianweng.github.io)   Blog         3D Ref ★   ✅
7   LLM Visualization (bbycroft.net/llm)      Interactive  3A Ref     ✅
8   Labonne LLM Course (GitHub)               Link index   3 Ref      ✅
9   Chip Huyen agents blog post               Blog         3C Ref     ✅
10  OpenCV-Python tutorials (docs.opencv.org) Docs         2D         ✅
11  Stanford CS231n notes + assignments       Academic     2D         ✅
12  Hugging Face docs (huggingface.co/docs)   Docs         Throughout ✅
13  StatQuest (Josh Starmer, YouTube)         YouTube      4A Ref     ✅
14  Khan Academy — LA and Calculus            Course       1B Ref     ✅
15  MML book (mml-book.github.io)             Free PDF     1B Ref     ✅
16  ML Systems by Reddi (mlsysbook.ai)        Free textbook 4E/4F     ✅
17  nanoGPT (GitHub karpathy/nanoGPT)         Code         2A         ✅
18  vLLM documentation                        Docs         4E ★       ✅
19  DeepSpeed documentation                   Docs         4E ★       ✅
20  HF TRL documentation                      Docs         4G ★       ✅
21  HF Accelerate documentation               Docs         4E ★       ✅
22  Patrick Loeber PyTorch Tutorials          YouTube      2A Ref     ✅
23  fast.ai: Practical Deep Learning          Course       General    ✅
24  Sentence Transformers (sbert.net)         Docs         3B Ref     ✅
25  Papers With Code — VLM section            Index        3D Ref ★   ✅
26  Labonne blog — fine-tuning articles       Blog         3A Ref     ✅
27  Sebastian Raschka — LoRA insights         Blog         3A Ref     ✅
28  Hamel Husain — Mastering LLMs             Video        3A Ref     ✅
29  LLM Evaluation Guidebook by HF           Docs         3A Ref     ✅
30  Chatbot Arena (lmarena.ai)                Interactive  3A Ref     ✅
```

---

## Papers

```
#   PAPER                                       AUTHORS           YEAR  PHASE
──  ──────────────────────────────────────────  ────────────────  ────  ─────
1   An Image is Worth 16x16 Words (ViT)         Dosovitskiy+      2021  2D ★
2   Learning Transferable Visual Models (CLIP)   Radford+          2021  3D ★
3   Visual Instruction Tuning (LLaVA)            Liu+              2023  3D ★
4   LLaVA-1.5 / LLaVA-NeXT                      Liu+              2023+ 3D ★
5   Qwen-VL or InternVL (pick one)               Various           2024  3D ★
6   Direct Preference Optimization (DPO)         Rafailov+         2023  4G ★
7   ZeRO: Memory Optimizations                   Rajbhandari+      2020  4E ★
8   FlashAttention                               Dao+              2022  4E ★
9   LayoutLMv3                                   Huang+            2022  3E ★
10  Donut                                        Kim+              2022  3E ★

HOW TO READ PAPERS (since you haven't done this before):
  1. Read the ABSTRACT — 1 paragraph, tells you what they did
  2. Read the INTRODUCTION — 2-3 pages, context and motivation
  3. Read the METHOD section — the actual technique, with diagrams
  4. Look at KEY FIGURES — architecture diagrams tell the story
  5. Read EXPERIMENTS/RESULTS — tables showing performance
  6. SKIP: Related Work, Proofs, Appendices
  Target: 1-2 hours per paper, not 4-6.
```

---

## Reza Rawassizadeh — Consolidated Reading Plan

```
Since Reza's book is used across Phases 4A, 4C, and 4D, here is
the consolidated reading plan in the order you will encounter each:

PHASE 4A (Prob/Stats):
  Ch 3: Statistics & Probability — SELECTIVE
    Focus on: KL-divergence, entropy, MLE, information gain
    Skip: basic distributions you already know
    Time: ~5 hrs

PHASE 4D (Deep Learning Theory):
  Ch 7: Dimensionality Reduction — FULL READ
    PCA, t-SNE, UMAP, SVD, tensor decompositions
    Time: ~5 hrs

  Ch 8: Regression, Regularisation, Optimisation — SELECTIVE
    Gradient descent variants, regularisation (Ridge, LASSO, Elastic Net)
    Time: ~5 hrs

  Ch 10: Neural Networks & DL — SKIM
    You've covered this via Karpathy + Mark Liu. Use Reza only
    when a concept from Ng doesn't click.
    Time: ~3 hrs

  Ch 11: Self-Supervised Neural Networks — SELECTIVE
    Autoencoders, GANs, contrastive learning (SimCLR, Siamese),
    text-to-image models (DALL-E, Stable Diffusion, CLIP)
    Time: ~3 hrs

  Ch 12: Deep Learning Models & Applications — REFERENCE
    Attention mechanisms, transformer architecture, Mamba/S4,
    BERT variants, GPT lineage, LLaMA, Mistral, fine-tuning,
    CV architectures, object detection, audio models.
    Use as encyclopedia — read relevant sections only.
    Time: ~2 hrs

  Ch 14: Making Lighter Neural Networks — SELECTIVE ★ PRIORITY
    Quantisation (PTQ, QAT), pruning, knowledge distillation,
    LoRA, FlashAttention, Neural Architecture Search.
    ★ Directly relevant to Sarvam bonus points.
    Time: ~5 hrs

TOTAL REZA (selective): ~28 hrs across Phases 4A-4D

SKIPPED from Reza:
  Ch 1: Introduction — you already know this
  Ch 4: Clustering — classical ML, not priority
  Ch 5: Frequent Itemset — classical ML, not priority
  Ch 6: Feature Engineering — learn through project work
  Ch 9: Classification — covered by Ng Course 1
  Ch 13: Reinforcement Learning — not relevant for Sarvam
  Ch 15: Graph Mining — specialised, not relevant
  Ch 16: Challenges of Working with Data — read IF TIME PERMITS
         (imbalanced data, data drift sections are useful)
```

---

## ML Systems by Reddi — Consolidated Reading Plan

```
PHASE 4E/4F:
  Ch 1: Introduction (~3 hrs)
    ML systems lifecycle, deployment spectrum, engineering challenges.
    Read first for the "five-pillar framework."

  Ch 2: ML Systems (~3 hrs)
    Cloud vs. Edge vs. Mobile vs. TinyML deployment paradigms.
    Decision framework for choosing where to deploy.

  Ch 9: Efficient AI (~4 hrs)
    Scaling laws, efficiency framework, trade-off management.
    WHY models cost what they cost and how to make them cheaper.

  Ch 10: Model Optimizations (~5 hrs)
    Pruning, quantisation, knowledge distillation, NAS.
    Systems view — pairs with Reza Ch 14 (algorithmic view).

  Ch 13: ML Operations (~4 hrs)
    MLOps from a systems engineering perspective.

TOTAL ML SYSTEMS (selective): ~19 hrs
Remaining chapters: use as reference when relevant.
```

---

## Complete Hours Summary

```
PHASE 1 (Foundations):          ~130 hrs    Weeks 1-2
PHASE 2 (PyTorch, CV):         ~130 hrs    Weeks 3-4
PHASE 3A-B (LLM Eng, RAG):     ~24 hrs     Week 5-6
PHASE 3D-E (VLMs, Doc AI):     ~37 hrs     Weeks 7-8 (personal)
PROJECT 1:                      ~25 hrs     Weeks 5-6 (personal)
PROJECT 2:                      ~35 hrs     Weeks 9-11 (personal)
PROJECT 3:                      ~45 hrs     Weeks 12-14 (personal)
PHASE 4E-4G (Dist Train, RLHF): ~35 hrs    Weeks 13-14 (personal)
PROJECT 4:                      ~25 hrs     Week 15 (personal)
────────────────────────────────────────────
SUBTOTAL TO SARVAM-READY:       ~486 hrs    ~15 weeks

PHASE 4A (Prob/Stats):          ~30 hrs     Weeks 16-17
PHASE 4B (SQL):                 ~8 hrs      Week 17
PHASE 4C (Classical ML):        ~35 hrs     Weeks 18-19
PHASE 4D (DL Theory):          ~60 hrs     Weeks 20-23
PHASE 4F (MLOps):              ~69 hrs     Weeks 24-27
PHASE 4H (System Design):      ~12 hrs     Week 28 (optional)
────────────────────────────────────────────
SUBTOTAL FULL STACK:            ~700 hrs    ~28-30 weeks

PROJECT 5 (Open Source):        ~20+ hrs    Ongoing from Week 8
────────────────────────────────────────────
GRAND TOTAL:                    ~720 hrs    ~7-8 months
```
