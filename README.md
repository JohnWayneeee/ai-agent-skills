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

## Usage

### Claude Code / Claude Agent SDK

Copy a skill folder into your project's `.agents/skills/` directory:

```
your-project/
└── .agents/
    └── skills/
        └── ui-final-polish/
            └── SKILL.md
```

Then invoke it in your agent prompt:

```
Use $ui-final-polish to improve the spacing and hierarchy on this card component.
```

### Codex / other runtimes

Place the `SKILL.md` in your skill directory and reference it by name according to your runtime's conventions.

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

## License

MIT — see [LICENSE](LICENSE).

---

> These skills were developed alongside [Casely](https://casely.digital/) — a hosted AI-powered workflow and QA tool. Check it out if you want the full product experience.
