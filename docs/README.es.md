# epicsagas plugins

> Plugins artesanales para el desarrollo serio asistido por IA — agentes autónomos, compresión de contexto y herramientas que no interrumpen tu flujo.

[![License](https://img.shields.io/badge/License-Apache--2.0-blue?style=flat)](../LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-2-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

**Traducciones:** [English](../README.md) · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh-cn.md) · [繁體中文](README.zh-tw.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [Русский](README.ru.md) · [العربية](README.ar.md)

---

## Plugins

| Plugin | Descripción | Fuente |
|--------|-------------|--------|
| [epic](#epic) | Arnés de agente autónomo — 6 comandos potentes, habilidades auto-evolutivas y hooks invisibles que protegen, pulen y reflexionan en cada sesión. | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | Lector de documentos optimizado en tokens — comprime silenciosamente archivos `.md`, `.html` y `.txt`, reduciendo el uso de contexto hasta un 40%. | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |

---

## Instalación

Agrega este marketplace a Claude Code:

```bash
claude plugin add epicsagas
```

Instala plugins individuales:

```bash
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
```

---

## Detalles de los plugins

### epic

**Arnés de Agente Autónomo**

Construye flujos de trabajo de agentes que manejan tareas complejas y de múltiples pasos de forma independiente. Equipado con 6 comandos potentes integrados, las habilidades evolucionan con el uso. Los hooks de sesión se ejecutan automáticamente para proteger tu código, pulir la salida y reflexionar sobre cada sesión.

**Cuándo usarlo:**
- Automatizar ciclos repetitivos de revisión de código, commits y pruebas
- Definir flujos de trabajo personalizados por proyecto
- Aplicar patrones de comportamiento consistentes en las sesiones de Claude

**Características principales:**
- 6 comandos potentes integrados (commit, review, test, deploy y más)
- Sistema de habilidades auto-evolutivas — aprende de los patrones de uso y mejora continuamente
- Hooks de guardia de sesión — previene errores y mantiene la calidad automáticamente

→ [Fuente y Documentación](https://github.com/epicsagas/epic-harness)

---

### transpile

**Lector de Documentos Optimizado en Tokens**

Comprime automáticamente archivos `.md`, `.html` y `.txt` en cada llamada a la herramienta Read, reduciendo el uso de tokens de contexto hasta un 40%. Efecto inmediato sin cambios en el flujo de trabajo.

**Cuándo usarlo:**
- Proyectos que referencian frecuentemente documentos grandes o especificaciones
- Cuando alcanzas regularmente los límites de la ventana de contexto
- Para reducir costos de tokens en sesiones largas

**Características principales:**
- Compresión silenciosa — misma salida, hasta 40% menos tokens
- Detecta automáticamente formatos `.md` / `.html` / `.txt`
- Totalmente compatible con los flujos de trabajo existentes de la herramienta Read

→ [Fuente y Documentación](https://github.com/epicsagas/llm-transpile)

---

## Contribuir

Para enviar un plugin o sugerir mejoras:

1. Haz un fork de este repositorio
2. Agrega tu entrada de plugin en `.claude-plugin/marketplace.json`
3. Abre un Pull Request

Los plugins se mantienen como repositorios independientes de GitHub. Este marketplace contiene solo metadatos.

---

## Licencia

Apache-2.0 © [epicsagas](https://github.com/epicsagas)
