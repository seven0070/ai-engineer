---
name: ai-engineer-audit
description: Audits codebases, prompts, and architectures for AI anti-patterns, prompt bloat, missing schemas, unindexed RAG, and unbounded agent loops. Use when reviewing AI pull requests, inspecting LLM applications for latency/cost waste, or diagnosing production hallucinations.
---
# ai-engineer-audit

A specialized diagnostic auditor that inspects software repositories and prompt libraries for expensive AI anti-patterns, security vulnerabilities, and latency bloat.

## Audit Checklist

When invoked on a file, directory, or pull request, check against these 5 pillars:

### 1. Prompt Bloat & Prefix Cache Hygiene
- Are static instructions at the top of the prompt or mixed dynamically?
- Does the prompt include unpruned conversational turns or raw debug logs?
- Could verbose explanations be replaced with concise structured schemas?

### 2. Schema Rigor & Type Safety
- Does the LLM return free-form text when structured JSON was required?
- Is there a validation layer (Pydantic / Zod) with automated retry/repair?
- Are fallback default responses defined in case of model degradation?

### 3. Retrieval & RAG Health
- Is vector search relying solely on dense embeddings without BM25 keyword matching?
- Is a cross-encoder reranker utilized before feeding top-K chunks to the model?
- Are document chunks oversized or missing metadata filters?

### 4. Agent Control Boundaries
- Is there an explicit maximum iteration ceiling (e.g. max 5-8 turns)?
- Are mutating or destructive actions protected by human-in-the-loop gates?
- Are tool functions idempotent?

### 5. Unit Economics & Model Routing
- Are frontier models being used for simple classification, routing, or extraction?
- Is streaming implemented for interactive user queries?
- Are high-frequency deterministic queries cached?
