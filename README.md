Guided Build Framework

Execution-focused AI framework for realistic project evaluation, incremental building, and hands-on learning guidance.

## Origins

This framework started with an AI-assisted idea generator prompt.

The idea generator helped produce project concepts, but it also revealed a problem: ideas are easy to generate, but finished builds require structure, scope, and discipline.

The Guided Build Framework exists to bridge that gap.

It turns raw project ideas into smaller, testable, buildable steps so that AI becomes a guide instead of a shortcut.

## Start Here Path

1. Open `framework/Idea_Generator.md`. Edit the domain list at the top to match your own interests. Then paste the entire file as a **user message** in a new AI chat session.
2. Pick all the ideas that interest you from the generated list.
3. Open `framework/idea_evaluation_system.md`. Paste it as a **system prompt** (Custom Instructions or System field). Then send your idea list as the first user message.
4. Decide the idea you still want to build after the evaluation.
5. Paste that idea into the same chat so it can be wrapped as a guided build prompt, then start building.

Using the Guided Build Framework:

1. Stress test the ideas
2. Reduce unnecessary complexity
3. Define the smallest useful MVP
4. Generate a guided implementation plan
5. Build incrementally with AI guidance

Result:
A smaller, finishable project with visible progress and hands-on learning.

Idea Generator → Idea List Evaluation → Simplify → Guided Build Prompt → Build Loop → MVP

## Who This Is For

- beginners overwhelmed by AI-generated complexity
- solo developers trying to finish projects
- AI-assisted builders using ChatGPT or Claude
- makers who want practical iteration instead of endless planning
- programmers learning through guided construction

## Overview

Most AI coding interactions drift toward:

- overengineering
- giant code dumps
- premature abstraction
- architecture-first thinking
- overwhelming project scope
- unfinished implementations

This project explores a different approach.

The Guided Build Framework is a structured AI interaction system designed to:

- evaluate project ideas realistically
- identify hidden complexity early
- reduce scope creep
- preserve visible progress
- encourage incremental implementation
- maintain hands-on learning
- improve project completion probability

Instead of treating AI as a "generate the whole project" tool, this framework treats AI as a:

execution-focused pair-programming mentor
## What It Does and Why

Most AI-assisted projects fail the same way — they expand too fast, 
become too abstract, and stop producing visible progress. The AI 
encourages complexity, the architecture grows, and momentum collapses 
before anything ships.

This framework treats AI as an execution-focused pair-programming mentor, 
not a code generator.

It stress-tests project ideas, exposes hidden complexity, detects 
motivation-collapse points, and ranks ideas by completion likelihood. 
Viable ideas get converted into guided build prompts that walk you through 
implementation incrementally — small steps, test-and-confirm loops, 
active construction by you.

What it actively suppresses:
- premature optimization
- architecture-heavy planning
- plugin-system escalation
- solving future problems before they exist

## Design Priorities

Completion over sophistication.
Visible progress over elegant architecture.
Hands-on learning over passive code generation.

The framework frames the user as the builder and the AI as the guide. 
That role distinction matters — it changes how implementation sessions 
behave over time and keeps you in the loop instead of watching AI write 
code you don't understand.

Ideas are evaluated on execution realism: setup friction, visible progress 
speed, debugging complexity, iteration quality, and completion likelihood. 
Not theoretical sophistication.


## Repository Structure

```text
framework/
    idea_evaluation_system.md
    Idea_Generator.md

examples/
    example_input_ideas.md
    example_output_evaluation.md
    generated_wrapped_prompt_example.md

```

## Example Workflow

1. Submit multiple project ideas
2. Framework stress-tests each idea
3. Ideas are ranked by execution realism
4. High-risk ideas are simplified or rejected
5. Viable ideas are converted into guided build prompts
6. AI guides implementation incrementally
7. User builds through small feedback loops

## Why I Built This?

While experimenting with AI coding tools, I noticed recurring problems:

- AI often encourages unnecessary complexity
- projects expand too quickly
- implementation becomes overwhelming
- users stop learning because AI does too much
- momentum collapses during large architectural phases

This project is an attempt to structure AI-assisted development around:

- constrained execution
- visible progress
- realistic scope
- sustainable iteration
- active participation

## Current Status

The framework is actively evolving through:

- prompt iteration
- behavior testing
- implementation-session observation
- ambiguity reduction
- role-framing refinement

The project is experimental and intended primarily as a practical exploration of human-AI workflow design.

## Important Note

This project is not intended to replace software engineering judgment.

It is a structured workflow framework designed to improve:

- execution discipline
- incremental learning
- project survivability
- AI-assisted implementation behavior

The long-term goal of this project is to explore healthier, more sustainable forms of AI-assisted software development that prioritize learning, execution, and finished projects over raw generation capability.
