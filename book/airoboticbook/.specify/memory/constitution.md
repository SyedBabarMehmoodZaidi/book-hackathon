<!--
Sync Impact Report:
Version change: 1.0.0 → 2.0.0
List of modified principles: All core principles, key standards, constraints, and success criteria updated to reflect "Book on Teaching Physical AI & Humanoid Robotics" project.
Added sections: Content Requirements, Technical Constraints, Output Behavior for Claude
Removed sections: None (existing sections were redefined/expanded)
Templates requiring updates: ✅ .specify/templates/plan-template.md, ✅ .specify/templates/spec-template.md, ✅ .specify/templates/tasks-template.md, ✅ .specify/templates/commands/*.md
Follow-up TODOs: None
-->
# Book on Teaching Physical AI & Humanoid Robotics using Docusaurus + GitHub Pages Constitution

## Core Principles

### Accuracy and Technical Correctness
All robotics, AI, and engineering concepts MUST be accurate and technically correct.

### Clarity for Learners
Content MUST be clear for learners ranging from beginners to intermediate robotics developers.

### Modularity
Each chapter MUST be standalone and reusable.

### Practical Usefulness
Content MUST include practical usefulness (examples, real-world analogies, applicable code).

### Consistency
Consistency in terminology, definitions, and structure across chapters MUST be maintained.

### Educational Focus
Content MUST be educationally focused and aligned with modern AI-native and robotics practices.

## Key Standards

- All factual/technical claims MUST come from reliable sources (robotics research papers, ROS docs, AI textbooks, authoritative blogs).
- Any algorithm or robotics concept MUST be explained step-by-step.
- Code samples MUST be tested and runnable.
- Writing level: Flesch-Kincaid Grade 8–10 for readability.
- Tone: Educational, structured, and friendly.
- Style: Non-fiction, technical writing, section-based.

## Content Requirements

- Book structure: 10 Chapters, each containing 6–8 headings/subsections.
- Include one meta description for each chapter (≤ 30 words).
- Minimum chapter length: 600+ words each.
- Each chapter MUST include at least one:
    - diagram description (for later image generation)
    - practical example
    - short exercise or activity
- Include glossary terms when needed.
- No plagiarism, all text MUST be original.

## Technical Constraints

- Format: Markdown (.mdx) compatible with Docusaurus.
- All images referenced MUST be placed in static/img/.
- MUST follow Docusaurus folder structure:
    - docs/ → All book chapters
    - sidebar.js → Auto-generated or manually written
- Chapters MUST be exportable to GitHub Pages build.
- Compatible with Claude Code workflows.

## Success Criteria

- Book builds successfully in Docusaurus without errors.
- All chapters meet word count & section requirements.
- Writing is clear, accurate, and original.
- Easy to navigate in sidebar structure.
- Passes internal technical review (AI + robotics expert level).
- Ready for public deployment on GitHub Pages.

## Output Behavior for Claude

When writing chapters or sections:
- Follow the constitution strictly.
- Use simple, clean explanations.
- Include real-world robotics and AI examples.
- Avoid unnecessary jargon.
- Structure output cleanly in Markdown.
- Treat each chapter as modular and standalone.
- Always check consistency (terms, headings, tone).

## Governance
Constitution supersedes all other practices; Amendments require documentation, approval, migration plan. All PRs/reviews must verify compliance; Complexity must be justified; Use relevant guidance files for runtime development guidance.

**Version**: 2.0.0 | **Ratified**: 2025-12-04 | **Last Amended**: 2025-12-04
