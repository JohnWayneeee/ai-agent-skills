# AI Agent Skills

**Drop-in instruction sets that make your AI agent actually useful.**

A curated catalog of reusable skills by [@JohnWayneeee](https://github.com/JohnWayneeee) — each one a self-contained prompt you plug into Claude Code, Codex, or any compatible agent runtime and invoke by name.

No configuration. No boilerplate. Just pick a skill and go.

---

## Why Agent Skills?

Most AI agents know everything and do nothing well.

Skills fix that. Each one gives your agent a focused role, a clear process, and opinionated defaults — so instead of writing a 500-word prompt every time, you invoke a name and get expert-level output.

- **Consistent results** — same inputs, same quality, every time
- **Team-ready** — share a skill folder and everyone's agent behaves the same way
- **Composable** — chain skills together for multi-step workflows

---

## Skills

| Skill | What it does |
|-------|-------------|
| [ui-final-polish](skills/ui-final-polish/) | Tighten spacing, hierarchy, and visual rhythm on an existing UI — without redesigning it |
| [react-flow-best-practices](skills/react-flow-best-practices/) | Build `@xyflow/react` v12 canvases and custom nodes the right way |
| [payoff-action-modeling](skills/payoff-action-modeling/) | Model post-outcome UI actions from user intent — turns "what happens next?" into a decision tree |
| [browser-audit](skills/browser-audit/) | Pre-deploy accessibility, SEO, and Lighthouse audit with actionable findings |
| [workflow-node-setup](skills/workflow-node-setup/) | Configure and debug React Flow workflow nodes without the usual trial-and-error |
| [pencil-to-code](skills/pencil-to-code/) | Convert Pencil `.pen` wireframes into production-ready frontend code |

---

## Install

### Via Claude Code marketplace (recommended)

```bash
/plugin marketplace add JohnWayneeee/ai-agent-skills
/plugin install ui-final-polish@ai-agent-skills
```

Replace `ui-final-polish` with any skill name from the table above.

### Manual — copy into your project

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

### Invoke a skill

```
Use $ui-final-polish to improve the spacing and hierarchy on this card component.
```

---

## How Skills Are Structured

Every skill follows the same layout so you always know where to look:

```
skills/<skill-name>/
├── SKILL.md          # Start here — the full instruction set
├── agents/
│   └── openai.yaml   # Optional: display name and default prompt
└── references/
    └── *.md          # Optional: checklists, criteria, reference docs
```

The `marketplace.json` in the repo root enables the `/plugin marketplace add` install flow.

---

## Built alongside a real product

These skills were developed while building [Casely](https://casely.digital/) — an AI-powered workflow and QA tool. They are production-tested, not theoretical.

If you want the full product experience, [check it out](https://casely.digital/).

---

## License

MIT — see [LICENSE](LICENSE).
