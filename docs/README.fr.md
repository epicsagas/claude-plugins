# epicsagas plugins

> Des plugins artisanaux pour le développement sérieux assisté par IA — agents autonomes, compression de contexte et outils qui ne perturbent pas votre flux de travail.

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](../LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-3-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**Traductions :** [English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-cn.md) · [繁體中文](README.zh-tw.md) · [Español](README.es.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [Русский](README.ru.md) · [العربية](README.ar.md)

---

## Plugins

| Plugin | Description | Source |
|--------|-------------|--------|
| [epic](#epic) | Harnais d'agent autonome — 6 commandes puissantes, compétences auto-évolutives et hooks invisibles qui protègent, peaufinent et analysent chaque session. | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | Lecteur de documents optimisé en tokens — compresse silencieusement les fichiers `.md`, `.html` et `.txt`, réduisant l'utilisation du contexte jusqu'à 40%. | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |
| [alcove](#alcove) | Serveur MCP de documentation — recherche hybride BM25+vectorielle, lint et gestion du cycle de vie launchd pour les documents de projet. | [epicsagas/alcove](https://github.com/epicsagas/alcove) |

---

## Installation

### Via Claude Code (recommandé)

Ajoutez le marketplace puis installez les plugins :

```bash
claude plugin add epicsagas
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
claude plugin install epicsagas/alcove
```

### epic — installation autonome

**Homebrew** (macOS) :
```bash
brew install epicsagas/tap/epic-harness
```

**cargo-binstall** (binaire précompilé) :
```bash
cargo binstall epic-harness
```

**Cargo** (compilation depuis les sources) :
```bash
cargo install epic-harness
```

### transpile — installation autonome

**cargo-binstall** (binaire précompilé) :
```bash
cargo binstall llm-transpile
```

**Cargo** (compilation depuis les sources) :
```bash
cargo install llm-transpile
```

### alcove — installation autonome

**Homebrew** (macOS) :
```bash
brew install epicsagas/tap/alcove
```

**cargo-binstall** (binaire précompilé) :
```bash
cargo binstall alcove
```

**Cargo** (compilation depuis les sources) :
```bash
cargo install alcove
```

---

## Détails des plugins

### epic

**Harnais d'Agent Autonome**

Construisez des workflows d'agents capables de gérer des tâches complexes et multi-étapes de manière indépendante. Équipé de 6 commandes puissantes intégrées, les compétences évoluent avec l'utilisation. Les hooks de session s'exécutent automatiquement pour protéger votre code, peaufiner la sortie et analyser chaque session.

**Quand l'utiliser :**
- Automatiser les cycles répétitifs de révision de code, commits et tests
- Définir des workflows personnalisés par projet
- Appliquer des patterns de comportement cohérents dans les sessions Claude

**Fonctionnalités principales :**
- 6 commandes puissantes intégrées (commit, review, test, deploy et plus)
- Système de compétences auto-évolutives — apprend des patterns d'utilisation et s'améliore continuellement
- Hooks de garde de session — prévient les erreurs et maintient la qualité automatiquement

→ [Source & Documentation](https://github.com/epicsagas/epic-harness)

---

### transpile

**Lecteur de Documents Optimisé en Tokens**

Compresse automatiquement les fichiers `.md`, `.html` et `.txt` à chaque appel de l'outil Read, réduisant l'utilisation des tokens de contexte jusqu'à 40%. Effet immédiat sans modification du flux de travail.

**Quand l'utiliser :**
- Projets référençant fréquemment de grands documents ou spécifications
- Lorsque vous atteignez régulièrement les limites de la fenêtre de contexte
- Pour réduire les coûts en tokens lors de longues sessions

**Fonctionnalités principales :**
- Compression silencieuse — même sortie, jusqu'à 40% moins de tokens
- Détecte automatiquement les formats `.md` / `.html` / `.txt`
- Entièrement compatible avec les workflows existants de l'outil Read

→ [Source & Documentation](https://github.com/epicsagas/llm-transpile)

---

### alcove

**Serveur MCP de Documentation**

Donne aux agents de codage IA un accès à la demande à vos documents de projet privés via MCP. Recherche hybride BM25+vectorielle, lint sémantique, validation de documents et serveur HTTP en arrière-plan avec mode proxy pour une réponse instantanée.

**Quand l'utiliser :**
- Gérer la documentation de projet privée à travers plusieurs agents IA
- Rechercher des décisions d'architecture, des PRD et des runbooks depuis tout agent compatible MCP
- Appliquer des normes de documentation avec validation de politiques et lint sémantique

**Fonctionnalités principales :**
- Recherche hybride — BM25 + similarité vectorielle avec Reciprocal Rank Fusion
- Un doc-repo, tout agent — Claude Code, Cursor, Gemini CLI, Codex et plus de 5 autres
- Serveur en arrière-plan avec mode proxy — élimine la latence de démarrage à froid pour les nouvelles sessions
- Lint sémantique — liens cassés, fichiers orphelins, marqueurs obsolètes, dates périmées
- Intégration macOS launchd — commandes de cycle de vie enable/disable/start/stop/restart

→ [Source & Documentation](https://github.com/epicsagas/alcove)

---

## Contribuer

Pour soumettre un plugin ou suggérer des améliorations :

1. Forkez ce dépôt
2. Ajoutez votre entrée de plugin dans `.claude-plugin/marketplace.json`
3. Ouvrez une Pull Request

Les plugins sont maintenus comme des dépôts GitHub indépendants. Ce marketplace contient uniquement des métadonnées.

---

## Licence

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
