# IMPORTANT — Repository-level safeguards

This file lives at the root of the repository. Any AI agent working in this tree **must** read it before acting.

It exists to prevent accidental destructive actions across the whole workspace.

## Hard rules

Never perform these actions without explicit user confirmation:

- Deleting a file or folder
- Renaming a file or folder
- Moving a file or folder out of its current location
- Overwriting a file with unrelated content
- Force-pushing, resetting, or rewriting git history
- Any other potentially destructive or irreversible operation

When in doubt: **ASK**.

## Scope

- This file applies to the whole repository.
- Each project lives under `projects/<ProjectName>/` and has its own operational documents (`planning/plan.md`, `planning/implementations.md`, `planning/backlog.md`, `planning/devlog.md`).
- Subfolders may define additional rules that **add to** — never weaken — the rules in this file.

## Repository layout

```
.
├── agents.md           # This file — repository-level safeguards
└── projects/           # One subfolder per project
    ├── agents.md       # Safeguards specific to the projects area
    └── <ProjectName>/  # Self-contained project (planning, code, manuals, input, output)
```
