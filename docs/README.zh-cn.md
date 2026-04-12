# epicsagas 插件

> 专为 AI 辅助开发精心打造的插件 — 自主代理、上下文压缩，以及不会干扰您工作流的工具。

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](../LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-2-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**翻译：** [English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [繁體中文](README.zh-tw.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [Русский](README.ru.md) · [العربية](README.ar.md)

---

## 插件列表

| 插件 | 描述 | 源码 |
|------|------|------|
| [epic](#epic) | 自主代理框架 — 6 个强力命令、自我进化的技能，以及每个会话自动运行的隐形钩子 | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | 令牌优化文档阅读器 — 静默压缩 `.md`、`.html`、`.txt` 文件，上下文用量最多减少 40% | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |

---

## 安装

在 Claude Code 中添加此市场：

```bash
claude plugin add epicsagas
```

安装单个插件：

```bash
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
```

---

## 插件详情

### epic

**自主代理框架**

构建能够独立处理复杂多步任务的代理工作流。内置 6 个强力命令，技能随使用而自我进化。会话钩子自动运行，守护代码、优化输出并反思每次会话。

**适用场景：**
- 自动化重复性代码审查、提交和测试周期
- 定义项目专属的自定义工作流
- 跨 Claude 会话执行一致的行为模式

**核心功能：**
- 6 个内置强力命令（commit、review、test、deploy 等）
- 自我进化技能系统 — 从使用模式中学习并持续改进
- 会话守护钩子 — 自动防止错误并维持质量

→ [源码与文档](https://github.com/epicsagas/epic-harness)

---

### transpile

**令牌优化文档阅读器**

每次调用 Read 工具时自动压缩 `.md`、`.html`、`.txt` 文件，将上下文令牌用量最多减少 40%。无需修改工作流，立即生效。

**适用场景：**
- 频繁引用大型文档或规格说明的项目
- 经常触及上下文窗口限制时
- 希望降低长会话中的令牌成本

**核心功能：**
- 静默压缩 — 输出不变，令牌最多减少 40%
- 自动检测 `.md` / `.html` / `.txt` 格式
- 与现有 Read 工具工作流完全兼容

→ [源码与文档](https://github.com/epicsagas/llm-transpile)

---

## 贡献

提交插件或建议改进：

1. Fork 本仓库
2. 在 `.claude-plugin/marketplace.json` 中添加插件信息
3. 提交 Pull Request

插件以独立 GitHub 仓库形式维护，市场仅包含元数据。

---

## 许可证

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
