# Vibe Coding Scaffolding

A reusable folder and Markdown scaffolding for **conscious AI-assisted development** — the operational structure described in the *Vibe Coding Consapevole — CAP 2* method.

The goal is to give any LLM-based coding agent (Claude, GPT, Gemini, …) the context, constraints, and memory it needs to work as a precise executor instead of a fast guesser, while keeping a clean separation between projects.

## Why this exists

LLMs do their best work when:

1. They know **what** they are building (goal and requirements).
2. They know **where** to put files (directory map).
3. They know **how** to build it (tech stack and constraints).
4. They have a **memory** that survives across sessions and across model switches.

This scaffolding encodes those four needs as a small set of Markdown files. Markdown is used deliberately — its heading hierarchy carries strong semantic meaning and is equally readable by humans and machines.

## Repository layout

```
.
├── agents.md              # Repository-level safeguards (no destructive action without consent)
├── projects/
│   ├── agents.md          # Safeguards specific to the projects area
│   └── <ProjectName>/     # One self-contained project per folder
│       ├── planning/
│       │   ├── plan.md            # Operational contract: what / where / how
│       │   ├── implementations.md # Architectural decisions log
│       │   ├── backlog.md         # Out-of-scope ideas
│       │   └── devlog.md          # Version-by-version development log
│       ├── code/          # Application source code
│       ├── manuals/       # User-facing documentation
│       ├── input/         # Raw files to be processed
│       └── output/        # Final results produced by the system
```

## The four planning files

| File | Role |
|---|---|
| `plan.md` | The **operational contract** between human and AI. Goal, requirements, directory map, tech stack, constraints, and the implementation plan the AI fills in for human validation. |
| `implementations.md` | Technical notebook. Every non-trivial architectural decision is recorded with date, rationale, and files involved. |
| `backlog.md` | Storage for ideas that fall outside the current scope, so the dialogue with the AI does not drift. |
| `devlog.md` | Version-by-version log of substantial changes. The single document a new agent (or a new model) reads to restore context. |

## How to use this scaffolding

1. Clone the repository (or copy the structure into your own).
2. Duplicate `projects/Project1/` and rename the copy to your project name.
3. Open `planning/plan.md` and fill in sections **1**, **2**, **3** (the human-owned parts).
4. Ask your AI agent to read `agents.md` and `planning/plan.md`, then to expand section **4** (Implementation plan) and ask any open questions.
5. Validate the plan with the AI **before** any code is written.
6. As you work, keep the four planning files alive — the AI should update `implementations.md`, `backlog.md`, and `devlog.md` as it goes.

## Safeguards

The two `agents.md` files at the root and inside `projects/` are not documentation — they are **rules** for any AI agent working in this tree. They forbid destructive or irreversible actions (delete, rename, move, force-push, history rewrite) without explicit user confirmation. Subfolders may add stricter rules but never weaken these.

## Credits

Method inspired by *Vibe Coding Consapevole — CAP 2*. Scaffolding maintained by [Search Foundry](https://github.com/Search-Foundry).
