# Expected Impact Record — RAG Assistant

## Workload

- **WorkloadId:** `rag-assistant`
- **Period:** `2026-09`

## Work

- **Attempted Work Units:** 20,000 user questions
- **Accepted Work Units:** 15,000 answers
- **Acceptance Rate:** 75%

## Cost

- **Effective Cost:** $60,000
- **Cost per Accepted Work Unit:** $4.00 per accepted answer

> Effective Cost is assumed to come from FinOps / FOCUS for this prototype.

## Outcomes

### Task Completion Rate

- **Metric:** User task completion rate
- **Baseline:** 62%
- **Observed:** 74%
- **Change:** +12 percentage points
- **Evidence Status:** OBSERVED
- **Attribution Method:** matched_comparison
- **Attribution Status:** ATTRIBUTED

### Time to Answer

- **Metric:** Average time to answer
- **Baseline:** 10 minutes
- **Observed:** 6 minutes
- **Change:** -40%
- **Evidence Status:** OBSERVED
- **Attribution Method:** before_after
- **Attribution Status:** OBSERVED

### Escalation Rate

- **Metric:** Human escalation rate
- **Baseline:** 22%
- **Observed:** 16%
- **Change:** -6 percentage points
- **Evidence Status:** OBSERVED
- **Attribution Method:** matched_comparison
- **Attribution Status:** ATTRIBUTED

## Economic Value

### Productivity Value

- **Amount:** $200,000
- **Method:** modeled_from_time_saved
- **Derived From:** `time_to_answer`
- **Evidence Status:** MODELED

### Avoided Escalation Cost

- **Amount:** $80,000
- **Method:** modeled_from_escalation_reduction
- **Derived From:** `escalation_rate`
- **Evidence Status:** MODELED

### Task Completion Value

- **Amount:** $140,000
- **Method:** modeled_from_task_completion_improvement
- **Derived From:** `task_completion_rate`
- **Evidence Status:** MODELED

## Decision Context

The workload shows:

- a 75% Accepted Work rate,
- higher observed task completion,
- lower time to answer,
- lower escalation,
- and several modeled economic value opportunities.

The value claims remain modeled and should not be treated as realized ROI.

The time-to-answer outcome also has weaker attribution evidence than task completion and escalation.

A downstream decision process could use this Impact Record to identify where stronger evidence is needed before making investment or scaling claims.
