# epicsagas plugins

> Handcrafted plugins for serious AI-assisted development — autonomous agents, context compression, and tools that get out of your way.

[![License](https://img.shields.io/github/license/epicsagas/claude-plugins?style=flat)](LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green?style=flat)](https://github.com/epicsagas/claude-plugins)
[![Plugins](https://img.shields.io/badge/Plugins-2-blueviolet?style=flat)](https://github.com/epicsagas/claude-plugins)
[![GitHub Stars](https://img.shields.io/github/stars/epicsagas/claude-plugins?style=flat)](https://github.com/epicsagas/claude-plugins/stargazers)
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/epicsaga)

## 플러그인 목록

| 플러그인 | 설명 | 소스 |
|---------|------|------|
| [epic](#epic) | 자율 에이전트 하니스 — 6개의 파워 커맨드, 자가 진화 스킬, 세션마다 작동하는 보이지 않는 훅 | [epicsagas/epic-harness](https://github.com/epicsagas/epic-harness) |
| [transpile](#transpile) | 토큰 최적화 문서 리더 — `.md`, `.html`, `.txt` 파일을 자동 압축해 컨텍스트 사용량 최대 40% 절감 | [epicsagas/llm-transpile](https://github.com/epicsagas/llm-transpile) |

---

## 설치

Claude Code에서 이 마켓플레이스를 추가합니다:

```bash
claude plugin add epicsagas
```

개별 플러그인 설치:

```bash
claude plugin install epicsagas/epic
claude plugin install epicsagas/transpile
```

---

## 플러그인 상세

### epic

**자율 에이전트 하니스**

복잡한 멀티스텝 작업을 독립적으로 수행하는 에이전트 워크플로우를 구축합니다. 6개의 파워 커맨드로 구성되어 있으며, 스킬이 사용될수록 자가 진화합니다. 세션마다 자동으로 실행되는 훅이 코드를 보호하고, 다듬고, 반성합니다.

**언제 사용하나요?**
- 반복적인 코드 리뷰, 커밋, 테스트 사이클을 자동화할 때
- 프로젝트별 커스텀 워크플로우를 정의하고 싶을 때
- Claude 세션 전반에 걸쳐 일관된 행동 패턴이 필요할 때

**주요 기능:**
- 6개 내장 파워 커맨드 (commit, review, test, deploy 등)
- 자가 진화 스킬 시스템 — 사용 패턴을 학습하여 점진적으로 개선
- 세션 가드 훅 — 실수를 방지하고 품질을 자동으로 유지

→ [소스 및 문서](https://github.com/epicsagas/epic-harness)

---

### transpile

**토큰 최적화 문서 리더**

Read 툴 호출 시 `.md`, `.html`, `.txt` 파일을 자동으로 압축하여 컨텍스트 토큰 사용량을 최대 40% 절감합니다. 워크플로우 변경 없이 즉시 효과가 나타납니다.

**언제 사용하나요?**
- 대형 문서나 레퍼런스를 자주 참조하는 프로젝트에서
- 컨텍스트 윈도우 한계에 자주 도달할 때
- 긴 세션에서 토큰 비용을 줄이고 싶을 때

**주요 기능:**
- 무음 압축 — 출력은 동일하게, 토큰은 최대 40% 절감
- `.md` / `.html` / `.txt` 포맷 자동 감지
- 기존 Read 툴 워크플로우와 완전 호환

→ [소스 및 문서](https://github.com/epicsagas/llm-transpile)

---

## 기여하기

플러그인을 제출하거나 개선을 제안하려면:

1. 이 레포지토리를 포크합니다
2. `.claude-plugin/marketplace.json`에 플러그인 정보를 추가합니다
3. Pull Request를 제출합니다

플러그인은 독립적인 GitHub 레포지토리로 관리되며, 마켓플레이스는 메타데이터만 포함합니다.

---

## 라이선스

MIT © [epicsagas](https://github.com/epicsagas)
