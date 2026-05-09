# <Project Name>

> **Operational contract** between human and AI. The human provides context and constraints; the AI fills in technical detail. Validate the path here, before writing a single line of code.

**Status:** `Not started` | `In progress` | `Blocked` | `Completed`
**Last updated:** YYYY-MM-DD
**Owner:** <name / email>

---

## 1. Functional description — the "What"

### Main goal

One sentence that states the outcome you want.
_e.g. "I want an automation that pulls data from GA4 and produces a weekly Excel report."_

### Specific requirements

- [ ] Requirement 1
- [ ] Requirement 2
- [ ] Requirement 3

### Out of scope

What this project explicitly will **not** do (move proposals to `backlog.md`).

-

### Success criteria

How we know we are done.

-

---

## 2. Architecture and structure — the "Where"

### Directory map

Describe what each folder contains. Prevents the AI from creating files in the wrong place.

```
.
├── agents.md           # General behavioral rules — read first
├── planning/           # Operational documents — read and keep updated
│   ├── plan.md         # This file: operational contract
│   ├── implementations.md  # Architectural decisions log
│   ├── backlog.md      # Out-of-scope ideas
│   └── devlog.md       # Version-by-version development log
├── code/               # Application source code
├── manuals/            # User-facing documentation
├── input/              # Raw files to be processed
└── output/             # Final results produced by the system
```

### Key control files

The AI **must** read and update these files during work:

| File | Purpose | When to update |
|---|---|---|
| `planning/plan.md` | Operational contract | Whenever scope, stack, or status changes |
| `planning/implementations.md` | Architectural decisions | Every non-trivial technical choice |
| `planning/backlog.md` | Out-of-scope ideas | Whenever an idea emerges that does not fit the current scope |
| `planning/devlog.md` | Version-by-version log | After every substantial change |

---

## 3. Tech stack and constraints — the "How"

### Languages and libraries

- Language:
- Frameworks:
- Key libraries:
- Package manager:

### Execution environment

- Runs on: `local` | `container (Docker)` | `server` | `serverless` | `CI`
- OS / runtime version:
- Required environment variables / secrets:

### External services and APIs

- Service 1 — purpose, auth method (e.g. OAuth, API key)
- Service 2 — …

### Constraints and conventions

- Coding style / linter:
- Testing strategy:
- Logging / observability:
- Other limits (rate limits, file size, latency, etc.):

---

## 4. Implementation plan (filled in by the AI)

> The AI expands this section after reading the file. The human validates before any code is written.

### Authentication / access

_(e.g. OAuth flow for Google APIs, token storage strategy)_

### Data model / file structure

_(e.g. Excel sheet layout, JSON schema, table definitions)_

### Operational tasks

- [ ] Task 1 —
- [ ] Task 2 —
- [ ] Task 3 —

### Error handling and retries

_(e.g. "if the API does not respond, retry 3 times with exponential backoff; on permanent failure, log to `output/errors.log` and exit non-zero")_

### Open questions for the human

-

---

## 5. Status and history

### Short-term goals

- [ ]

### Long-term goals

- [ ]

### Recent milestones

_(see `devlog.md` for the full history)_

-
