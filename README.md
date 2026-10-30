# ai-engineer ⚡

> **The Massively Parallel, Contract-First AI Company Operating Engine.**
> Inspired by the senior engineering discipline of [Ponytail](https://github.com/DietrichGebert/ponytail).

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Skills.sh](https://img.shields.io/badge/skills.sh-ai--engineer-brightgreen)](https://skills.sh)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Plugin-purple)](https://claude.ai)

Traditional software teams move sequentially: Product writes PRDs, Design builds mockups, Backend writes APIs, Frontend implements views, QA finds regressions, Marketing writes launch copy, and DevOps configures monitors.

`ai-engineer` replaces this sequential waterfall with **Contract-First Synchronization**. By freezing strict data contracts at $T=0$, an AI agent runs systems architecture, AI prompt engineering, frontend design, automated evals, and GTM execution **simultaneously in parallel**, compressing weeks of work into single-pass execution.

---

## ⚡ Quick Start

### Install via skills.sh / npx
```bash
npx skills add https://github.com/username/ai-engineer --skill ai-engineer
```

### Install in Claude Code
```bash
/plugin marketplace add username/ai-engineer
/plugin install ai-engineer@ai-engineer
```

### Cursor / Codex / Universal Agents
Add `skills/ai-engineer/SKILL.md` to your project's `.cursor/rules/`, `AGENTS.md`, or agent context directory.

---

## 🏛️ The Architecture: Contract-First Parallelism

```
                         [ Phase 0: Contract Freeze (T=0) ]
            (Pydantic Models, OpenAPI Schemas, State Machines, UX SLAs)
                                      |
     +-----------------+--------------+---------------+-----------------+
     |                 |              |               |                 |
 [ Thread A ]     [ Thread B ]   [ Thread C ]    [ Thread D ]      [ Thread E ]
 Systems & Data   AI & Prompts   UI/UX Front     Evals & QA        GTM & RevOps
 - DB schemas     - Model tier   - UI components - Golden evals    - Landing copy
 - Async workers  - RAG index    - Stream hooks  - Red-teaming     - Docs & quickstart
 - Server routes  - Schema retry - Design tokens - CI assertions   - Stripe & margins
     |                 |              |               |                 |
     +-----------------+--------------+---------------+-----------------+
                                      |
                   [ Phase 2: Convergence & Integration Barrier ]
           (End-to-End Test Suite, Observability Verification, Release Gate)
```

---

## 📦 What's Inside

| Path | Purpose |
| :--- | :--- |
| `skills/ai-engineer/` | Core solo company operating engine and parallel execution framework |
| `skills/ai-engineer-audit/` | Codebase scanner that detects vibe-prompting, missing schemas, and AI bloat |
| `skills/ai-engineer-eval/` | Golden dataset generator and 3-tier automated evaluation harness |
| `evals/` | Runnable benchmark test runner measuring token savings and schema reliability |
| `AGENTS.md` | Universal root specification file for agent portability |

---

## 🧭 The AI Engineering Ladder

Before adding complexity, the agent must stop at the lowest viable rung:
1. **Deterministic Code First**: Use regex, string parsing, arithmetic, or SQL before calling an LLM.
2. **Zero-Shot with Strict Schema**: Enforce typed Pydantic/Zod schemas with constrained decoding.
3. **Dynamic Few-Shot Grounding**: Retrieve 2-4 verified exemplars; optimize prompt prefixes for caching.
4. **Constrained Tool Calling**: Use typed, idempotent tool contracts with recursion ceilings (max 5-8 turns).
5. **Hybrid RAG**: Combine dense vector embeddings + BM25 keyword matching + cross-encoder reranking.
6. **Model Distillation & Fine-Tuning**: Apply only when latency, domain tone, or token costs demand it.

---

## 🧪 Benchmark & Evaluation Suite

Run the included benchmark runner to verify your AI agents:
```bash
python3 evals/benchmark_suite.py
```

Measures:
* **Token Budget Reduction**: Eliminates verbose prompt bloat and maximizes prefix cache reuse.
* **Schema Pass Rate**: Guarantees 100% valid JSON responses via automated reflection retries.
* **Zero-Hallucination Retrieval**: Validates hybrid BM25 + dense vector ranking against gold standards.

---

## 📜 License

MIT License. See [LICENSE](LICENSE) for details.
