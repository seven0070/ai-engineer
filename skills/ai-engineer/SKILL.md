---
name: ai-engineer
description: Autonomous enterprise AI founder and massively parallel company operating engine. Executes all cross-functional company workstreams—executive strategy, system architecture, full-stack AI implementation, frontend design, QA evals, security audits, GTM documentation, and unit economics—simultaneously in parallel using contract-first synchronization. Compresses full-company build cycles into rapid, high-throughput execution passes.
---
# ai-engineer

An elite autonomous enterprise operating framework designed to execute the full workload of an entire AI technology company concurrently. By replacing sequential, department-by-department handoffs with contract-first parallel workstreams, it collapses weeks of company operations into synchronized, high-throughput execution.

## When to Use

- Building and launching production AI products in record time without sequential bottlenecks.
- Executing multi-department workflows simultaneously: strategy, architecture, backend, frontend, evals, GTM, and ops.
- Developing contract-first architectures where APIs, UIs, AI prompts, and test suites are developed concurrently against shared schemas.
- Replacing siloed organizational coordination with a single, highly synchronized parallel execution engine.
- Auditing security, benchmarking performance, and optimizing unit economics concurrently with feature development.

## The Massively Parallel Execution Model

Traditional companies work sequentially: Product writes specs -> Design creates mocks -> Backend builds APIs -> Frontend integrates -> QA tests -> Marketing writes copy -> Ops monitors. 

The **ai-engineer** model executes these streams simultaneously using **Contract-First Synchronization**:

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

## The 5 Synchronous Workstreams

Once data contracts and type definitions are frozen in Phase 0, all five streams execute in parallel:

### 1. Thread A: Systems & Infrastructure (Backend Engineering)

- Spins up high-throughput async server endpoints (FastAPI, Next.js, Node.js).
- Generates database migrations, ORM schemas, and relational indexes.
- Configures background worker queues (Redis, Celery, BullMQ) and event streaming (SSE/WebSockets).
- Implements idempotency keys and state persistence layers.

### 2. Thread B: Intelligence & Model Pipelines (AI Engineering)

- Configures model tiering (fast small models for routing, frontier models for complex reasoning).
- Assembles hybrid retrieval engines (dense vector embeddings + BM25 keyword matching + cross-encoder reranking).
- Constructs prefix-cache-optimized prompt templates and strict JSON schema constrained decoders.
- Builds automated retry loops with error-reflection logic for schema self-correction.

### 3. Thread C: Interface & Interaction Flow (Product & Frontend Design)

- Develops responsive, accessible component hierarchies using modular styling (Tailwind CSS, Radix UI).
- Implements progressive streaming UX patterns, optimistic state updates, and latency-masking skeletons.
- Integrates frontend client hooks with the backend contracts and mock fixtures.

### 4. Thread D: Rigorous Verification & Security (QA & InfoSec)

- Generates a golden evaluation dataset with 30-50 real-world examples, edge cases, and historical regressions.
- Builds automated assertion harnesses: deterministic schema validity, latency profiling, and binary LLM scoring.
- Conducts adversarial red-teaming: prompt injection, boundary escapes, data leakage, and denial-of-wallet stress tests.

### 5. Thread E: Commercialization & GTM (Marketing, Docs & RevOps)

- Crafts commercial product positioning, value proposition copy, and launch announcements.
- Produces comprehensive developer documentation, API references, quickstart tutorials, and sample repos.
- Instruments unit-economic tracking: input/output token monitors, cache hit rates, and Stripe billing meters.

## Convergence Protocol: Zero-Delay Integration

To ensure all concurrent threads lock together seamlessly without integration drift:

1. **Phase 0 Contract Freeze**:
   - Every interface (database models, API endpoints, LLM output schemas, and client state) is explicitly typed before code generation begins.
   - Mock response stubs are produced instantly so frontend and QA can proceed immediately without waiting for backend implementation.

2. **Parallel Tooling Fan-Out**:
   - Independent files, components, and configurations are written and validated concurrently across independent modules.

3. **The Convergence Barrier**:
   - Once all streams complete their execution pass, the system runs end-to-end integration tests that stitch frontend, backend, AI models, and monitoring hooks together.
   - Any integration failure is isolated and repaired locally using reflection without breaking other workstreams.

## Operational Discipline & Hard Guardrails

- **Immutable Contracts During Execution**: Do not alter frozen interfaces mid-flight without updating mock fixtures across all parallel tracks.
- **Human Approval for Irreversible Operations**: Always pause for explicit user confirmation before executing financial transactions, production database drops, or external service provisioning.
- **Strict Context Hygiene**: Prune intermediate scratchpads and raw tool outputs to prevent context pollution during high-throughput execution.
- **Fail-Safe Fallbacks**: Every asynchronous pipeline must include graceful degradation paths, explicit timeouts, and circuit breakers.
