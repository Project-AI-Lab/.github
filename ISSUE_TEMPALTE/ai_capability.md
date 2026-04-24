---
name: AI Capability Proposal
about: Propose a reusable AI capability to build in pw-ai-capabilities
title: "[CPABILITY] "
labels: capability, proposal
assignees: ''
---

## capability Name
(e.g., Prompt Orchestration, Evaluation layer)
<!-- e.g., Prompt Orchestration, Evaluation Layer, Semantic Chunker -->

## What it Does
Describe the capability.
<!-- Describe the capability in 2-3 sentences. What does it do, not how it does it. -->

## Why it Mattters
What problem does it solve?
<!-- What problem does it solve? What breaks or slows down without it? -->

## Where It Applies
<!-- Which projects, apps, or client scenarios will use this? Be specific — this is the reusability proof. -->
- 
- 

## Target Layer

- [ ] `pw-ai-capabilities` — reusable AI logic with some domain knowledge
- [ ] `pw-ai-core` — purely foundational, zero business logic
- [ ] Not sure — needs discussion

## Inputs / Outputs

**Inputs:**

**Outputs:**

## Rough Interface

```python
# What should calling this look like?
# Even a sketch helps align before building.
```

## Dependencies
- **Model** (e.g., Claude Sonet, any)
- **Data** (e.g., document corpus, none)
- **Tools / Libraries:** (e.g., LlamaIndex, none)
- **Other capabilities:** (e.g., depends on pw-ai-core logging)

## Reusability Score

- [ ] High (cross-use case) - needed across 3+ projects or clients
- [ ] Medum - needed for 2 projects
- [ ] Low - needed for 1 project (consider building in appp first, extract later)

## Priority

- [ ] High - blocking current work
- [ ] Medium - needed soon
- [ ] Low - future investment

## Notes / Open questions

<!--
- Any design decisions that need discussion?
- Known risks or unknowns?
-->


