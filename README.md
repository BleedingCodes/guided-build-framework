# Guided Build Framework

Execution-focused AI framework for realistic project evaluation, incremental building, and hands-on learning guidance.

---

## Origins

This framework started with an AI-assisted idea generator prompt.

The idea generator helped produce project concepts, but it also revealed a problem: ideas are easy to generate, but finished builds require structure, scope, and discipline.

The Guided Build Framework exists to bridge that gap.

It turns raw project ideas into smaller, testable, buildable steps so that AI becomes a guide instead of a shortcut.

---

## Framework Editions

The framework ships in three editions. Each is a self-contained file — paste it as a user message in any AI chat session to start.

| Edition | File | Use When |
|---|---|---|
| **Core** | `framework/Idea_Generator.md` + `framework/idea_evaluation_system.md` | You want to generate and evaluate ideas across any domain you define |
| **3D Python Games** | `framework/Python3d-games-idea-gener-n-tester.md` | You want to build real-time 3D games in Python (Ursina, Panda3D, PyOpenGL, raylib-py) |
| **Public API + Python** | `framework/Free-Public-API-n-Python-idea-gener-n-tester.md` | You want to build Python tools that talk to real, live, free public APIs |

All three editions share the same three-phase structure and the same 15-point stress test. What differs is the domain — the constraints, the idea format fields, and the specific risk categories the stress test targets.

---

## Which Edition to Use

**Use the Core edition** if your domain isn't listed above, or if you want to supply your own topic list and let the framework handle evaluation. Edit the domain list at the top of `Idea_Generator.md` to match your interests.

**Use the 3D Python Games edition** if you want to build real rendered 3D projects in Python. This edition adds: Library/Engine selection per idea, GPU/driver and Linux platform risk analysis, asset pipeline warnings, camera/controls complexity flags, and a ban on terminal/ASCII output — every idea must open a real window.

**Use the Public API edition** if you want to build Python tools that fetch, combine, log, or react to live internet data. This edition adds: Auth Type per idea (none / free API key / free-tier signup / OAuth), rate-limit and key-acquisition risk analysis, secret management guidance, and a ban on mocked or hardcoded data — every idea must make a real HTTP request.

---

## How It Works (All Editions)

Every edition runs three phases with two hard stops.

**Phase 1 — Idea Generation**
The AI generates 12–15 domain-specific project ideas, each with a structured format covering domain, difficulty, dependencies, visible result, smallest working version, scope risk, and domain-specific risk fields. After output, the AI stops completely and waits for your selection.

**Phase 2 — Stress Test**
You select which ideas to stress test. The AI runs all 15 evaluations on each: reality check, motivation collapse analysis, hidden complexity analysis, value analysis, momentum and feedback loop analysis, scope classification, force simplification, execution risk analysis, infrastructure complexity rule, ambition balancing rule, scoring, ranking, final decision (BUILD NOW / DELAY / DROP), execution plans for surviving ideas, and a quick-strike summary. After output, the AI stops completely.

**Phase 3 — Wrapped Prompt Generation**
You select a surviving idea. The AI generates a guided build prompt for that idea — a self-contained session starter that turns AI into an execution-focused pair-programming mentor, not a code generator. The wrapped prompt enforces guide-first coding: no implementation code until you attempt it or ask for it.

---

## Start Here — Core Edition

1. Open `framework/Idea_Generator.md`. Edit the domain list at the top to match your interests. Paste the entire file as a **user message** in a new AI chat session.
2. Pick the ideas that interest you from the generated list.
3. Open `framework/idea_evaluation_system.md`. Paste it as a **system prompt**. Send your idea list as the first user message.
4. Decide the idea you still want to build after evaluation.
5. Paste that idea into the same chat to wrap it as a guided build prompt, then start building.

---

## Start Here — Domain Editions (3D Games / Public API)

Domain editions are self-contained single files — all three phases are embedded.

1. Open the edition file for your domain.
2. Paste the **entire file** as a **user message** in a new AI chat session. No system prompt needed.
3. The AI runs Phase 1 and stops. Review the ideas.
4. Reply: `stress test ideas [numbers]` — e.g. `stress test ideas 2, 5, 9`
5. The AI runs Phase 2 and stops. Review the stress test results.
6. Reply: `wrap idea [number]` to generate a guided build prompt for a surviving idea.
7. Start building in a new session using the wrapped prompt.

---

## What the Framework Actively Suppresses

- premature optimization
- architecture-heavy planning before anything runs
- plugin-system and framework escalation
- solving future problems before the first working version exists
- invisible progress — ideas that become interesting only after massive setup
- motivation collapse from scope that grows faster than output

---

## Design Priorities

Completion over sophistication.
Visible progress over elegant architecture.
Hands-on learning over passive code generation.

Ideas are evaluated on execution realism: setup friction, visible progress speed, debugging complexity, iteration quality, and completion likelihood — not theoretical sophistication.

---

## Who This Is For

- solo developers trying to finish projects
- beginners overwhelmed by AI-generated complexity
- AI-assisted builders using ChatGPT or Claude
- makers who want practical iteration instead of endless planning
- programmers learning through guided construction

---

## Repository Structure

```
framework/
    Idea_Generator.md                            ← Core edition: domain-configurable idea generator
    idea_evaluation_system.md                    ← Core edition: evaluation system (use as system prompt)
    Python3d-games-idea-gener-n-tester.md        ← 3D Python Games edition (self-contained, single file)
    Free-Public-API-n-Python-idea-gener-n-tester.md  ← Public API edition (self-contained, single file)

examples/
    example_input_ideas.md
    example_output_evaluation.md
    generated_wrapped_prompt_example.md
```

---

## Example Workflow

1. Submit multiple project ideas (or generate them with Phase 1)
2. Framework stress-tests each idea across 15 evaluation points
3. Ideas are ranked by execution realism
4. High-risk ideas are simplified or rejected
5. Viable ideas are converted into guided build prompts
6. AI guides implementation incrementally
7. You build through small, visible feedback loops

---

## Important Note

This project is not intended to replace software engineering judgment.

It is a structured workflow framework designed to improve execution discipline, incremental learning, project survivability, and AI-assisted implementation behavior.

The long-term goal is to explore healthier, more sustainable forms of AI-assisted software development — ones that prioritize learning, execution, and finished projects over raw generation capability.

---

## About

Execution-focused AI framework for realistic project evaluation, incremental building, and hands-on learning guidance.

MIT License — see LICENSE file.

Built by [MainbyteLabs](https://github.com/MR-MainbyteLabs)
