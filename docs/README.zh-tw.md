# epicsagas 插件

> 專為 AI 輔助開發精心打造的插件 — 自主代理、上下文壓縮，以及不會干擾您工作流程的工具。

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](../LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-2-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**翻譯：** [English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-cn.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [Русский](README.ru.md) · [العربية](README.ar.md)

---

## 插件列表

| 插件 | 描述 | 原始碼 |
|------|------|--------|
| [epic](#epic) | 自主代理框架 — 6 個強力指令、自我進化的技能，以及每個工作階段自動執行的隱形鉤子 | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | 令牌最佳化文件閱讀器 — 靜默壓縮 `.md`、`.html`、`.txt` 檔案，上下文用量最多減少 40% | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |

---

## 安裝

在 Claude Code 中新增此市場：

```bash
claude plugin add epicsagas
```

安裝個別插件：

```bash
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
```

---

## 插件詳情

### epic

**自主代理框架**

建構能夠獨立處理複雜多步驟任務的代理工作流程。內建 6 個強力指令，技能隨使用而自我進化。工作階段鉤子自動執行，守護程式碼、最佳化輸出並反思每次工作階段。

**適用場景：**
- 自動化重複性程式碼審查、提交和測試週期
- 定義專案專屬的自訂工作流程
- 跨 Claude 工作階段執行一致的行為模式

**核心功能：**
- 6 個內建強力指令（commit、review、test、deploy 等）
- 自我進化技能系統 — 從使用模式中學習並持續改進
- 工作階段守護鉤子 — 自動防止錯誤並維持品質

→ [原始碼與文件](https://github.com/epicsagas/epic-harness)

---

### transpile

**令牌最佳化文件閱讀器**

每次呼叫 Read 工具時自動壓縮 `.md`、`.html`、`.txt` 檔案，將上下文令牌用量最多減少 40%。無需修改工作流程，立即生效。

**適用場景：**
- 頻繁參照大型文件或規格說明的專案
- 經常觸及上下文視窗限制時
- 希望降低長工作階段中的令牌成本

**核心功能：**
- 靜默壓縮 — 輸出不變，令牌最多減少 40%
- 自動偵測 `.md` / `.html` / `.txt` 格式
- 與現有 Read 工具工作流程完全相容

→ [原始碼與文件](https://github.com/epicsagas/llm-transpile)

---

## 貢獻

提交插件或建議改進：

1. Fork 本儲存庫
2. 在 `.claude-plugin/marketplace.json` 中新增插件資訊
3. 提交 Pull Request

插件以獨立 GitHub 儲存庫形式維護，市場僅包含中繼資料。

---

## 授權條款

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
