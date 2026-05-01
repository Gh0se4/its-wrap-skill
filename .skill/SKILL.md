---
name: its-wrap
description: Use when researchers need to turn rough research outputs, vibe-coding projects, runnable frontends/backends, demos, algorithms, prompts, screenshots, or notes into product-decision handoff material for product managers or leaders.
---

# Its Wrap

## Overview

Turn research assets into a product-decision handoff package. This skill guides reasoning and framing; it is not a rigid fill-in template.

It helps researchers move from "the research is done" to "a PM can decide what to do next."

## When to Use

Use this when the input is research-oriented and needs to become decision material, such as:

- research demos, prototypes, algorithms, models, prompts, agents, scripts, notebooks, or code
- vibe-coding projects with runnable frontends, backends, APIs, or databases
- PRDs, technical notes, experiment logs, screenshots, rough drafts, or fragmented ideas
- AI/LLM capabilities that may become product features
- early-stage work where evidence, cost, users, or integration paths are incomplete

Do not use this as a generic summary skill. The output must support product decision-making.

## Core Principle

Translate research into PM decision language:

```text
Research content → user problem → product value → product shape → evidence → cost/risk → execution path → decision gaps
```

The skill is strict about what must be considered, but flexible about wording, length, and section granularity.

## First: Judge Information Sufficiency

Before producing the handoff, decide whether missing information blocks useful decision-making.

Ask clarifying questions when missing information may change:

- target user or usage scenario
- core problem or product value
- product form or system position
- feasibility, cost, risk, or integration path
- whether this should proceed at all

Clarification rules:

- ask only the most decision-critical question first
- prefer multiple-choice questions when possible
- ask one question at a time
- do not require every gap to be resolved before output
- if the user wants to continue, still produce the handoff and mark the gaps clearly

If gaps do not block an initial decision, continue and label unknowns as `TBD`, `to verify`, or `assumption`.

## Required Reasoning Checklist

Always consider these areas, even if some remain blank:

| Area | Required thinking |
|---|---|
| Problem | Who has the problem, what pain exists, and why current handling is insufficient |
| Research asset | What exists now: demo, code project, frontend, backend, API, model, prompt, docs, screenshots, experiments |
| Product value | What user value this creates, not just what the technology can do |
| Product shape | How it may appear as a feature, workflow, tool, API, automation, assistant, admin panel, dashboard, or full app |
| Evidence | Current demo result, sample size, baseline, metrics, or explicit lack of evidence |
| Quantitative value | Metrics, baseline comparison, expected improvement direction |
| Non-quantitative value | Experience, strategic, risk, or cognitive value with confidence |
| Alternatives | Simpler manual flows, rules, existing tools, or traditional models |
| Execution | MVP path, integration point, dependencies, owners, rollout path |
| Demo usage | If a runnable frontend/backend or code project exists, extract what can be shown to PMs and how it should be presented |
| Cost | Development, data, model/API, runtime, and maintenance cost |
| Risk | Technical, business, compliance, data, model, operational, and adoption risks |
| Observability | Logs, success metrics, error rates, human review, alerts, feedback loop |
| Missing information | What is unknown and how it affects the decision |
| Next action | What should be researched, validated, estimated, or reviewed next |

## Output Contract

Produce a handoff package that a PM can use to decide the next step. Adapt depth to input quality and complexity, but cover every required decision area.

### 1. Executive Summary

- what the research asset is
- what product problem it may solve
- why it may be worth continuing
- current decision recommendation: proceed / validate first / pause / insufficient information
- confidence level: high / medium / low

### 2. Problem and User Scenario

- target user or role
- usage scenario
- current pain point
- existing workaround or process
- why now

### 3. Research Asset Reconstruction

- input type: code project / runnable frontend-backend / demo / model / prompt / PRD / doc / screenshot / notes / mixed
- current capability
- current implementation shape: script / CLI / frontend / backend / API / database / local app / deployed service
- demo entry points: page, endpoint, command, screenshot, recording, or run steps
- what has been verified
- what has not been verified
- what can be reused directly
- what is only good for demonstration and should not be treated as production-ready

### 4. Productized Solution

- product-language feature description
- proposed user flow
- system position: new feature / enhancement / replacement / internal tool / external capability
- if a runnable frontend/backend exists, explain which pages, endpoints, or flows can support PM demos
- expected user-visible behavior
- explicit non-goals or boundaries

### 5. Decision Evidence

If quantitative evidence exists, state:

- metric
- baseline
- current result
- data source and sample size
- reliability of the evidence

If no metric exists, say so clearly and propose proxy metrics such as:

- time saved
- error rate reduced
- manual steps reduced
- review throughput increased
- completion rate increased
- complaint or rework rate reduced

### 6. Non-Quantitative Value

When value cannot yet be measured directly, use this structure:

```text
Type: experience / strategy / risk reduction / cognition / operational efficiency
Description:
Potential proxy metric:
Validation method:
Confidence: high / medium / low
Impact scope: local / cross-team / company-wide
```

### 7. Alternatives and Comparison

Include at least one simpler alternative when possible.

```text
Existing approach:
Proposed approach:
Simpler alternative:
Difference:
Tradeoff:
```

Compare by value, cost, risk, speed, scalability, and maintainability.

### 8. Execution Path

- MVP version
- integration point
- required data or interfaces
- technical changes
- reusable, rewrite-needed, and discard-needed parts of any existing code project
- what is still missing to move from demo to production: auth, permissions, config, deployment, monitoring, persistence, error handling, scalability
- product / design / operations dependencies
- suggested phases: validation → pilot → integration → rollout
- suggested participants

### 9. Cost Model

Include known values or blanks:

- development effort
- data collection or labeling cost
- model/API/runtime cost, especially for AI projects
- QPS or usage estimate, if relevant
- monthly cost range, if estimable
- maintenance and monitoring cost

### 10. Risks and Boundaries

Cover likely risks:

- technical feasibility
- data quality or availability
- model instability or hallucination, if AI-related
- edge cases and non-ideal inputs
- integration complexity
- vibe-coding risks: unstable prototype code, missing tests, messy state management, unclear API contracts, unclear environment dependencies, missing security or permissions
- user adoption risk
- compliance, privacy, or security risk
- failure modes and fallback expectations

### 11. Data and Optimization Loop

- data source
- data quality requirement
- labeling requirement
- feedback collection method
- offline evaluation plan
- online monitoring metrics
- iteration mechanism

### 12. Missing Information and Discussion Points

Write missing items as decision gaps, not generic questions.

For each gap:

```text
Missing item:
Why it matters for PM decision:
Suggested way to fill it:
Priority: high / medium / low
```

### 13. Recommended Next Actions

Give concrete next steps:

- what to do next
- who should participate: researcher / PM / engineer / designer / ops / legal / data owner
- priority
- expected output of that step

## Code Project Input Handling

If the input includes a code repository, vibe-coding project, or runnable frontend/backend, treat it as part of the research asset but do not turn this skill into a code review tool.

Focus on extracting:

- user flows and core capabilities already demonstrable
- how frontend pages map to product features
- how backend interfaces, data flows, and external dependencies support capabilities
- which parts can support PM demos, user interviews, or pilot validation
- which parts are prototype-only and should not be treated as production-ready
- what is still missing from "it runs" to "it can ship"

Do not provide line-by-line code review unless code issues directly affect product decisions such as security, cost, performance, data reliability, or integration feasibility.

## AI-Specific Checks

If the research involves LLMs, agents, prompts, RAG, classifiers, or AI automation, also consider:

- prompt or model behavior summary
- whether RAG is used
- whether there are tool calls or external system calls
- whether human review is required
- fallback path
- evaluation set and acceptance criteria
- cost per call and expected usage
- safety, privacy, and controllability
- quality drift monitoring

Do not claim AI quality without evidence. If the evidence is observational, label it as such.

## Maturity Model

Assess research maturity when useful:

| Level | Meaning |
|---|---|
| L0 Idea | Only a concept or rough note exists |
| L1 Demo | A demo or script exists, but validation is limited |
| L2 Validated | Has evaluation data, user feedback, or operational feedback |
| L3 Integrable | Has interfaces, data paths, and a system integration plan |
| L4 Launchable | Has cost model, monitoring, fallback, and rollout plan |

Use maturity to guide next actions. Do not overstate readiness.

## Decision Scoring

When helpful, score each dimension from 1-5 or high / medium / low:

- business impact
- user value
- technical feasibility
- implementation cost
- risk level
- scalability
- evidence strength

Explain each score. If evidence is missing, score conservatively or leave it blank.

## Forbidden Output Patterns

Avoid:

- vague claims like "great results" or "high value" without evidence or confidence
- quantified claims without source, sample, or baseline
- describing only technology without user value
- hiding missing information
- treating assumptions as facts
- forcing every project into the same long template when a concise handoff is enough
- making final product decisions on behalf of the PM without stating uncertainty

## Good Default Behavior

- use PM-facing language in the main output
- keep research details only when they support decisions
- separate facts, assumptions, and unknowns
- keep the handoff actionable
- make the next discussion easier, not longer
- when input is weak, produce a useful first draft with visible blanks

## Minimal Example

Input:

```text
We built an LLM demo that automatically groups customer-support ticket reasons. It reads a batch of tickets and outputs first-level and second-level reason labels plus summaries. It looks decent on 200 historical tickets, but there are no formal metrics yet. The goal may be to reduce the time support managers spend manually summarizing issues each week. It is not connected to a system yet, and cost is unclear.
```

Good response shape:

```text
## Executive Summary
This is a customer-support ticket grouping demo. The likely product value is reducing recurring manual summary work and improving visibility into issue patterns. Recommendation: move to small-scale validation first, not direct launch planning. Confidence: medium-low because accuracy, manual baseline, system integration cost, and real user feedback are still missing.

## Problem and User Scenario
Target user: support manager / operations analyst
Scenario: review weekly or daily ticket themes, identify recurring problems, and drive improvements
Current pain: manual reading, grouping, and summarizing is slow and inconsistent
To verify: current workflow, frequency, time spent, and error rate

## Productized Solution
Feature: automated ticket reason grouping and summary
Workflow: ingest tickets → generate first-level / second-level reason labels → PM or ops reviews distribution and summary → human correction → trend report
Boundary: should not replace formal operational judgment yet; human review is still required

## Decision Evidence
Known: demo results on 200 historical tickets
Missing: label accuracy, recall, human agreement, baseline, evaluation set source
Proxy metrics: weekly summarization time, manual correction rate, label agreement, issue discovery lead time

## Missing Information and Discussion Points
Missing item: how much time support managers currently spend summarizing tickets each week
Why it matters: determines ROI and priority
Suggested way to fill it: interview 2-3 support managers and trace the last two weeks of their workflow
Priority: high
```

The final output should continue with execution path, cost, risk, data loop, and next actions.
