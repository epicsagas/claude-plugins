# epicsagas plugins

> Handcrafted plugins for serious AI-assisted development — autonomous agents, context compression, and tools that get out of your way.

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-2-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**Translations:** [한국어](docs/README.ko.md) · [日本語](docs/README.ja.md) · [简体中文](docs/README.zh-cn.md) · [繁體中文](docs/README.zh-tw.md) · [Español](docs/README.es.md) · [Français](docs/README.fr.md) · [Deutsch](docs/README.de.md) · [Português](docs/README.pt.md) · [Русский](docs/README.ru.md) · [العربية](docs/README.ar.md)

---

## Plugins

| Plugin | Description | Source |
|--------|-------------|--------|
| [epic](#epic) | Autonomous agent harness — 6 power commands, self-evolving skills, and invisible hooks that guard, polish, and reflect on every session. | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | Token-optimized document reader — silently compresses `.md`, `.html`, and `.txt` files on Read, cutting context usage by up to 40%. | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |

---

## Installation

Add this marketplace to Claude Code:

```bash
claude plugin add epicsagas
```

Install individual plugins:

```bash
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
```

---

## Plugin Details

### epic

**Autonomous Agent Harness**

Build agent workflows that handle complex, multi-step tasks independently. Powered by 6 built-in power commands, skills evolve the more you use them. Session hooks run automatically to guard your code, polish output, and reflect on each session.

**When to use:**
- Automating repetitive code review, commit, and test cycles
- Defining custom per-project workflows
- Enforcing consistent behavior patterns across Claude sessions

**Key features:**
- 6 built-in power commands (commit, review, test, deploy, and more)
- Self-evolving skill system — learns from usage patterns and improves over time
- Session guard hooks — prevents mistakes and maintains quality automatically

→ [Source & Docs](https://github.com/epicsagas/epic-harness)

---

### transpile

**Token-Optimized Document Reader**

Automatically compresses `.md`, `.html`, and `.txt` files on every Read tool call, cutting context token usage by up to 40%. Takes effect immediately with no workflow changes required.

**When to use:**
- Projects that frequently reference large documents or specs
- When you regularly hit context window limits
- Reducing token costs across long sessions

**Key features:**
- Silent compression — same output, up to 40% fewer tokens
- Auto-detects `.md` / `.html` / `.txt` formats
- Fully compatible with existing Read tool workflows

→ [Source & Docs](https://github.com/epicsagas/llm-transpile)

---

## Contributing

To submit a plugin or suggest improvements:

1. Fork this repository
2. Add your plugin entry to `.claude-plugin/marketplace.json`
3. Open a Pull Request

Plugins are maintained as independent GitHub repositories. This marketplace contains metadata only.

---

## License

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
