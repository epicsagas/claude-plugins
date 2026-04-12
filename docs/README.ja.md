# epicsagas プラグイン

> 本格的なAI支援開発のための手作りプラグイン — 自律エージェント、コンテキスト圧縮、邪魔にならないツール群。

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](../LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-2-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**翻訳:** [English](../README.md) · [한국어](README.ko.md) · [简体中文](README.zh-cn.md) · [繁體中文](README.zh-tw.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [Русский](README.ru.md) · [العربية](README.ar.md)

---

## プラグイン一覧

| プラグイン | 説明 | ソース |
|-----------|------|--------|
| [epic](#epic) | 自律エージェントハーネス — 6つのパワーコマンド、自己進化スキル、毎セッション動作する不可視フック | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | トークン最適化ドキュメントリーダー — `.md`、`.html`、`.txt`ファイルを自動圧縮し、コンテキスト使用量を最大40%削減 | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |

---

## インストール

Claude Codeにこのマーケットプレイスを追加:

```bash
claude plugin add epicsagas
```

個別プラグインのインストール:

```bash
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
```

---

## プラグイン詳細

### epic

**自律エージェントハーネス**

複雑なマルチステップタスクを独立して処理するエージェントワークフローを構築します。6つの組み込みパワーコマンドを備え、スキルは使用するほど自己進化します。セッションフックが自動実行され、コードを保護し、出力を洗練し、各セッションを振り返ります。

**使用場面:**
- コードレビュー、コミット、テストサイクルの繰り返し自動化
- プロジェクト固有のカスタムワークフロー定義
- Claudeセッション全体での一貫した動作パターンの適用

**主な機能:**
- 6つの組み込みパワーコマンド（commit、review、test、deployなど）
- 自己進化スキルシステム — 使用パターンを学習して継続的に改善
- セッションガードフック — ミスを防ぎ品質を自動維持

→ [ソース & ドキュメント](https://github.com/epicsagas/epic-harness)

---

### transpile

**トークン最適化ドキュメントリーダー**

Readツール呼び出し時に`.md`、`.html`、`.txt`ファイルを自動圧縮し、コンテキストトークン使用量を最大40%削減します。ワークフローの変更なしに即効果が現れます。

**使用場面:**
- 大規模ドキュメントや仕様書を頻繁に参照するプロジェクト
- コンテキストウィンドウの上限に頻繁に達する場合
- 長いセッションでのトークンコスト削減

**主な機能:**
- サイレント圧縮 — 同じ出力、最大40%少ないトークン
- `.md` / `.html` / `.txt`フォーマットの自動検出
- 既存のReadツールワークフローと完全互換

→ [ソース & ドキュメント](https://github.com/epicsagas/llm-transpile)

---

## コントリビューション

プラグインの提出や改善提案:

1. このリポジトリをフォーク
2. `.claude-plugin/marketplace.json`にプラグイン情報を追加
3. Pull Requestを作成

プラグインは独立したGitHubリポジトリで管理され、マーケットプレイスはメタデータのみを含みます。

---

## ライセンス

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
