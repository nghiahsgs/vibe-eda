# vibe-eda

> Drag-and-drop PCB design in the browser — no coding needed.

A simple, visual EDA (Electronic Design Automation) tool: place and wire up
electronic components on a board by dragging blocks around, the way old-school
no-code / drag-and-drop builders let you compose things without writing code.

## Status

🌱 **Starter repo — prepared for the "From Idea to PR" workshop (Day 2).**

The actual build is intentionally left empty. It will be grown through the
`idea → spec → tickets → PR` flow (wayfinder → to-spec → to-tickets → implement)
during the workshop, one small slice at a time.

## The idea

- A web canvas where you **drag components** (resistor, capacitor, IC, connector…)
  onto a board.
- **Draw connections** (nets/traces) between component pins by dragging.
- Everything visual — **no code required** to lay out a simple board.

## v1 scope (keep it small)

**In:**
- A board canvas.
- Drag a single component from a palette onto the canvas and move it around.

**Out (later slices):**
- Wiring / net routing
- Design-rule checks (DRC)
- Gerber / netlist export
- Component library / footprints

## First slice (the smallest thing to build first)

> Show an empty board canvas + a palette with one component, and let the user
> drag that component onto the canvas and reposition it.

## Getting started

_To be defined during the workshop (stack not locked in yet — see `AGENTS.md`)._
