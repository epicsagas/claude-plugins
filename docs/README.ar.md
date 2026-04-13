# إضافات epicsagas

> إضافات مصنوعة بعناية للتطوير الجاد المدعوم بالذكاء الاصطناعي — وكلاء مستقلون، ضغط السياق، وأدوات لا تعترض مسيرتك.

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](../LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-3-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**الترجمات:** [English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-cn.md) · [繁體中文](README.zh-tw.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [Русский](README.ru.md)

---

## الإضافات

| الإضافة | الوصف | المصدر |
|---------|-------|--------|
| [epic](#epic) | إطار عمل وكيل مستقل — 6 أوامر قوية، مهارات تتطور ذاتياً، وخطافات خفية تحمي وتُحسّن وتُراجع كل جلسة. | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | قارئ مستندات مُحسَّن للرموز — يضغط ملفات `.md` و`.html` و`.txt` بصمت، مما يقلل استخدام السياق بنسبة تصل إلى 40%. | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |
| [alcove](#alcove) | خادم MCP للتوثيق — بحث هجين BM25+متجهي، فحص الجودة وإدارة دورة حياة launchd لمستندات المشروع. | [epicsagas/alcove](https://github.com/epicsagas/alcove) |

---

## التثبيت

### عبر Claude Code (مُوصى به)

أضف السوق ثم ثبّت الإضافات:

```bash
claude plugin add epicsagas
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
claude plugin install epicsagas/alcove
```

### epic — تثبيت مستقل

**Homebrew** (macOS):
```bash
brew install epicsagas/tap/epic-harness
```

**cargo-binstall** (ملف ثنائي مُجمَّع مسبقاً):
```bash
cargo binstall epic-harness
```

**Cargo** (البناء من المصدر):
```bash
cargo install epic-harness
```

### transpile — تثبيت مستقل

**cargo-binstall** (ملف ثنائي مُجمَّع مسبقاً):
```bash
cargo binstall llm-transpile
```

**Cargo** (البناء من المصدر):
```bash
cargo install llm-transpile
```

### alcove — تثبيت مستقل

**Homebrew** (macOS):
```bash
brew install epicsagas/tap/alcove
```

**cargo-binstall** (ملف ثنائي مُجمَّع مسبقاً):
```bash
cargo binstall alcove
```

**Cargo** (البناء من المصدر):
```bash
cargo install alcove
```

---

## تفاصيل الإضافات

### epic

**إطار عمل الوكيل المستقل**

ابنِ سير عمل للوكلاء تتعامل مع المهام المعقدة متعددة الخطوات بشكل مستقل. مزوّد بـ 6 أوامر قوية مدمجة، تتطور المهارات مع الاستخدام. تعمل خطافات الجلسة تلقائياً لحماية كودك وتحسين المخرجات والتفكير في كل جلسة.

**متى تستخدمه:**
- أتمتة دورات مراجعة الكود والـ commits والاختبارات المتكررة
- تعريف سير عمل مخصصة لكل مشروع
- تطبيق أنماط سلوك متسقة عبر جلسات Claude

**الميزات الرئيسية:**
- 6 أوامر قوية مدمجة (commit، review، test، deploy والمزيد)
- نظام مهارات يتطور ذاتياً — يتعلم من أنماط الاستخدام ويتحسن باستمرار
- خطافات حماية الجلسة — تمنع الأخطاء وتحافظ على الجودة تلقائياً

→ [المصدر والتوثيق](https://github.com/epicsagas/epic-harness)

---

### transpile

**قارئ المستندات المُحسَّن للرموز**

يضغط تلقائياً ملفات `.md` و`.html` و`.txt` في كل استدعاء لأداة Read، مما يقلل استخدام رموز السياق بنسبة تصل إلى 40%. تأثير فوري دون الحاجة إلى تغيير سير العمل.

**متى تستخدمه:**
- المشاريع التي تشير كثيراً إلى مستندات كبيرة أو مواصفات
- عند الوصول المتكرر إلى حدود نافذة السياق
- لتقليل تكاليف الرموز في الجلسات الطويلة

**الميزات الرئيسية:**
- ضغط صامت — نفس المخرجات، أقل بنسبة 40% من الرموز
- يكتشف تلقائياً صيغ `.md` / `.html` / `.txt`
- متوافق تماماً مع سير عمل أداة Read الحالية

→ [المصدر والتوثيق](https://github.com/epicsagas/llm-transpile)

---

### alcove

**خادم MCP للتوثيق**

يمنح وكلاء البرمجة بالذكاء الاصطناعي وصولاً فورياً إلى مستندات مشروعك الخاصة عبر MCP. بحث هجين BM25+متجهي، فحص دلالي، التحقق من المستندات وخادم HTTP في الخلفية مع وضع الوكيل للاستجابة الفورية.

**متى تستخدمه:**
- إدارة توثيق المشاريع الخاصة عبر وكلاء ذكاء اصطناعي متعددين
- البحث في قرارات الهندسة المعمارية وPRDs وrunbooks من أي وكيل متوافق مع MCP
- فرض معايير التوثيق مع التحقق من السياسات والفحص الدلالي

**الميزات الرئيسية:**
- بحث هجين — BM25 + تشابه متجهي مع Reciprocal Rank Fusion
- مستودع توثيق واحد، أي وكيل — Claude Code، Cursor، Gemini CLI، Codex وأكثر من 5 آخرين
- خادم في الخلفية مع وضع الوكيل — يزيل تأخر البداية الباردة في الجلسات الجديدة
- فحص دلالي — روابط معطلة، ملفات يتيمة، علامات قديمة، تواريخ منتهية الصلاحية
- تكامل macOS launchd — أوامر دورة الحياة enable/disable/start/stop/restart

→ [المصدر والتوثيق](https://github.com/epicsagas/alcove)

---

## المساهمة

لتقديم إضافة أو اقتراح تحسينات:

1. افعل fork لهذا المستودع
2. أضف بيانات الإضافة في `.claude-plugin/marketplace.json`
3. افتح Pull Request

تُدار الإضافات كمستودعات GitHub مستقلة. يحتوي هذا السوق على البيانات الوصفية فقط.

---

## الرخصة

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
