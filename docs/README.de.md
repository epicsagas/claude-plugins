# epicsagas Plugins

> Handgefertigte Plugins für ernsthaftes KI-unterstütztes Entwickeln — autonome Agenten, Kontextkomprimierung und Werkzeuge, die nicht im Weg stehen.

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](../LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-2-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**Übersetzungen:** [English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-cn.md) · [繁體中文](README.zh-tw.md) · [Español](README.es.md) · [Français](README.fr.md) · [Português](README.pt.md) · [Русский](README.ru.md) · [العربية](README.ar.md)

---

## Plugins

| Plugin | Beschreibung | Quelle |
|--------|--------------|--------|
| [epic](#epic) | Autonomes Agenten-Harness — 6 leistungsstarke Befehle, selbstevolvierende Skills und unsichtbare Hooks, die jede Session schützen, verfeinern und reflektieren. | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | Token-optimierter Dokumentenleser — komprimiert `.md`-, `.html`- und `.txt`-Dateien lautlos und reduziert die Kontextnutzung um bis zu 40%. | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |

---

## Installation

### Über Claude Code (empfohlen)

Marketplace hinzufügen und dann Plugins installieren:

```bash
claude plugin add epicsagas
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
```

### epic — Eigenständige Installation

**Homebrew** (macOS):
```bash
brew install epicsagas/tap/epic-harness
```

**cargo-binstall** (vorkompiliertes Binary):
```bash
cargo binstall epic-harness
```

**Cargo** (aus Quellcode bauen):
```bash
cargo install epic-harness
```

### transpile — Eigenständige Installation

**cargo-binstall** (vorkompiliertes Binary):
```bash
cargo binstall llm-transpile
```

**Cargo** (aus Quellcode bauen):
```bash
cargo install llm-transpile
```

---

## Plugin-Details

### epic

**Autonomes Agenten-Harness**

Erstellen Sie Agenten-Workflows, die komplexe, mehrstufige Aufgaben selbstständig bewältigen. Ausgestattet mit 6 integrierten leistungsstarken Befehlen, entwickeln sich Skills mit der Nutzung weiter. Session-Hooks laufen automatisch, um Ihren Code zu schützen, die Ausgabe zu verfeinern und jede Session zu reflektieren.

**Wann verwenden:**
- Automatisierung wiederkehrender Code-Review-, Commit- und Testzyklen
- Definition projektspezifischer benutzerdefinierter Workflows
- Durchsetzung konsistenter Verhaltensmuster in Claude-Sessions

**Hauptfunktionen:**
- 6 integrierte leistungsstarke Befehle (commit, review, test, deploy und mehr)
- Selbstevolvierendes Skill-System — lernt aus Nutzungsmustern und verbessert sich kontinuierlich
- Session-Guard-Hooks — verhindert Fehler und erhält Qualität automatisch

→ [Quelle & Dokumentation](https://github.com/epicsagas/epic-harness)

---

### transpile

**Token-Optimierter Dokumentenleser**

Komprimiert automatisch `.md`-, `.html`- und `.txt`-Dateien bei jedem Read-Tool-Aufruf und reduziert die Kontexttoken-Nutzung um bis zu 40%. Sofortige Wirkung ohne Workflow-Änderungen.

**Wann verwenden:**
- Projekte, die häufig große Dokumente oder Spezifikationen referenzieren
- Wenn Sie regelmäßig Kontextfenstergrenzen erreichen
- Zur Reduzierung von Tokenkosten in langen Sessions

**Hauptfunktionen:**
- Lautlose Komprimierung — gleiche Ausgabe, bis zu 40% weniger Token
- Erkennt automatisch `.md` / `.html` / `.txt`-Formate
- Vollständig kompatibel mit bestehenden Read-Tool-Workflows

→ [Quelle & Dokumentation](https://github.com/epicsagas/llm-transpile)

---

## Mitwirken

Plugin einreichen oder Verbesserungen vorschlagen:

1. Dieses Repository forken
2. Plugin-Eintrag in `.claude-plugin/marketplace.json` hinzufügen
3. Pull Request öffnen

Plugins werden als unabhängige GitHub-Repositories gepflegt. Dieser Marketplace enthält nur Metadaten.

---

## Lizenz

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
