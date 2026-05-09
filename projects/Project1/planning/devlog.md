# Development Log (Devlog)

Log of substantial changes, version after version. Useful for humans and for restoring context when switching AI model (e.g. Claude ↔ GPT).

Suggested format:

```
## vX.Y.Z — YYYY-MM-DD
**Main changes:**
- ...
**Rationale:**
**Impact:**
**Notes for next session:**
```

---

## v0.1.0 — 2026-05-09
**Main changes:**
- Initialized the "Vibe Coding Consapevole" structure.
- Created folders: `planning/`, `code/`, `manuals/`, `input/`, `output/`.
- Created planning files: `plan.md`, `implementations.md`, `backlog.md`, `devlog.md`.
- Created `agents.md` with general behavioral instructions.

**Rationale:** establish the operational baseline described in CAP 2 of the course.

## v0.2.0 — 2026-05-09
**Main changes:**
- Translated the entire structure to English (folders, filenames, and file contents).
- `pianificazione/` → `planning/`, `codice/` → `code/`, `manuali/` → `manuals/`.
- `implementazioni.md` → `implementations.md`, `blog.md` → `devlog.md`.

**Rationale:** make the structure international and easier to share.

**Impact:** any external reference to the previous Italian paths must be updated.

## v0.3.0 — 2026-05-09
**Main changes:**
- Moved `planning/`, `code/`, `manuals/`, `input/`, `output/` under `projects/Project1/`.
- Repository root now contains only `agents.md` (deletion safeguards) and `projects/`.

**Rationale:** these folders are per-project, not repository-wide. Hosting them at the root would mix multiple projects in the same namespace.

**Impact:** all paths in `plan.md` are relative to the project root (`projects/Project1/`).
