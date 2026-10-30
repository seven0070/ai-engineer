---
name: ai-engineer-eval
description: Automatically scaffolds golden evaluation test suites, assertion runners, and adversarial red-teaming checks for LLM applications. Use when setting up CI/CD model testing, designing benchmark datasets, or preventing prompt regression.
---
# ai-engineer-eval

An automated evaluation generator that builds rigorous test suites for AI features, replacing subjective "vibe checks" with deterministic and statistical regression tests.

## The 3-Tier Evaluation Architecture

For any AI feature or prompt pipeline, generate tests across three tiers:

### Tier 1: Deterministic Assertions (Fast, Zero Model Call Cost)
- Schema validation: Pydantic/Zod parse success.
- Regex pattern matching for mandatory fields.
- Latency and token consumption ceilings.

### Tier 2: Statistical & Semantic Assertions
- Cosine similarity against golden reference answers.
- Keyword and entity recall (BLEU/ROUGE or exact entity inclusion).
- Output length and compression ratios.

### Tier 3: Calibrated Binary LLM-as-a-Judge
- Single-criteria binary rubrics (Pass/Fail) rather than 1-10 scores.
- Clear grading rubrics with explicit failure condition examples.
- Judge model tiering (independent evaluator model to prevent self-preference bias).

## Adversarial Stress-Testing Suite
- Prompt injection injection tests (e.g. "Ignore previous instructions").
- Boundary escape and system prompt exfiltration probes.
- Malformed or empty input resilience tests.
