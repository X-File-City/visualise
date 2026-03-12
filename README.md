# visualise

An [Agent Skill](https://agentskills.io) for rendering inline interactive visuals — SVG diagrams, HTML widgets, charts, and explainers — directly in agent conversations.

## What it does

When activated, the agent can generate rich visual content that renders in a sandboxed iframe alongside conversation text. Two output modes:

- **SVG mode** — static diagrams (flowcharts, architecture, illustrative)
- **HTML mode** — interactive content (sliders, controls, charts, steppers)

## When it triggers

Requests containing: visualize, diagram, chart, illustrate, draw, map out, show me, explain (spatial concepts), compare (side-by-side).

## Install

```bash
# Claude Code
claude mcp add-skill /path/to/visualise

# Or copy to your skills directory
cp -r visualise/ ~/.skills/visualise
```

## Structure

```
visualise/
├── SKILL.md                          # Skill metadata + instructions
└── references/
    ├── design-system.md              # CSS variables, color ramps, typography
    ├── components.md                 # Interactive explainers, comparisons, cards
    ├── diagrams.md                   # Flowcharts, structural, illustrative
    ├── charts.md                     # Chart.js, data viz
    └── client-implementation.md      # Iframe sandbox details
```

## License

MIT
