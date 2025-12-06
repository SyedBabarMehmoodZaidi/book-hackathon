# Tasks: Book on Teaching Physical AI & Humanoid Robotics

**Input**: Design documents from `/specs/1-robotics-book/`
**Prerequisites**: plan.md (required), spec.md (required for user stories), research.md, data-model.md, contracts/

**Tests**: The spec does not explicitly request generating test tasks, so only content creation and setup tasks are included.

**Organization**: Tasks are grouped by user story to enable independent implementation and testing of each story.

## Format: `[ID] [P?] [Story] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1, US2, US3)
- Include exact file paths in descriptions

## Path Conventions

- **Project Structure**: Docusaurus-based, as defined in `specs/1-robotics-book/plan.md`
- All content paths will be relative to the `docs/` directory for chapters and `static/img/` for images.

---

## Phase 1: Setup (Shared Infrastructure)

**Purpose**: Project initialization and basic Docusaurus structure.

- [ ] T001 Initialize Docusaurus project in the root directory
- [ ] T002 Create `docs/intro.mdx` for the book introduction
- [ ] T003 [P] Create `docs/module1-ros2/_category_.json` for Module 1 sidebar configuration
- [ ] T004 [P] Create `docs/module2-simulation/_category_.json` for Module 2 sidebar configuration
- [ ] T005 [P] Create `docs/module3-nvidia-isaac/_category_.json` for Module 3 sidebar configuration
- [ ] T006 [P] Create `docs/module4-vla/_category_.json` for Module 4 sidebar configuration
- [ ] T007 [P] Create `docs/module5-capstone/_category_.json` for Module 5 sidebar configuration
- [ ] T008 [P] Create `docs/appendices/hardware-setup.mdx`
- [ ] T009 [P] Create `docs/appendices/software-installation.mdx`
- [ ] T010 [P] Create `docs/appendices/glossary.mdx`
- [ ] T011 Update `docusaurus.config.js` with project metadata and sidebar configuration
- [ ] T012 Configure `sidebar.js` to reflect the book's chapter structure
- [ ] T013 Create `static/img/` directory for diagrams and images

---

## Phase 2: Foundational (Blocking Prerequisites)

**Purpose**: Core infrastructure that MUST be complete before ANY user story content can be implemented.

**⚠️ CRITICAL**: No user story content creation can begin until this phase is complete.

- [ ] T014 Review and ensure all project dependencies (Docusaurus, necessary plugins) are installed in `package.json`
- [ ] T015 Verify Docusaurus build process with a minimal setup
- [ ] T016 Confirm image referencing (`static/img/`) works correctly in a sample `.mdx` file

**Checkpoint**: Foundation ready - user story content creation can now begin in parallel.

---

## Phase 3: User Story 1 - Understand ROS 2 Fundamentals (Priority: P1) 🎯 MVP

**Goal**: Learners understand core ROS 2 concepts and Python integration for humanoid robot control.

**Independent Test**: Reader can create ROS 2 nodes/packages, publish/subscribe to topics, and visualize joint movement in RViz.

### Implementation for User Story 1

- [ ] T017 [US1] Draft `docs/module1-ros2/chapter1.mdx` covering Introduction to ROS 2, Nodes, Topics, Services, Actions, and Python integration (rclpy)
- [ ] T018 [US1] Draft `docs/module1-ros2/chapter2.mdx` covering URDF, Launch files, Parameter management, and Hands-on: basic ROS 2 node network and controlling a humanoid joint
- [ ] T019 [US1] Add practical examples and short exercises for ROS 2 concepts within `docs/module1-ros2/` chapters
- [ ] T020 [US1] Add textual diagram descriptions to `docs/module1-ros2/` chapters where needed
- [ ] T021 [US1] Ensure meta descriptions are included for `docs/module1-ros2/` chapters

**Checkpoint**: At this point, User Story 1 content should be drafted and internally consistent.

---

## Phase 4: User Story 2 - Simulate Humanoid Robots (Priority: P1)

**Goal**: Learners simulate humanoid robots in virtual environments (Gazebo/Unity) with physics and sensor data.

**Independent Test**: Reader can create a Gazebo world, simulate sensors, and visualize robot behavior in Unity.

### Implementation for User Story 2

- [ ] T022 [US2] Draft `docs/module2-simulation/chapter3.mdx` covering Introduction to simulation, Digital Twin concept, Gazebo physics (collisions, gravity, dynamics)
- [ ] T023 [US2] Draft `docs/module2-simulation/chapter4.mdx` covering Unity rendering, Human-robot interaction, Sensor simulation (LIDAR, Depth Cameras, IMUs), and Synchronizing simulation with ROS 2
- [ ] T024 [US2] Add hands-on sections for building a humanoid simulation and navigating a virtual environment within `docs/module2-simulation/` chapters
- [ ] T025 [US2] Add textual diagram descriptions to `docs/module2-simulation/` chapters where needed
- [ ] T026 [US2] Ensure meta descriptions are included for `docs/module2-simulation/` chapters

**Checkpoint**: At this point, User Stories 1 AND 2 content should be drafted and internally consistent.

---

## Phase 5: User Story 3 - Train AI for Robot Control (Priority: P2)

**Goal**: Learners use NVIDIA Isaac Sim and Isaac ROS to train humanoid robots for perception, navigation, and AI-driven behavior.

**Independent Test**: Reader can train perception models, implement VSLAM-based navigation, and understand sim-to-real transfer.

### Implementation for User Story 3

- [ ] T027 [US3] Draft `docs/module3-nvidia-isaac/chapter5.mdx` covering Introduction to NVIDIA Isaac Sim, Photorealistic simulation, and Synthetic data generation
- [ ] T028 [US3] Draft `docs/module3-nvidia-isaac/chapter6.mdx` covering Isaac ROS perception pipelines (VSLAM), Nav2 path planning, Reinforcement learning basics, and Sim-to-real transfer techniques
- [ ] T029 [US3] Add hands-on sections for perception and navigation pipeline within `docs/module3-nvidia-isaac/` chapters
- [ ] T030 [US3] Add textual diagram descriptions to `docs/module3-nvidia-isaac/` chapters where needed
- [ ] T031 [US3] Ensure meta descriptions are included for `docs/module3-nvidia-isaac/` chapters

**Checkpoint**: At this point, User Stories 1, 2, AND 3 content should be drafted and internally consistent.

---

## Phase 6: User Story 4 - Enable Voice Command Control (Priority: P2)

**Goal**: Learners integrate language models and speech recognition with humanoid robots for autonomous voice-command execution.

**Independent Test**: Reader can implement a voice-command pipeline and convert natural language to robot actions.

### Implementation for User Story 4

- [ ] T032 [US4] Draft `docs/module4-vla/chapter7.mdx` covering Introduction to VLA in robotics, OpenAI Whisper (voice-to-action commands), and Cognitive planning
- [ ] T033 [US4] Draft `docs/module4-vla/chapter8.mdx` covering Multi-modal interaction (speech, gesture, vision), and Integration with NVIDIA Isaac and ROS 2
- [ ] T034 [US4] Add hands-on section for a simple voice-command humanoid robot within `docs/module4-vla/` chapters
- [ ] T035 [US4] Add textual diagram descriptions to `docs/module4-vla/` chapters where needed
- [ ] T036 [US4] Ensure meta descriptions are included for `docs/module4-vla/` chapters

**Checkpoint**: At this point, User Stories 1, 2, 3, AND 4 content should be drafted and internally consistent.

---

## Phase 7: User Story 5 - Deploy Autonomous Humanoid (Priority: P1 - Capstone)

**Goal**: Learners design and deploy a fully autonomous humanoid robot performing navigation, perception, and object manipulation tasks, integrating all learned concepts.

**Independent Test**: Reader can simulate and deploy a full humanoid task, including integration of ROS 2, Isaac, and VLA pipeline.

### Implementation for User Story 5

- [ ] T037 [US5] Draft `docs/module5-capstone/chapter9.mdx` covering Capstone overview, Hardware/software integration, Autonomous navigation planning, and Object identification and manipulation
- [ ] T038 [US5] Draft `docs/module5-capstone/chapter10.mdx` covering Multi-modal interaction (speech, vision, gesture), Sim-to-real deployment on edge kit, and Assessment and success criteria
- [ ] T039 [US5] Add exercises for simulating and deploying a full humanoid task in `docs/module5-capstone/` chapters
- [ ] T040 [US5] Add textual diagram descriptions to `docs/module5-capstone/` chapters where needed
- [ ] T041 [US5] Ensure meta descriptions are included for `docs/module5-capstone/` chapters

**Checkpoint**: All user story content should now be drafted and internally consistent.

---

## Phase 8: Polish & Cross-Cutting Concerns

**Purpose**: Improvements that affect multiple user stories and overall book quality.

- [ ] T042 Review all chapters for Flesch-Kincaid Grade 8–10 readability (`docs/`)
- [ ] T043 Review all chapters for consistency in terminology, definitions, and structure (`docs/`)
- [ ] T044 Review `docs/appendices/hardware-setup.mdx` for accuracy and completeness
- [ ] T045 Review `docs/appendices/software-installation.mdx` for accuracy and completeness
- [ ] T046 Review `docs/appendices/glossary.mdx` for completeness
- [ ] T047 Verify all chapters meet minimum 600+ word count (`docs/`)
- [ ] T048 Verify all chapters have 6-8 headings/subsections (`docs/`)
- [ ] T049 Verify all chapters have a meta description (≤30 words) (`docs/`)
- [ ] T050 Verify all chapters include at least one diagram description, practical example, and short exercise/activity (`docs/`)
- [ ] T051 Perform plagiarism check across all content (`docs/`)
- [ ] T052 Final review of `docusaurus.config.js` and `sidebar.js` for correctness
- [ ] T053 Build Docusaurus project and verify no errors or broken links
- [ ] T054 Perform Lighthouse audit for performance (>90 score) and accessibility (WCAG 2.1)

---

## Dependencies & Execution Order

### Phase Dependencies

- **Setup (Phase 1)**: No dependencies - can start immediately
- **Foundational (Phase 2)**: Depends on Setup completion - BLOCKS all user stories.
- **User Stories (Phase 3-7)**: All depend on Foundational phase completion.
  - User stories can then proceed in parallel (if staffed) or sequentially in priority order (P1 → P2 → P3).
- **Polish (Phase 8)**: Depends on all desired user stories content being complete.

### User Story Dependencies

- **User Story 1 (P1)**: Can start after Foundational (Phase 2) - Foundational for subsequent modules.
- **User Story 2 (P1)**: Can start after Foundational (Phase 2) - Depends on US1 for ROS 2 fundamentals.
- **User Story 3 (P2)**: Can start after Foundational (Phase 2) - Depends on US1 and US2.
- **User Story 4 (P2)**: Can start after Foundational (Phase 2) - Depends on US1, US2, and US3.
- **User Story 5 (P1 - Capstone)**: Can start after Foundational (Phase 2) - Depends on US1, US2, US3, and US4.

### Within Each User Story

- Drafting foundational chapters before more advanced ones.
- Adding examples and exercises as content is drafted.
- Textual diagram placeholders should be added during drafting.

### Parallel Opportunities

- Tasks marked [P] within Phase 1 (Setup) can run in parallel.
- Different chapters within the same module (if applicable and content is distinct enough) could be drafted in parallel.
- Once foundational content for a module is laid out, the detailed drafting of individual chapters can potentially be parallelized.
- Once all core module content is drafted, some tasks in the Polish & Cross-Cutting Concerns phase (e.g., readability review, plagiarism check) can be initiated in parallel.

---

## Parallel Example: Content Creation for Module 1 (US1)

```bash
# Draft chapters for Module 1 concurrently:
Task: "Draft docs/module1-ros2/chapter1.mdx covering ROS 2 introduction..."
Task: "Draft docs/module1-ros2/chapter2.mdx covering URDF, Launch files..."

# Add details to drafted chapters concurrently:
Task: "Add practical examples and short exercises for ROS 2 concepts within docs/module1-ros2/ chapters"
Task: "Add textual diagram descriptions to docs/module1-ros2/ chapters where needed"
```

---

## Implementation Strategy

### MVP First (Module 1 Only)

1. Complete Phase 1: Setup
2. Complete Phase 2: Foundational (CRITICAL - blocks all content creation)
3. Complete Phase 3: User Story 1 (Module 1 content)
4. **STOP and VALIDATE**: Review Module 1 content for clarity, accuracy, and adherence to requirements. Build Docusaurus and verify Module 1 renders correctly.
5. Deploy/demo if ready (e.g., a preview of the first module).

### Incremental Delivery

1. Complete Setup + Foundational → Foundation ready.
2. Add User Story 1 (Module 1) → Review independently → Deploy/Demo (MVP!).
3. Add User Story 2 (Module 2) → Review independently → Deploy/Demo.
4. Continue for User Stories 3, 4, and 5 sequentially.
5. Each completed module adds value and integrates with previous modules.

### Parallel Team Strategy

With multiple content creators/developers:

1. Team completes Setup + Foundational together.
2. Once Foundational is done:
   - Content Creator A: User Story 1 (Module 1)
   - Content Creator B: User Story 2 (Module 2)
   - Content Creator C: User Story 3 (Module 3)
   - Content Creator D: User Story 4 (Module 4)
   - Content Creator E: User Story 5 (Module 5)
3. Modules are drafted and reviewed; integration points (e.g., ROS 2 basics from M1 in M2) are coordinated.

---

## Notes

- [P] tasks = different files, no direct blocking dependencies
- [Story] label maps task to specific user story/module for traceability
- Each user story/module should be independently completable and testable (content-wise)
- Commit after each task or logical group of tasks.
- Stop at any checkpoint to validate content independently.
- Avoid: vague tasks, cross-module dependencies that break independent review.
