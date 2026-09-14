# Migration record

Date: 2026-09-14

This repository was split out of `c3right/notepad` when the work evolved from a set of research notes into a standalone project with its own methodology, candidate pipeline, case workspaces, templates and packet prototypes.

## Source-of-truth change

From this migration forward:

> **`c3right/history-case-lab` is the sole source of truth for this project.**

The older `notepad` copies are historical snapshots only. Future agents and contributors should not read `notepad` in order to recover project state unless explicitly doing provenance research.

## Core artifacts copied into this repository

The following project artifacts were copied into `docs/`:

1. `2026-09-14-history-life-simulation-roadmap.md`
2. `2026-09-14-history-decision-atom-schema-v1.md`
3. `2026-09-14-history-decision-atom-scoring-v1.md`
4. `2026-09-14-history-decision-atom-ranking-experiment-1.md`
5. `2026-09-14-history-decision-atom-qualification-sprint-1.md`
6. `2026-09-14-history-case-packet-feasibility-mini-design-1.md`
7. `2026-09-14-history-case-packet-starkloff-v0.1.md`

These preserve the complete active project state that had been stored in `notepad`.

## Cross-repository links removed as operational dependencies

The Decision Atom schema referenced two separate macro-history reading-framework notes. Those are conceptually related but not required to operate this project. Local context stubs were added under `docs/` so the repository remains self-contained.

## New standalone project structure added here

- `AGENTS.md` — project rules
- `cases/` — case workspaces
- `templates/` — reusable research / qualification / packet / test templates
- `data/candidates.yaml` — current candidate registry
- `docs/INDEX.md` — local document index

## Next migration principle

Do not mirror ongoing edits back into `notepad`. Avoid dual maintenance. If an old `notepad` note contains useful project material that was missed, copy it here once, record the migration, and continue only here.
