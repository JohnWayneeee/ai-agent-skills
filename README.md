# AI Agent Skills

A catalog of reusable AI agent skills by [@JohnWayneeee](https://github.com/JohnWayneeee).

Each skill is a self-contained instruction set for an AI agent — drop it into your Claude Code, Codex, or compatible agent runtime and invoke it by name.

## Skills

| Skill | Description |
|-------|-------------|
| [ui-final-polish](skills/ui-final-polish/) | Final visual polish for an existing UI without redesigning it |
| [react-flow-best-practices](skills/react-flow-best-practices/) | Best practices for `@xyflow/react` v12 canvases and custom nodes |
| [payoff-action-modeling](skills/payoff-action-modeling/) | Model post-outcome UI actions from user intent questions |
| [browser-audit](skills/browser-audit/) | Pre-deploy accessibility, SEO, and Lighthouse quality audit |
| [workflow-node-setup](skills/workflow-node-setup/) | Configure and debug React Flow workflow nodes |
| [pencil-to-code](skills/pencil-to-code/) | Convert Pencil `.pen` designs into production frontend code |

## Install

### Via Claude Code marketplace (recommended)

Add this repo as a marketplace source, then install individual skills:

```
/plugin marketplace add JohnWayneeee/ai-agent-skills
/plugin install ui-final-polish@ai-agent-skills
```

Replace `ui-final-polish` with any skill name from the table above.

### Manual — copy into your project

Copy a skill folder into your project's `.agents/skills/` directory:

```
your-project/
└── .agents/
    └── skills/
        └── ui-final-polish/
            └── SKILL.md
```

Or into your personal skills directory:

```
~/.claude/skills/ui-final-polish/
```

### Invoking a skill

```
Use $ui-final-polish to improve the spacing and hierarchy on this card component.
```

## Structure

Each skill follows a consistent layout:

```
skills/<skill-name>/
├── SKILL.md                  # Main skill entrypoint — start here
├── agents/
│   └── openai.yaml           # Optional: display name and default prompt
└── references/
    └── *.md                  # Optional: reference docs, checklists, criteria
```

The `marketplace.json` in the repo root enables `/plugin marketplace add` install flow.

## License

MIT — see [LICENSE](LICENSE).

---

> These skills were developed alongside [Casely](https://casely.digital/) — a hosted AI-powered workflow and QA tool. Check it out if you want the full product experience.
