# Guided Build Framework

Execution-focused AI framework for realistic project evaluation, incremental building, and hands-on learning guidance.

---

## What It Does

Most AI-assisted projects fail the same way — they expand too fast, become too abstract, and stop producing visible progress. The AI encourages complexity, the architecture grows, and momentum collapses before anything ships.

This framework treats AI as an execution-focused pair-programming mentor, not a code generator.

It stress-tests project ideas, exposes hidden complexity, detects motivation-collapse points, and ranks ideas by completion likelihood. Viable ideas get converted into guided build prompts that walk you through implementation incrementally — small steps, test-and-confirm loops, active construction by you.

What it actively suppresses:
- premature optimization
- architecture-heavy planning
- scope creep
- solving future problems before they exist

---

## How It Works

One file. Three phases. Two hard stops.

```
Phase 1 → Generates 12–15 project ideas → HARD STOP
Phase 2 → Stress-tests only the ideas you select → HARD STOP
Phase 3 → Generates a guided build prompt for ideas you choose to wrap
```

The hard stops are enforced by the framework itself. The AI will not proceed to the next phase until you send your selection.

---

## Start Here

**Step 1 — Customize**

Open `guided-build-framework.md`. Find the domain list near the top of Phase 1:

```
- system monitoring
- automation engines
- Linux infrastructure tooling
- serial/UART communication
- log analysis
- CLI wrappers
```

Replace it with your own areas of interest. The rest of the file does not need to change.

**Step 2 — Generate ideas**

Paste the entire file as a **user message** in a new AI chat session. Phase 1 runs and produces 12–15 project ideas, then stops and waits.

**Step 3 — Select ideas to stress test**

Review the ideas. Reply with:

```
stress test ideas 2, 5, 7
```

Phase 2 runs a full evaluation on only the ideas you selected, then stops and waits.

**Step 4 — Wrap a surviving idea**

Review the stress test results. If you want a guided build prompt for a surviving idea, reply with:

```
wrap idea 5
```

Phase 3 generates a guided build session prompt for that idea. Paste it as a user message in a new session to start building.

---

## Who This Is For

- solo developers trying to finish projects
- AI-assisted builders using ChatGPT or Claude
- beginners overwhelmed by AI-generated complexity
- makers who want practical iteration instead of endless planning
- programmers who learn by building, not by reading code dumps

---

## Design Priorities

Completion over sophistication.  
Visible progress over elegant architecture.  
Hands-on learning over passive code generation.

The framework frames the user as the builder and the AI as the guide. That role distinction changes how implementation sessions behave — it keeps you in the loop instead of watching AI write code you don't understand.

Ideas are evaluated on execution realism: setup friction, visible progress speed, debugging complexity, iteration quality, and completion likelihood. Not theoretical sophistication.

---

## Repository Structure

```
guided-build-framework.md         ← the entire framework — paste this
guided-build-framework-modification-guide.md   ← how to adapt it
```

---

## Current Status

The framework is actively evolving through prompt iteration, behavior testing, and implementation-session observation. It is experimental and intended as a practical exploration of human-AI workflow design.

---

## Important Note

This project is not intended to replace software engineering judgment. It is a structured workflow framework designed to improve execution discipline, incremental learning, project survivability, and AI-assisted implementation behavior.

---

*Built by MainbyteLabs — [github.com/MR-MainbyteLabs](https://github.com/MR-MainbyteLabs)*
