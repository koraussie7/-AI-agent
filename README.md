# 🤖 DADA App AI Agent

> OpenClaw 기반 통합 AI Agent Platform — 다다앱을 위한 올인원 에이전트

## 🧬 통합 구성

| # | 프로젝트 | 설명 | 언어/스택 |
|---|---------|------|-----------|
| 1 | **[OpenClaw](https://github.com/openclaw/openclaw)** | AI Agent 프레임워크 (코어) | Node.js |
| 2 | **[Hermes Agent](https://github.com/NousResearch/hermes-agent)** | NousResearch 에이전트 (멀티플랫폼) | Python |
| 3 | **[OpenMythos](https://github.com/kyegomez/OpenMythos)** | 멀티에이전트 오케스트레이션 | Python |
| 4 | **[Mythos Router](https://github.com/thewaltero/mythos-router)** | AI 라우터 & 오케스트레이터 | TypeScript |
| 5 | **[OpenClaude](https://github.com/Gitlawb/openclaude)** | Claude 기반 AI 에이전트 | TypeScript/Bun |
| 6 | **[Roo Code Memory Bank](https://github.com/GreatScottyMac/roo-code-memory-bank)** | 메모리/지식 관리 시스템 | YAML/Markdown |
| 7 | **[Memind](https://github.com/openmemind/memind)** | AI 메모리 & 마인드 스토리지 | Java/Spring |
| 8 | **[OpenViking](https://github.com/volcengine/OpenViking)** | 멀티모달 AI 에이전트 | Rust/Python |
| 9 | **[WrenAI](https://github.com/Canner/WrenAI)** | Text-to-SQL 시맨틱 엔진 | Rust/Python/WASM |
| 10 | **[Obscura](https://github.com/h4ckf0r0day/obscura)** | 프라이버시 AI 브라우저 | Rust |
| 11 | **[Tavily AI Search](https://github.com/cameronking4/github-repo-tavily-ai-search)** | AI 검색 엔진 | Next.js/TypeScript |

## 🚀 시작하기

```bash
# OpenClaw 실행
npm start

# Hermes Agent 실행
cd hermes-agent && python -m hermes_cli

# OpenClaude 실행
cd openclaude && bun run src/index.ts
```

## 📦 디렉토리 구조

```
dada-agent/
├── (루트)               ← OpenClaw 코어
├── hermes-agent/        ← Hermes Agent
├── open_mythos/         ← OpenMythos
├── mythos-router/       ← Mythos Router
├── openclaude/          ← OpenClaude
├── roo-memory-bank/     ← Memory Bank
├── memind/              ← Memind
├── openviking/          ← OpenViking
├── wrenai/              ← WrenAI
├── obscura/             ← Obscura
└── tavily-search/       ← Tavily Search
```

## 🏗️ 아키텍처

```
┌──────────────────────────────────────────────────┐
│                 DADA App Agent                    │
├──────────────────────────────────────────────────┤
│  OpenClaw (Core Framework)                       │
├──────┬──────┬──────┬──────┬──────┬──────┬───────┤
│Her-  │Open  │Mythos│Open  │Open  │Obscu-│Tavily │
│mes   │Mythos│Router│Claude│Viking│ra    │Search │
│      │      │      │      │      │      │       │
├──────┴──────┴──────┴──────┴──────┴──────┴───────┤
│  Memory Layer                                    │
├─────────────────┬───────────────────────────────┤
│  Roo Memory Bank│  Memind │ WrenAI (Data)       │
└─────────────────┴───────────────────────────────┘
```

## 📄 라이선스

각 프로젝트는 원본 라이선스를 따릅니다.
- OpenClaw: Apache 2.0
- Hermes Agent: Apache 2.0
- OpenMythos: Apache 2.0
- Mythos Router: MIT
- OpenClaude: Apache 2.0
- Roo Memory Bank: MIT
- Memind: Apache 2.0
- OpenViking: Apache 2.0
- WrenAI: Apache 2.0 / AGPL-3.0
- Obscura: GPL-3.0
- Tavily Search: MIT

---

_Made with ❤️ for DADA App_
