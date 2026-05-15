# Cursor Rules — Setup Guide



## A Gist of These Files and What they Intend to Do

**`core-learning.mdc`** is the only rule set to `alwaysApply: true` — it runs in every conversation inside Cursor regardless of file type. It contains your current Independence Ladder rung (starts at 1) and tells the AI exactly what it's allowed and not allowed to do at each rung. The key mechanism is a `CURRENT_RUNG = 1` variable at the top that you manually bump as you progress. At Rung 1, the AI literally refuses to write code for you. At Rung 3, it won't even answer questions you could find in documentation. This is the guard rail that prevents the old dependency pattern from creeping back in.

**`python-quality.mdc`** triggers on `.py` files and enforces your Clean Code from Day 1 practices — type hints are mandatory, functions do one thing, meaningful names, error handling, tests expected. When the AI reviews your code, it checks these in a specific order: type hints first, then structure, then correctness. This means even your Week 1 practice scripts get held to the standard.

**`ml-projects.mdc`** triggers on `.py` files and adds ML-specific standards: proper project structure (model separate from training loop), hyperparameters in config files not hardcoded, reproducibility (random seeds), evaluation on held-out data, checkpoint saving. This kicks in when you're building Projects 1-4.

**`resource-guidance.mdc`** contains a quick-reference of your Roadmap v5 resources organized by phase, so Cursor's AI can point you to the right book/chapter when you hit a gap — without you needing to paste the entire roadmap into every chat.

**`portfolio-projects.mdc`** triggers on README files and enforces that every portfolio project has proper structure, a README that a hiring manager can understand in 60 seconds, evaluation with concrete metrics, and no hardcoded paths or secrets.

**`coding-practice.mdc`** triggers in `practice/` and `exercises/` folders and enforces the daily reps protocol: typed not copy-pasted, written from memory, type hints even in practice code, Exercism exercises tracked.

**To install:** Copy the `.cursor/` folder into every project or study folder you create. The README explains both per-project and global installation. When you progress on the ladder, edit the `CURRENT_RUNG` value in `core-learning.mdc` — that single change shifts how every AI interaction works across the entire project.

## What These Rules Do in Short

These Cursor rules enforce the learning system from your Learning Prompt v3.0
and Complete Roadmap v5. They ensure that the AI in Cursor:

1. **Doesn't write code for you** when you should be writing it yourself
2. **Enforces clean code practices** (type hints, testing, meaningful names)
3. **Points you to the right resource** instead of hand-holding through gaps
4. **Maintains ML project standards** (proper structure, evaluation, reproducibility)
5. **Enforces portfolio project quality** for your Sarvam GitHub portfolio

## The 5 Rule Files

```
.cursor/rules/
├── core-learning.mdc       ← ALWAYS APPLIED. Independence Ladder,
│                              anti-dependency rules. The AI adapts its
│                              behaviour based on your current rung.
│
├── python-quality.mdc      ← Applied to .py files. Type hints, clean code,
│                              testing expectations. The AI reviews your
│                              code against these standards.
│
├── ml-projects.mdc         ← Applied to .py files in ML projects. PyTorch
│                              conventions, experiment tracking, evaluation,
│                              project structure.
│
├── resource-guidance.mdc   ← Applied when you have a knowledge gap. Tells
│                              the AI how to recommend resources from your
│                              Roadmap v5 or via web search.
│
├── portfolio-projects.mdc  ← Applied to README files. Enforces project
│                              structure, documentation, evaluation, and
│                              GitHub presentation standards.
│
└── coding-practice.mdc     ← Applied to practice/ and exercises/ folders.
                               Enforces daily coding reps, from-memory
                               writing, and exercise tracking.
```

## How to Install

### Option 1: Copy to Every Project (Recommended)

For each project or study folder you create, copy the `.cursor/` directory:

```bash
cp -r /path/to/cursor-rules/.cursor /path/to/your-project/

HERE->
cp -r "/Users/vanshpahwa/Desktop/Complete-AI-Enginering/Learning_Folder_V3-V5/cursor-rules/.cursor" /path/to/your-project/
```

This gives each project its own rules. Commit them to git so they persist.

### Option 2: Global User Rules (Simpler but Less Control)

Open Cursor → Settings → Rules → User Rules. Paste the contents of
`core-learning.mdc` there. This applies globally but only supports
plain text (no globs, no conditional application).

For the full power of conditional rules (e.g., python-quality only
applying to .py files), use Option 1.

## How to Update Your Rung

When you progress on the Independence Ladder, edit `core-learning.mdc`
and change the line:

```
CURRENT_RUNG = 1
```

to your new rung (1, 2, 3, or 4). This changes how the AI interacts
with you across ALL conversations in that project.

**Rung transition guide:**
- Start at Rung 1 (Weeks 1-3). You're studying, not building.
- Move to Rung 2 when you can write a 50-line script without help,
  read docs independently, and debug simple errors from tracebacks.
- Move to Rung 3 when you can design a system, choose tools, and
  implement a feature with only occasional questions.
- Move to Rung 4 when you're contributing to open source and reading
  research papers. The AI is now a peer, not a guide.

## How These Rules Interact with Your Learning Prompt

Your Learning Prompt v3.0 (pasted into Claude/ChatGPT conversations)
defines HOW you learn. These Cursor rules define HOW THE IDE AI BEHAVES
while you're writing code. They complement each other:

- Learning Prompt → for chat-based learning conversations
- Cursor Rules → for in-IDE coding assistance

Both enforce the same principles: independence, clean code, proper
resources, no dependency on AI-generated code you don't understand.



## 
