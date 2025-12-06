---
id: 0002
title: Update project constitution for robotics book
stage: constitution
date: 2025-12-04
surface: agent
model: claude-sonnet-4-5-20250929
feature: none
branch: main
user: unknown
command: /sp.constitution
labels: ["constitution", "update", "robotics"]
links:
  spec: null
  ticket: null
  adr: null
  pr: null
files:
  - .specify/memory/constitution.md
tests:

---

## Prompt

```text
    Project: Book on Teaching Physical AI & Humanoid Robotics using Docusaurus + GitHub Pages
Core Principles:

Accuracy and technical correctness in all robotics, AI, and engineering concepts

Clarity for learners ranging from beginners to intermediate robotics developers

Modularity (each chapter must be standalone and reusable)

Practical usefulness (examples, real-world analogies, applicable code)

Consistency in terminology, definitions, and structure across chapters

Educational focus aligned with modern AI-native and robotics practices

Key Standards

All factual/technical claims must come from reliable sources (robotics research papers, ROS docs, AI textbooks, authoritative blogs)

Any algorithm or robotics concept must be explained step-by-step

Code samples must be tested and runnable

Writing level: Flesch-Kincaid Grade 8–10 for readability

Tone: Educational, structured, and friendly

Style: Non-fiction, technical writing, section-based

Content Requirements

Book structure: 10 Chapters, each containing 6–8 headings/subsections

Include one meta description for each chapter (≤ 30 words)

Minimum chapter length: 600+ words each

Each chapter must include at least one:

diagram description (for later image generation)

practical example

short exercise or activity

Include glossary terms when needed

No plagiarism, all text must be original

Technical Constraints

Format: Markdown (.mdx) compatible with Docusaurus

All images referenced must be placed in static/img/

Must follow Docusaurus folder structure:

docs/ → All book chapters

sidebar.js → Auto-generated or manually written

Chapters must be exportable to GitHub Pages build

Compatible with Claude Code workflows

Success Criteria

Book builds successfully in Docusaurus without errors

All chapters meet word count & section requirements

Writing is clear, accurate, and original

Easy to navigate in sidebar structure

Passes internal technical review (AI + robotics expert level)

Ready for public deployment on GitHub Pages

Output Behavior for Claude

When writing chapters or sections:

Follow the constitution strictly

Use simple, clean explanations

Include real-world robotics and AI examples

Avoid unnecessary jargon

Structure output cleanly in Markdown

Treat each chapter as modular and standalone

Always check consistency (terms, headings, tone)
```

## Response snapshot

The project constitution was updated to version 2.0.0 based on the provided input for "Book on Teaching Physical AI & Humanoid Robotics using Docusaurus + GitHub Pages". A Prompt History Record (PHR) has been created to document this.

## Outcome

- ✅ Impact: Constitution updated to version 2.0.0 and PHR created.
- 🧪 Tests: No explicit tests were run for this constitution update.
- 📁 Files: `.specify/memory/constitution.md` updated and PHR created for the action.
- 🔁 Next prompts: None
- 🧠 Reflection: PHR created to document the constitution update process.

## Evaluation notes (flywheel)

- Failure modes observed: None
- Graders run and results (PASS/FAIL): N/A
- Prompt variant (if applicable): N/A
- Next experiment (smallest change to try): N/A
