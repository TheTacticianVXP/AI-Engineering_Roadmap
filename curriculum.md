# Complete Roadmap v5.0 — FILE 1 of 3: CURRICULUM
## Phase-by-Phase Learning Plan

```
TARGET:          ML/AI Engineer with Vision/Multimodal specialisation
PURPOSE:         Complete AI/ML engineering curriculum from scratch
LAST UPDATED:    May 15, 2026
SUPERSEDES:      All previous versions (v3, v4, v5.0)
COMPANION FILES: Weekly Plan (office or home-study variant),
                 Resource Registry (FILE 3)

NOTE ON TIME ESTIMATES:
  All book reading times assume ACTIVE READING: reading + typing every
  code example + writing a 20-40 line practice script after each chapter.
  Real pace for active reading: ~12-15 pages/hour.
  Video/course times are accurate as-is (platform-paced).
  Paper reading times are accurate as-is (method sections only).
```

---

## Time Estimates

```
TWO STUDY MODES (see the Weekly Plan files for schedules):

  FULL-TIME HOME STUDY (no job):
    ~65 hrs/week of foundation study
    Portfolio-ready by Week 10, full stack by Week 20 (~5 months)

  ALONGSIDE A JOB (office onboarding):
    ~46 hrs/week of foundation study + 42.5 hrs/week production code
    Portfolio-ready by Week 14, full stack by Week 28 (~7 months)

  Choose the Weekly Plan file that matches your situation.
  This curriculum file covers WHAT to study. The weekly plans cover WHEN.
```

---

## PHASE 1: Foundations

```
CURRICULUM AREA: Python mastery, math for AI, testing, DSA
  Weeks: 1-3 (home study) or 1-4 (alongside job)
  Total hours: ~120 hrs
  Status: [not started]
```

### 1A: Python Mastery

```
CURRICULUM AREA: Python — beyond basics
  Phase: 1A
  Status: [not started]

  PRIMARY:
    1. "Robust Python" by Patrick Viafore — O'Reilly, 2021
       - Goodreads: 4.31/5 (97 ratings). Well-reviewed, unique niche.
       - Chapters 1-4 (types and annotations): ~5 hours
       - Chapters 5-7 (enums, dataclasses, classes): ~5 hours
       - Chapters 8-14 (extensibility, dependencies): ~13 hours
       - Chapters 15-16, 20 (selective — defer ch 17-19, 21-24): ~4 hours
       - Total: ~27 hours
       - Status: [not started]
       - HOW TO USE: Read actively. After each chapter, write a small
         script (20-50 lines) that uses the concepts. Type hints are
         not optional — every Python file you write from now on uses them.

    2. "Fluent Python" by Luciano Ramalho (2nd Edition) — O'Reilly, 2022
       - Goodreads: 4.62/5 (2,800+ ratings). Best intermediate Python book.
       - Part I: Data structures (~7 hours)
       - Part II: Functions as objects (~5 hours)
       - Part III: Classes and protocols (~7 hours)
       - Part IV: Control flow (~6 hours)
         ★ Pay extra attention to generators, iterators, __iter__,
           __next__, and generator pipelines. These patterns appear
           constantly in data pipeline code.
       - Part V: Metaprogramming (~5 hours)
       - Total: ~30 hours
       - Status: [not started]
       - Note: Start this AFTER Robust Python chapters 1-7

  Prerequisites: Basic Python syntax (you have this)
  Unlocks: Everything. Every resource after this assumes solid Python.
```

### 1B: Math for AI

```
CURRICULUM AREA: Math foundations for AI/ML
  Phase: 1B
  Status: [not started]

  PRIMARY:
    1. "Essence of Linear Algebra" by 3Blue1Brown — YouTube (free)
       - Full playlist: 16 videos (~3.5 hours)
       - Status: [not started]
       - Watch FIRST. Tensors, matrix ops, eigenvalues — this is the
         language of PyTorch and attention mechanisms.
       - HOW TO USE: Watch at 1x speed. Pause when he introduces a
         new concept. Sketch the transformations on paper. The visual
         intuition you build here pays off for months.

    2. "Essence of Calculus" by 3Blue1Brown — YouTube (free)
       - Full playlist: 12 videos (~3 hours)
       - Status: [not started]
       - Chain rule IS backpropagation. This is not abstract —
         you will use this directly when Karpathy builds micrograd.

    3. "Mathematics for Machine Learning and Data Science" — DeepLearning.AI
       - Course 1: Linear Algebra (~15 hours) — do NOW
       - Course 2: Calculus (~15 hours) — do NOW
       - Course 3: Probability & Statistics — DEFER to Phase 4A
       - Phase 1 total: ~30 hours
       - Status: [not started]
       - HOW TO USE: Watch lectures, do ALL exercises. The quizzes
         and programming assignments are where the learning happens.
         3Blue1Brown gives you visual intuition; this course gives
         you the ability to compute and apply.

  REFERENCE (use if a concept isn't clicking, not required to read):
    - "Mathematics for Machine Learning" by Deisenroth, Faisal, Ong
      — free PDF at mml-book.github.io (also on O'Reilly).
      Use chapters 2-4 (LA) and 5 (vector calculus) as backup.
    - Khan Academy — Linear Algebra and Calculus sections (free).
      Use for extra practice on specific topics that need drilling.

  Prerequisites: High school math, college ML/DL theory
  Unlocks: Understanding tensor ops, loss functions, attention math
```

### 1C: Testing & Software Engineering

```
CURRICULUM AREA: Testing and engineering practices
  Phase: 1C
  Status: [beginner — learned assert/pytest basics]

  PRIMARY:
    1. "Python Testing with pytest" by Brian Okken (2nd Ed) — O'Reilly, 2022
       - Goodreads: 4.35/5 (230+ ratings). The definitive pytest book.
       - Chapters 1-2: Getting started (~45 min)
       - Chapters 3-4: Fixtures, parametrize (~2 hours)
       - Chapters 5-6: Markers, mocking (~2 hours)
       - Chapters 7+: Plugins, CI (~3 hours)
       - Total: ~10 hours
       - Status: [not started]

    2. "Clean Code" by Robert C. Martin — O'Reilly
       - Goodreads: 4.37/5 (12,000+ ratings). Classic.
       - Chapters 1-6: Core practices (~4 hours)
       - Chapters 7-10: Error handling, boundaries, tests (~3 hours)
       - Total: ~7 hours
       - Status: [not started]
       - Note: Examples are in Java but principles are universal.

  Prerequisites: Basic Python
  Unlocks: Writing production-quality code, CI/CD pipelines
```

### 1D: Data Structures & Algorithms

```
CURRICULUM AREA: DSA fundamentals
  Phase: 1D
  Status: [beginner]

  PRIMARY:
    1. "Grokking Algorithms" by Aditya Bhargava — O'Reilly
       - Goodreads: 4.41/5 (7,900+ ratings). Beautifully illustrated.
       - Full book: ~10 hours
       - Status: [not started]
       - HOW TO USE: Read the illustrations carefully — they ARE the
         explanation. Implement each algorithm in Python after reading.

  Prerequisites: Basic Python
  Unlocks: Efficient code, understanding algorithm complexity
```

---

## PHASE 2: PyTorch, Vision & Understanding Models

```
CURRICULUM AREA: Deep learning implementation, generative models, CV
  Weeks: 3-5 (home study) or 4-7 (alongside job)
  Total hours: ~135 hrs
  Status: [not started]
```

### 2A: Neural Networks from Scratch + PyTorch

```
CURRICULUM AREA: Deep learning fundamentals with PyTorch
  Phase: 2A
  Status: [not started]

  PRIMARY:
    1. "Neural Networks: Zero to Hero" by Andrej Karpathy — YouTube (free)
       - Full playlist: ~18 hours (including code-along and re-runs)
       - Link: karpathy.ai/zero-to-hero.html
       - Status: [not started]
       - HOW TO USE: Code along with EVERY video. Type everything.
         Run everything locally in Jupyter notebooks. This is not a
         "watch and absorb" resource. You will build:
           Video 1: micrograd — backprop engine from scratch
           Videos 2-5: makemore — MLPs, BatchNorm, activations, WaveNet
           Video 6: building GPT from scratch
           Video 7: tokenization
       - After "Let's Build GPT" (video 6), spend 2-3 hours reading
         the nanoGPT source code on GitHub (karpathy/nanoGPT). Navigate
         model.py, train.py, understand config objects and checkpoint
         loading. This builds the skill of reading and modifying
         model internals — a core requirement for ML engineering roles.

  REFERENCE:
    - Patrick Loeber — PyTorch Tutorials (YouTube, free). Short videos
      for quick PyTorch syntax lookups if Karpathy moves too fast on
      PyTorch-specific APIs.
    - PyTorch official tutorials (pytorch.org/tutorials) — "Learn the
      Basics" 60-min blitz. Use as a quick reference, not a course.

  Prerequisites: Python mastery (Phase 1A), LA/calculus intuition (1B)
  Unlocks: Everything in Phases 2B-2D and Phase 3
```

### 2B: Generative AI with PyTorch (Project-Based)

```
CURRICULUM AREA: Building generative models in PyTorch
  Phase: 2B
  Status: [not started]

  PRIMARY:
    1. "Learn Generative AI with PyTorch" by Mark Liu — Manning, 2024
       (available on O'Reilly)
       - Manning-published, GitHub repo with working code.
       - Part 1: GenAI intro + deep learning with PyTorch (ch 1-3)
       - Part 2: Image generation — GANs, CycleGAN, VAEs (ch 4-7)
         ★ Focus here — directly relevant to vision work
       - Part 3: Text generation — RNNs, Transformers from scratch,
                 GPT from scratch (ch 8-12)
         ★ Focus here — you need this for VLMs
       - Part 4: Music generation, diffusion models, LangChain (ch 13-16)
       - Total: ~28 hours
       - Status: [not started]
       - Every chapter builds a working project. All pure PyTorch.

  Prerequisites: Karpathy Zero to Hero (Phase 2A)
  Unlocks: Practical GenAI implementation, Phase 2C and Phase 3
```

### 2C: Pretrained Models & Hugging Face

```
CURRICULUM AREA: Using pretrained models in production
  Phase: 2C
  Status: [not started]

  PRIMARY:
    1. "Hands-On Large Language Models" by Alammar & Grootendorst
       — O'Reilly, 2024
       - Amazon: 4.7/5. Goodreads: 4.33/5. Andrew Ng endorsed it.
       - Full book: ~18 hours
       - Status: [not started]
       - Bridges "I understand how transformers work" to "I can use
         pretrained models effectively." Covers embeddings, semantic
         search, classification, generation, multimodal — all with
         Hugging Face.
       - ★ When you reach the multimodal chapters, spend extra time.
         This is your bridge to VLMs.

  REFERENCE:
    - "NLP with Transformers" by Tunstall, von Werra, Wolf — O'Reilly.
      Written by the Hugging Face team. Use chapters on fine-tuning
      (ch 5-7), the Trainer API, and deployment (ch 8-9) when your
      project specifically needs Hugging Face fine-tuning depth.
    - Jay Alammar's blog (jalammar.github.io) — free. Read "The
      Illustrated Transformer" and "The Illustrated GPT-2" before
      or alongside the book. Best visual explanations ever made.
    - Hugging Face documentation (huggingface.co/docs)
      The best docs in the ML ecosystem. Use for any Hugging Face
      API questions, Trainer API reference, model cards, etc.

  Prerequisites: Phase 2B (or at minimum Karpathy + Mark Liu Part 3)
  Unlocks: Fine-tuning, LoRA, working with pretrained models
```

### 2D: Computer Vision with PyTorch & OpenCV

```
CURRICULUM AREA: Computer vision (practical, deep learning focus)
  Phase: 2D
  Status: [not started — college theory in DIP, CV, Advanced CV]

  ⚠️ RESOURCE CHANGE FROM v3:
    "Modern Computer Vision with PyTorch" (Ayyadevara/Reddy) REMOVED.
    O'Reilly reviews: 2.0/5 (3 reviews). Broken code, poor explanations.
    REPLACED with Elgendy + CS231n below.

  PRIMARY:
    1. "Deep Learning for Vision Systems" by Mohamed Elgendy
       — Manning, 2020 (available on O'Reilly)
       - Amazon: 4.5/5 (200+ ratings). Goodreads: 4.28/5 (43 ratings).
       - Author built and taught the CV course at Amazon's ML University.
       - Read SELECTIVELY (you know the theory from college):
         - Ch 5: Advanced CNN architectures — FULL READ
         - Ch 6: Transfer learning — FULL READ (high priority)
         - Ch 7: Object detection (R-CNN, SSD, YOLO) — FULL READ
         - Ch 8: GANs — SELECTIVE (you covered this with Mark Liu)
         - Ch 9: DeepDream and neural style transfer — SKIM
         - Ch 10: Visual embeddings — FULL READ
         - Ch 1-4: SKIP — CNN basics covered by Karpathy
       - Estimated selective reading: ~18 hours
       - Status: [not started]
       - LIMITATION: Published 2020, so no Vision Transformers (ViTs),
         CLIP, or Stable Diffusion. You get those from the ViT/CLIP
         papers and the VLM book in Phase 3D.

    2. Stanford CS231n lecture notes + assignments — free (cs231n.github.io)
       - Assignment 1: Image classification, kNN, Softmax, fully-connected
         neural network. Implement in NumPy/PyTorch. (~4 hours)
       - Assignment 2: Batch normalisation, dropout, convolutional nets,
         network visualisation. (~4 hours)
       - The 2025 offering includes CLIP and diffusion model assignments.
       - Lecture notes are freely available and updated regularly.
       - Video lectures from 2017 on YouTube (fundamentals unchanged).
       - Total: ~10 hours for assignments 1-2
       - Status: [not started]
       - HOW TO USE: Read the assignment instructions, then implement.
         When stuck, refer to the corresponding lecture notes (not
         solutions). This is deliberate practice — you're implementing
         CV concepts in code, not watching someone else do it.

    3. OpenCV-Python tutorials (docs.opencv.org)
       - Core operations, image I/O, feature detection
       - Learn just-in-time alongside project work
       - Total: ~5 hours
       - Status: [not started]

  VISION-SPECIFIC ADDITIONS:
    - ViT paper: "An Image is Worth 16x16 Words" (Dosovitskiy et al.)
      Read method section + figures (~2-3 hours)
    - Jay Alammar blog: "The Illustrated Stable Diffusion" (~1 hour)
    - DLAI short course: "How Diffusion Models Work" (~1.5 hours)

  REFERENCE:
    - Stanford CS231n lecture notes — for refreshers on any CV topic
    - "Deep Learning" by Goodfellow/Bengio/Courville — CV chapters

  Prerequisites: Phase 2A-2B (PyTorch fluency), college CV theory
  Unlocks: Team CV projects, Phase 3D (VLMs), portfolio projects
```

---

## PHASE 3: LLM Engineering, VLMs, RAG, Agents

```
CURRICULUM AREA: Building with LLMs, vision-language models, RAG, agents
  Weeks: 5-7 (home study) or 7-11 (alongside job)
  Total hours: ~110 hrs
  Status: [not started]
```

### 3A: LLM Engineering

```
CURRICULUM AREA: Building with LLMs in practice
  Phase: 3A
  Status: [not started]

  PRIMARY:
    1. "AI Engineering" by Chip Huyen — O'Reilly, 2025
       - Amazon: 4.7/5. Goodreads: 4.43/5 (933 ratings).
         Most read book on O'Reilly platform since launch.
       - Chapter structure:
         Ch 1-2: AI engineering overview, understanding LLMs
         Ch 3: Evaluation methodology
         Ch 4: Evaluate AI systems (benchmarks, human eval, AI judge)
         Ch 5: Prompt engineering (incl. defensive prompt engineering)
         Ch 6: RAG and Agents (architecture, retrieval, tools, planning)
         Ch 7: Fine-tuning (when to, LoRA, quantization, merging)
         Ch 8: Dataset engineering (curation, synthesis, processing)
         Ch 9: Inference optimization (latency, cost, accelerators)
         Ch 10: AI engineering architecture and user feedback
       - Total: ~20 hours
       - Status: [not started]
       - HOW TO USE: Read sequentially. Each chapter builds on the
         previous. Take notes on decisions and tradeoffs — this book
         teaches you to THINK about LLM systems, not just build them.

  REFERENCE:
    - Labonne's LLM Course (github.com/mlabonne/llm-course)
      NOT a course — it's a curated link index. Use it two ways:

      BEFORE a topic: Scan the DeepWiki version
      (deepwiki.com/mlabonne/llm-course) for 5-10 minutes. It has
      auto-generated architecture diagrams, concept maps, and
      workflow visualizations that orient you on how things connect
      before you dive into Chip Huyen. Do this for every new topic.

      AFTER a topic: Check Labonne's GitHub for curated links to
      hands-on code examples and deeper articles on that subtopic.
      Specific high-value items from Labonne's index:

      For fine-tuning (after Chip Huyen ch 7):
        - "Fine-tune Llama 3.1 with Unsloth" — Labonne's blog + Colab
        - "LoRA insights" by Sebastian Raschka — practical LoRA tips
        - "Mastering LLMs" by Hamel Husain — video collection

      For quantization (after Chip Huyen ch 7/9):
        - "Introduction to quantization" — Labonne's blog + Colab
        - "Quantize with llama.cpp" — Labonne's blog + Colab

      For evaluation (after Chip Huyen ch 3-4):
        - LLM Evaluation Guidebook by Hugging Face
        - Chatbot Arena (lmarena.ai) for understanding human eval

      For architecture/tokenization (after Chip Huyen ch 2):
        - "Visual intro to Transformers" by 3Blue1Brown (YouTube)
        - "LLM Visualization" by Brendan Bycroft (bbycroft.net/llm)
          — interactive 3D visualization of LLM internals
        - Karpathy's tokenization video (YouTube) — already in Phase 2A

    - "Generative AI with LLMs" — DeepLearning.AI (Coursera, ~16 hrs)
      Structured video course covering transformer architecture,
      training, fine-tuning, RLHF. Use if you prefer video format
      after reading Chip Huyen. Skip if concepts are clear.

    - Hugging Face documentation (huggingface.co/docs)
      The best docs in the ML ecosystem. Use for any Hugging Face
      API questions, Trainer API reference, model cards, etc.

  Prerequisites: Phase 2 (PyTorch, transformers, pretrained models)
  Unlocks: Fine-tuning, LoRA, quantization, evaluation, deployment
```

### 3B: RAG Systems

```
CURRICULUM AREA: Retrieval-Augmented Generation
  Phase: 3B
  Status: [not started]

  PRIMARY:
    1. "AI Engineering" by Chip Huyen — Chapter 6 (RAG sections)
       - Covers: RAG architecture, retrieval algorithms, optimization
       - Re-read for depth after initial pass in 3A: ~2 hours

    2. DeepLearning.AI: "Building and Evaluating Advanced RAG" (~1.5 hrs)
       - Hands-on RAG implementation practice with evaluation

    3. DeepLearning.AI: "Preprocessing Unstructured Data for LLMs" (~1.5 hrs)
       - How to prepare documents for RAG ingestion

  REFERENCE:
    - Labonne's LLM Course — RAG section for architecture diagrams
    - Sentence Transformers docs (sbert.net) — embedding model selection
    - Hands-On LLMs (Alammar) — revisit RAG-relevant chapters

  Prerequisites: Phase 3A (Chip Huyen ch 1-6)
  Unlocks: Production RAG systems, Project 2 (Multimodal RAG)
```

### 3C: AI Agents

```
CURRICULUM AREA: Building and evaluating AI agents
  Phase: 3C
  Status: [not started]

  PRIMARY:
    1. "AI Engineering" by Chip Huyen — Chapter 6 (Agent sections)
       - Covers: agent overview, tools, planning, failure modes
       - ~3 hours for the agent-specific sections

  ONLY IF YOU NEED AGENT DEPTH — pick ONE:
    - DeepLearning.AI: "AI Agents in LangGraph" (~1.5 hrs)
    - DeepLearning.AI: "Multi AI Agent Systems with crewAI" (~1.5 hrs)

  REFERENCE:
    - Chip Huyen blog post "Agents" (huyenchip.com/2025/01/07/agents.html)
    - "AI Agents with MCP" by Kyle Stratis — O'Reilly, 2025

  Prerequisites: Phase 3A + 3B
  Unlocks: Office agent projects (if applicable)
```

### 3D: Vision-Language Models ★ VISION SPECIALISATION

```
CURRICULUM AREA: VLMs — critical for vision ML roles
  Phase: 3D
  Status: [not started]
  ★ This section does not exist in the original v3 roadmap.
    It is the most critical addition for vision ML roles.

  PRIMARY:
    1. "Vision Language Models" — O'Reilly (currently in early release)
       - Available on O'Reilly platform. Covers: VLM applications
         (captioning, VQA, visual reasoning, document understanding),
         core architectures, contrastive learning (CLIP), fine-tuning,
         building VLM applications.
       - Total: ~20 hours (estimate based on available chapters)
       - Status: [not started]
       - ⚠️ EARLY RELEASE: Check if all chapters are available when
         you reach this phase. If incomplete, substitute with:
         → Hugging Face VLM tutorials + documentation
         → Lilian Weng blog posts on multimodal models
         → Additional papers (see below)

    2. DeepLearning.AI short courses:
       - "Prompt Vision Models" (~1.5 hrs)
       - "Building Multimodal Search and RAG" (~1.5 hrs)

    3. Key papers (read method sections + experiments only):
       - CLIP (Radford et al., 2021): "Learning Transferable Visual
         Models From Natural Language Supervision" (~2 hrs)
         WHY: CLIP is the foundation of most VLMs. It teaches how
         to align image and text representations. Most VLMs
         use contrastive pre-training derived from CLIP.
       - LLaVA (Liu et al., 2023): "Visual Instruction Tuning" (~2 hrs)
         WHY: LLaVA is the most popular open-source VLM architecture.
         Understanding it means understanding how vision encoders
         connect to language models.
       - LLaVA-NeXT, Qwen-VL, or InternVL (~4 hrs total)
         WHY: These are the state-of-the-art open-source VLMs.
         Reading 2-3 of them gives you landscape awareness.
       - HOW TO READ PAPERS: Read abstract → introduction → method
         section → key figures/tables → experiments/results. Skip
         related work and proofs. Take notes on architecture diagrams.
         Total time per paper should be 1-2 hours, not 4-6.

    4. Hugging Face Transformers VLM documentation:
       - VisionEncoderDecoderModel, Pix2Struct, BLIP-2 pipeline
       - Practice: load 2-3 VLMs from the Hub, run inference,
         inspect outputs (~3 hrs)

  REFERENCE:
    - Lilian Weng's blog (lilianweng.github.io) — multimodal surveys
    - Papers With Code — Vision-Language Models section

  Prerequisites: Phase 2C-2D (pretrained models, CV), Phase 3A
  Unlocks: Projects 2-4, vision ML role readiness
```

### 3E: Document AI & OCR Pipelines ★ VISION SPECIALISATION

```
CURRICULUM AREA: Document processing and visual search
  Phase: 3E
  Status: [not started]
  ★ Key use cases for vision ML roles: document processing,
    visual search, form extraction, structured output extraction.

  PRIMARY:
    1. LayoutLM / LayoutLMv3 paper + Hugging Face implementation
       - LayoutLMv3 (Huang et al., 2022) combines text, layout, and
         image in a single model for document understanding.
       - Read the paper's method section (~1.5 hrs), then follow the
         HF tutorial to run it on a sample document (~1.5 hrs).
       - Total: ~3 hours

    2. Donut (Kim et al., 2022) — OCR-free document understanding
       - Donut skips OCR entirely and reads documents end-to-end.
       - Read method section (~1 hr), run HF demo (~1 hr).
       - Total: ~2 hours

    3. PaddleOCR and Tesseract — OCR baselines
       - Install both, run them on sample Indian documents (Hindi,
         Devanagari script). Compare accuracy. (~2 hrs)
       - WHY: You need to know what baseline OCR can and cannot do
         so you can explain why VLM-based approaches are better.

    4. DeepLearning.AI: "Building Applications with Vector Databases"
       (~1.5 hrs) — for the visual search use case

  REFERENCE:
    - DocVQA benchmark and dataset — how document AI is evaluated
    - "Nougat" paper (Meta) — academic PDFs to structured text

  Prerequisites: Phase 3D (VLM understanding)
  Unlocks: Project 1 (Document Digitisation), vision role readiness
```

---

## PHASE 4: Deepen Foundations & Production

```
CURRICULUM AREA: Theory depth, MLOps, distributed training, alignment
  Weeks: 11-20 (home study) or 14-28 (alongside job)
  Total hours: ~350 hrs
  Status: [not started]
```

### 4A: Probability, Statistics & Data Analysis

```
CURRICULUM AREA: Prob/stats + data manipulation
  Phase: 4A
  Status: [not started]

  PRIMARY:
    1. DeepLearning.AI Math Spec — Course 3: Probability & Statistics
       - ~15 hours. Same quality as Courses 1-2.

    2. "Python for Data Analysis" by Wes McKinney (3rd Ed) — O'Reilly
       - Goodreads: 4.15/5. Written by the creator of pandas.
       - Ch 4-8 selectively: ~14 hours
       - Skip time series chapters unless needed for work

    3. "ML and AI" by Reza Rawassizadeh
       - Ch 3: Statistics & Probability — selective read
         Focus on: KL-divergence, entropy, MLE (~5 hours)
         WHY: These appear in VLM training losses. KL-divergence
         is in every VAE and many fine-tuning objectives.

  REFERENCE:
    - "Practical Statistics for Data Scientists" by Bruce et al.
    - StatQuest with Josh Starmer (YouTube, free)

  Total: ~34 hours
```

### 4B: Databases & SQL

```
CURRICULUM AREA: Databases and SQL
  Phase: 4B
  Status: [not started]

  PRIMARY:
    1. "Learning SQL" by Alan Beaulieu (3rd Ed) — O'Reilly
       - Goodreads: 3.95/5. Standard SQL textbook.
       - Ch 1-8 only: ~10 hours (sufficient for data pipeline work)
```

### 4C: Classical ML — Compressed

```
CURRICULUM AREA: Classical ML (compressed — deep learning is the priority)
  Phase: 4C
  Status: [not started]

  PRIMARY:
    1. "Machine Learning Specialization" by Andrew Ng — DeepLearning.AI
       - Course 1 ONLY: ~30 hours. Skip Courses 2-3.

    2. "Hands-On Machine Learning" by Géron (3rd Ed) — O'Reilly
       - Skim Ch 1-3 only: ~7 hours. Part II skipped.

  Total: ~37 hours
```

### 4D: Deep Learning Theory

```
CURRICULUM AREA: Formal deep learning curriculum
  Phase: 4D
  Status: [not started]

  PRIMARY:
    1. "Deep Learning Specialization" by Andrew Ng — DeepLearning.AI
       - 5 courses, ~80 hrs nominal. Realistically ~50 hrs by
         skipping exercises already covered through project work.

    2. "ML and AI" by Reza Rawassizadeh — selective chapters:
       - Ch 7: Dimensionality Reduction (~5 hrs)
         PCA, t-SNE, UMAP — essential for embedding analysis in VLMs
       - Ch 8: Regression, Regularisation, Optimisation (~5 hrs)
         Gradient descent variants, regularisation — core knowledge
       - Ch 10-12: Neural Networks, Self-Supervised, DL Applications
         SKIM (~8 hrs) — you'll have covered most through projects
       - Ch 14: Making Lighter Neural Networks (~5 hrs) ★ PRIORITY
         Quantisation, pruning, distillation, FlashAttention —
         critical for inference optimisation roles

  REFERENCE:
    - "Deep Learning" by Goodfellow, Bengio, Courville

  Total: ~73 hours (spread across several weeks)
```

### 4E: Distributed Training & Inference Optimisation ★ ADVANCED

```
CURRICULUM AREA: Multi-GPU training, model serving, optimisation
  Phase: 4E
  Status: [not started]
  ★ Covers: FSDP, DeepSpeed, quantisation, serving infrastructure

  PRIMARY:
    1. Hugging Face Accelerate — documentation + tutorials (~4 hrs)
       WHAT THIS IS: A library by Hugging Face that lets you take
       a normal single-GPU training script and run it across multiple
       GPUs with minimal code changes. It handles FSDP (Fully Sharded
       Data Parallel), mixed precision, and gradient accumulation.
       WHAT YOU DO: Read the Accelerate docs "Quick Tour" and
       "Launching distributed training" pages. Then take a training
       script from Phase 2B or 3D and modify it to use Accelerate.
       Run it (even on a single GPU — the API still works).

    2. DeepSpeed — documentation + ZeRO tutorial (~3 hrs)
       WHAT THIS IS: Microsoft's library for training very large
       models efficiently. ZeRO (Zero Redundancy Optimizer) splits
       model parameters, gradients, and optimizer states across GPUs
       so each GPU only holds a fraction. This lets you train models
       that wouldn't fit on a single GPU's memory.
       WHAT YOU DO: Read the DeepSpeed "Getting Started" guide and
       the ZeRO tutorial. Read the ZeRO paper overview (Rajbhandari
       et al., 2020) — just the first 4 pages that explain the three
       stages (ZeRO-1, ZeRO-2, ZeRO-3). You don't need to implement
       this from scratch — you need to understand what it does and
       when to use which stage.

    3. vLLM / TGI — documentation + local deployment (~3 hrs)
       WHAT THIS IS: vLLM is a library for serving LLMs/VLMs in
       production. It implements PagedAttention (efficient memory
       management) and continuous batching (processing multiple
       requests simultaneously instead of one at a time). TGI is
       Hugging Face's alternative serving solution.
       WHAT YOU DO: Install vLLM locally. Download a small model
       (e.g., a 7B parameter model). Start the vLLM server. Send
       it requests using curl or Python. Measure throughput (requests
       per second) at different batch sizes. This is what production
       "batching and serving infrastructure" looks like.

    4. Flash Attention + mixed precision concepts (~3 hrs)
       WHAT THIS IS: Flash Attention (by Tri Dao) is an algorithm
       that computes attention without materialising the full NxN
       attention matrix in GPU memory. This makes attention O(N)
       in memory instead of O(N²). Mixed precision means using
       FP16 or BF16 instead of FP32 for most computations,
       which halves memory usage and doubles throughput.
       WHAT YOU DO: Read Tri Dao's blog post on Flash Attention.
       Read the PyTorch docs on "Automatic Mixed Precision." These
       are concepts you need to UNDERSTAND, not implement — they're
       already built into the libraries you'll use.

    5. FSDP (PyTorch docs) + gradient checkpointing (~3 hrs)
       WHAT THIS IS: FSDP (Fully Sharded Data Parallel) is PyTorch's
       native way to split a model across GPUs. Gradient checkpointing
       trades compute for memory — instead of storing all intermediate
       activations, it recomputes them during the backward pass.
       WHAT YOU DO: Read the PyTorch FSDP tutorial. Read the
       gradient checkpointing docs. Understand when you'd use each.

  REFERENCE:
    - "Machine Learning Systems" by Reddi — Ch 9, Ch 10
    - Megatron-LM paper — skim for vocabulary only

  Total: ~16 hours of reading/tutorials + ~9 hours hands-on = ~25 hrs
```

### 4F: MLOps & Production

```
CURRICULUM AREA: ML in production
  Phase: 4F
  Status: [not started]

  PRIMARY:
    1. "Designing Machine Learning Systems" by Chip Huyen — O'Reilly
       - Amazon: 4.6/5. Goodreads: 4.26/5. ~18 hours.

    2. "MLOps Specialization" — DeepLearning.AI
       - 4 courses: ~40 hours total.

    3. "Machine Learning Systems" by Vijay Janapa Reddi
       — free at mlsysbook.ai
       - Ch 1-2 (systems foundations): ~6 hrs
       - Ch 9 (Efficient AI): ~4 hrs
       - Ch 10 (Model Optimisations): ~5 hrs
       - Ch 13 (ML Operations): ~4 hrs
       - Total selective: ~19 hrs

  Total: ~73 hours
```

### 4G: Post-Training & Alignment ★ ADVANCED

```
CURRICULUM AREA: RLHF, DPO, alignment techniques
  Phase: 4G
  Status: [not started]

  PRIMARY:
    1. DeepLearning.AI short course: "RLHF" (~1.5 hrs)
       WHAT THIS IS: RLHF (Reinforcement Learning from Human Feedback)
       is how models like ChatGPT are fine-tuned to follow instructions
       and be helpful. The course explains the reward model → PPO
       training pipeline.
       WHAT YOU DO: Watch the short course. Do the exercises.

    2. DPO paper (Rafailov et al., 2023) — method + experiments (~2 hrs)
       WHAT THIS IS: DPO (Direct Preference Optimization) is a simpler
       alternative to RLHF. Instead of training a separate reward model,
       DPO directly optimises the language model using human preference
       data. It's become the dominant alignment method because it's
       easier to implement and more stable to train.
       WHAT YOU DO: Read the abstract, introduction, Section 3 (method),
       and Section 5 (experiments). Skip the proofs in Section 4.

    3. Chip Huyen Ch 7 re-read — RLHF/DPO sections (~2 hrs)
       Go back to "AI Engineering" chapter 7 and re-read the fine-tuning
       sections now that you understand RLHF and DPO conceptually.

    4. Hands-on: Fine-tune a small model with TRL using DPO (~4 hrs)
       WHAT THIS IS: TRL (Transformer Reinforcement Learning) is
       Hugging Face's library for RLHF and DPO training. It has
       step-by-step tutorials that walk you through the entire process.
       WHAT YOU DO: Follow the TRL DPO tutorial on Hugging Face docs.
       Take a small model (e.g., a 1B parameter model), a preference
       dataset, and run DPO training. The tutorial gives you every
       line of code — your job is to understand what each line does
       and be able to explain it.

  Total: ~10 hours
```

### 4H: System Design — Optional

```
CURRICULUM AREA: System design (interview prep)
  Phase: 4H
  Status: [not started]

  PRIMARY:
    1. "Machine Learning System Design Interview" by Aminian & Xu
       - Goodreads: 4.15/5. ~12 hours.
       - OPTIONAL. Useful for system design interviews.
```

---

## PORTFOLIO PROJECTS

### How Projects Work (Since You Haven't Built Projects Before)

```
IMPORTANT: You have never built a project from scratch before.
Here is how it works. Every project follows this pattern:

  1. SCOPE: Before writing any code, define EXACTLY what you're building.
     Write a 1-page document: what the inputs are, what the outputs are,
     what "done" looks like. This prevents scope creep.

  2. SKELETON: Create the repo structure. README.md, requirements.txt,
     src/ folder, tests/ folder, .gitignore. Commit this empty skeleton.

  3. BUILD INCREMENTALLY: Break the project into 3-5 milestones.
     Each milestone produces something runnable. You NEVER spend more
     than 2-3 days without something that runs and produces output.

  4. LOOK THINGS UP AS YOU GO: You will encounter tools, libraries,
     and concepts you haven't studied. THIS IS NORMAL. Projects are
     where you learn to learn on the fly. When you hit something new:
     - Check the official documentation first (not Stack Overflow)
     - If it's a core concept gap, go back to the curriculum
     - If it's a "how do I use this API" question, read the docs
     - If you're stuck for more than 30 minutes, ask your AI mentor

  5. TEST AND EVALUATE: Every project has an evaluation component.
     You're not just building — you're measuring whether it works.

  6. DOCUMENT: Write a README that explains what you built, why,
     how to run it, and what the results are. Include screenshots
     or sample outputs. This is what hiring managers will see.
```

### Project 1: Indian Document Digitisation Pipeline

```
PROJECT 1: Indian Document Digitisation Pipeline
  When: Weeks 5-6 (personal time, alongside office onboarding)
  Time: ~25 hours
  Maps to: "Document processing, form extraction, structured output"
  Status: [not started]

  WHAT YOU BUILD:
    A pipeline that takes a photographed document (identity card,
    utility bill, bank statement) and extracts structured fields
    (name, address, ID number, amounts).

  MILESTONES:
    M1 (5 hrs): Set up repo. Collect 20-30 sample documents (photograph
      your own, redact sensitive info). Define the fields you want to
      extract for each document type. Create a simple annotation format
      (JSON) for ground truth.

    M2 (5 hrs): Build OpenCV preprocessing pipeline — deskewing,
      denoising, contrast normalisation. Test on your sample documents.
      Verify visually that preprocessed images are cleaner.

    M3 (5 hrs): Implement OCR layer — run Tesseract (with Hindi/Devanagari
      language pack), PaddleOCR, and EasyOCR on each document. Compare
      raw text output. Measure character-level accuracy where possible.

    M4 (5 hrs): Add VLM-based extraction — use an open-source VLM
      (or API) to directly extract fields from the document image.
      Compare with OCR-based approach. Build a simple evaluation script
      that measures field-level accuracy against your ground truth.

    M5 (5 hrs): Wrap everything in a FastAPI endpoint. Write README.
      Add tests for the preprocessing pipeline. Push to GitHub.

  WHAT YOU'LL LEARN ON THE FLY (not pre-studied):
    - FastAPI basics (read the official tutorial, ~1 hr)
    - How to use PaddleOCR/EasyOCR (read their README + quickstart)
    - How to structure a Python project with multiple modules
    - How to write an evaluation script that compares predictions to GT

  SKILLS DEMONSTRATED:
    Data pipelines, OpenCV, VLMs, evaluation harnesses, production API
```

### Project 2: Multimodal RAG for Indian Educational Content

```
PROJECT 2: Multimodal RAG for Indian Educational Content
  When: Weeks 9-11 (personal time)
  Time: ~35 hours
  Maps to: "Retrieval-augmented workflows," "multimodal pipelines"
  Status: [not started]

  WHAT YOU BUILD:
    A system where an Indian student can ask questions about NCERT
    textbook content (including diagrams and figures) and get answers
    that reference both text and relevant images.

  MILESTONES:
    M1 (7 hrs): Download 2-3 NCERT textbooks (freely available at
      ncert.nic.in). Build PDF ingestion: page images + extracted text.
      Detect which pages have diagrams vs. text-only.

    M2 (7 hrs): Use a VLM to generate captions/descriptions for every
      diagram and figure. Store captions alongside page text.

    M3 (7 hrs): Index everything in a vector store (ChromaDB or FAISS).
      Text chunks get embedded with a text embedder. Image descriptions
      get embedded alongside. Build a query function.

    M4 (7 hrs): Build query interface. Student asks a question in
      English or Hindi → retrieve relevant text + images → generate
      answer using an LLM with retrieved context.

    M5 (7 hrs): Evaluate. Build a 50-question test set. Measure
      recall@5 (are the right documents retrieved?) and answer
      relevance (is the answer correct?). Write up results + README.

  WHAT YOU'LL LEARN ON THE FLY:
    - ChromaDB/FAISS usage (read quickstart docs)
    - PDF processing in Python (PyMuPDF or pdfplumber)
    - Embedding model selection (check MTEB leaderboard)
    - How to structure a RAG evaluation pipeline
```

### Project 3: Fine-Tuning a VLM for Indian Visual QA

```
PROJECT 3: Fine-Tuning a VLM for Indian Visual Question Answering
  When: Weeks 12-15 (personal time)
  Time: ~45 hours
  Maps to: "Training and fine-tuning large models," "vision-language models"
  Status: [not started]

  WHAT YOU BUILD:
    Fine-tune an open-source VLM on Indian visual content so it better
    understands Indian-specific images (Devanagari text, Indian currency,
    Indian food, Indian architecture).

  MILESTONES:
    M1 (10 hrs): DATASET CURATION. This is the hardest part.
      Collect ~500-1000 image-question-answer triples:
      - Photograph Indian street signs, menus, buildings
      - Use Creative Commons images from Wikimedia
      - Write questions in English and Hindi
      - Write ground truth answers
      Format as JSON. Split into train/val/test.

    M2 (10 hrs): FINE-TUNING SETUP. Choose base model (LLaVA-1.5 7B
      or similar). Set up training with LoRA using HF TRL or
      LLaMA-Factory. Document every decision: learning rate, LoRA rank,
      batch size, number of epochs. Run a short training run (~100 steps)
      to verify nothing crashes before committing to full training.

    M3 (10 hrs): FULL TRAINING + DEBUGGING. Run full fine-tuning.
      Monitor loss curves. Debug any issues (NaN losses, memory errors,
      degrading performance). This is where you learn to "debug broken
      training runs" — a core ML engineering skill.

    M4 (10 hrs): EVALUATION. Build automated metrics (accuracy for VQA,
      BLEU/CIDEr for captioning). Also do manual evaluation on 50
      examples. Document failure modes: what does the model get wrong?
      Where does it hallucinate?

    M5 (5 hrs): INFERENCE OPTIMISATION. Quantise the fine-tuned model
      (GPTQ or AWQ). Measure latency vs. quality trade-off. Write up
      everything in a technical blog post format.

  WHAT YOU'LL LEARN ON THE FLY:
    - LoRA configuration and training (TRL docs)
    - Dataset formatting for VLM fine-tuning
    - How to monitor training with Weights & Biases or TensorBoard
    - Quantisation tools (AutoGPTQ, bitsandbytes)
```

### Project 4: Serving Infrastructure for Vision Models

```
PROJECT 4: Serving Infrastructure for Vision Models
  When: Week 18 (personal time, after distributed training study)
  Time: ~25 hours
  Maps to: "Quantisation, batching, serving infrastructure"
  Status: [not started]

  WHAT YOU BUILD:
    A production-ready serving pipeline for a VLM with benchmarks
    showing the impact of different optimisation strategies.

  MILESTONES:
    M1 (5 hrs): Take your fine-tuned model from Project 3 (or a
      public VLM). Implement three quantisation levels: FP16 → INT8 →
      INT4. Measure quality on your eval set at each level.

    M2 (5 hrs): Deploy with vLLM. Configure continuous batching.
      Measure throughput at batch sizes 1, 4, 8, 16, 32.

    M3 (5 hrs): Build FastAPI server with health checks, request
      queuing, timeout handling. Add Prometheus metrics: latency
      p50/p95/p99, throughput, GPU memory usage, error rate.

    M4 (5 hrs): Load test with Locust or k6. Produce a benchmark
      report with concrete numbers and graphs.

    M5 (5 hrs): Write a technical blog post comparing the three
      optimisation strategies. Push everything to GitHub.

  WHAT YOU'LL LEARN ON THE FLY:
    - vLLM server configuration
    - Prometheus + Grafana basics (or just Prometheus client library)
    - Load testing with Locust (read their quickstart)
    - How to write a technical benchmark report
```

### Project 5: Open-Source Contributions

```
PROJECT 5: Open-Source Contributions
  When: Ongoing from Week 8
  Maps to: "Contributions to open-source projects or solid GitHub portfolio"
  Status: [not started]

  TARGET REPOS (pick 1-2):
    - vLLM (github.com/vllm-project/vllm) — serving infrastructure
    - Hugging Face Transformers — VLM implementations
    - LLaVA or InternVL — fix bugs you find during Project 3
    - PaddleOCR — Indic script improvements from Project 1

  APPROACH:
    Week 8-9:   Documentation and test improvements (low risk, learn
                the codebase). Read CONTRIBUTING.md. Look at "good first
                issue" labels. Submit 1-2 small PRs.
    Week 10-12: Bug fixes. Pick reported issues, reproduce them
                locally, write a fix. Submit PRs with tests.
    Week 14-16: Small feature or improvement. By now you know the
                codebase. Propose something useful.
    Target: 3-5 merged PRs before applying to jobs.
```

---

## What Was Deprioritised or Removed

```
REMOVED:
  "Modern CV with PyTorch" (Ayyadevara/Reddy) — 2.0/5 reviews, broken code
    → Replaced with Elgendy "DL for Vision Systems" + CS231n assignments

SKIPPED (not needed for initial competency):
  Andrew Ng ML Specialization Courses 2-3 — classical ML depth
  Reza Ch 4 (Clustering), Ch 5 (Freq Itemset), Ch 6 (Feature Eng),
    Ch 9 (Classification) — classical ML algorithms
  Reza Ch 13 (Reinforcement Learning) — not relevant
  Reza Ch 15 (Graph Mining) — specialised
  Matplotlib/Seaborn/Plotly deep dives — learn through projects
  Multiple agent framework courses — one is enough
  ISLP, UDL books — redundant (see v3 analysis)
  ML System Design Interview book — optional

DEFERRED TO REFERENCE:
  Reza Ch 4, 5, 6, 9 — read only if needed for a specific project
  "Hands-On ML" by Géron Part II — covered by Karpathy + Mark Liu
```

---

## Design Principles

```
1. No redundancy. Every resource earns its place.
2. Implementation first. Pretrained models, PyTorch, LLMs, CV, RAG.
3. College theory is leverage. You covered ML, DL, DIP, CV theory.
   The plan gets you to implementation faster than a true beginner.
4. Free resources are often the best. Karpathy, 3Blue1Brown, fast.ai,
   Jay Alammar — world-class and free.
5. One primary resource per topic. Supplements and references clearly
   marked so you know what's core vs. optional.
6. Specialisation without sacrificing breadth. VLMs and vision are
   front-loaded, but the full AI stack is completed by Week 20 (home
   study) or Week 28 (alongside a job).
7. Every resource vetted. Ratings checked, reviews read, alternatives
   evaluated. See FILE 3 (Resource Registry) for full vetting data.
8. Projects teach through building. You will encounter things you
   haven't studied. Look them up. This is how real engineers work.
```
