# Its Wrap Skill

[中文版](README.zh-CN.md) | English

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> Turn research into decisions. A Claude Code skill for researchers who need to communicate with product managers.

Convert research content into actionable decision assets to streamline the transition from theory to engineering. Now, go dump those materials on that ever-demanding PM!

## Quick Start

```bash
git clone https://github.com/Gh0se4/its-wrap-skill.git
cp -r its-wrap-skill/.skill ~/.claude/skills/its-wrap
```

Then in Claude Code: *"I have a research demo. Help me turn it into a product decision package."*

## What It Is

Its Wrap bridges the gap between **research done** and **product decision made**.

Researchers often have working demos, prototypes, or experiments that show promise—but translating that work into something a product manager can evaluate and act on is hard.

This skill structures that translation.

## When to Use It

| You have... | Use Its Wrap when... |
|-------------|---------------------|
| A working demo | You need to frame it for PM evaluation |
| Vibe-coded prototype | You want to identify what's production-ready vs. throwaway |
| LLM/AI experiment | You need to structure evidence and validation plan |
| Algorithm improvement | You want to map technical gains to user value |
| Research notes | You need to organize them into a decision package |

## What It Produces

A structured handoff package covering:

1. **Executive Summary** — Quick decision recommendation
2. **Problem & User Scenario** — Why this matters
3. **Research Asset** — What exists now
4. **Productized Solution** — What it could become
5. **Decision Evidence** — What's proven vs. assumed
6. **Non-Quantitative Value** — Strategic/experience value
7. **Alternatives** — Simpler options considered
8. **Execution Path** — How to get from here to shipped
9. **Cost Model** — Development and operational costs
10. **Risks & Boundaries** — What could go wrong
11. **Data Loop** — How to measure and improve
12. **Missing Information** — Known gaps to fill
13. **Next Actions** — Concrete recommended steps

## Installation

See [INSTALL.md](INSTALL.md) for detailed instructions.

### Quick Install

```bash
# Clone the repository
git clone https://github.com/Gh0se4/its-wrap-skill.git

# Install for Claude Code
mkdir -p ~/.claude/skills
cp -r its-wrap-skill/.skill ~/.claude/skills/its-wrap

# Restart Claude Code
```

## Usage

See [USAGE.md](USAGE.md) for detailed examples and workflows.

### Basic Usage

Describe your research and ask for a product decision handoff:

```
"I built an LLM demo that categorizes support tickets.
It works on 200 historical tickets. Help me turn this into
something my PM can use to decide next steps."
```

Claude will invoke Its Wrap and produce a structured handoff package.

### Handling Missing Information

If critical information is missing, Its Wrap will ask clarifying questions:

- "Who is the target user?"
- "What problem does this solve?"
- "Do you have any baseline metrics?"

Answer these to improve the output, or continue with gaps marked as `TBD`.

## Key Features

### 🎯 Decision-Focused

Every output element serves a product decision. No fluff, no generic summaries.

### 🔍 Gap Detection

Automatically identifies missing information that would affect the decision.

### 🛠️ Vibe-Coding Aware

Special handling for vibe-coded prototypes—distinguishing demo-quality from production-ready.

### 🤖 AI/LLM Ready

Includes specific checks for AI research: prompt structures, evaluation criteria, cost models, and safety considerations.

### ⚖️ Balanced

Always presents alternatives and tradeoffs, not just the "build it" case.

## Documentation

| File | Description |
|------|-------------|
| [README.md](README.md) | This file — overview and introduction |
| [README.zh-CN.md](README.zh-CN.md) | 中文说明 |
| [INSTALL.md](INSTALL.md) | Detailed installation instructions |
| [USAGE.md](USAGE.md) | Usage examples and workflows |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute |
| [.skill/SKILL.md](.skill/SKILL.md) | Full skill specification |

## Philosophy

Its Wrap follows these principles:

1. **Researcher-First** — Serves researchers communicating with PMs
2. **Decision-Support** — Prepares materials, doesn't make decisions
3. **Honest About Gaps** — Always surfaces missing information
4. **Flexible Structure** — Adapts to input complexity while maintaining rigor

## Contributing

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

MIT License — see [LICENSE](LICENSE) for details.

## Related

- [Claude Code](https://claude.ai/code) — The AI coding assistant that uses this skill
- [Agent Skills Specification](https://agentskills.io) — Standard for agent skills

---

**Made with ❤️ for researchers who want their work to ship.**
