# AGENTS.md — vibe-eda

Be extremely concise. Sacrifice grammar for concision.
At the end of each plan, list unresolved questions.

## WHAT

Browser-based, drag-and-drop PCB / EDA tool. Users place and wire electronic
components on a board visually — no code needed. Greenfield project.

## WHY

Make simple PCB layout approachable like an old no-code drag-drop builder.
Learning vehicle for the "From Idea to PR" workflow — grown one small slice at a time.

## HOW (proposed — NOT locked in)

- Frontend: React + TypeScript + Vite
- Canvas: SVG first (easy hit-testing / drag), consider Canvas2D if perf needs it
- State: keep it minimal (React state / Zustand) — no backend for v1
- Everything runs client-side; no server, no DB in v1

## Conventions

- Keep specs and slices small — small context = cheaper, fewer bugs.
- One slice = one branch = one PR.
- Let the linter/formatter own code style (don't hand-police it here).
- Write a test for each slice before calling it done.

## Workflows

- dev / test / build commands: _to be added once the stack is scaffolded._

## Progressive disclosure

- Architecture decisions → `docs/adr/` (add as decisions are made)
- Reusable know-how → `.agents/skills/<name>/SKILL.md`

## Unresolved questions

- SVG vs Canvas2D for the board surface?
- How are components/footprints modelled (data shape for a placed part)?
- Do we need persistence in v1 (localStorage), or purely in-memory?
- Grid + snapping in the first slice, or free positioning?
- Units / board coordinate system (mm vs mils vs px)?
