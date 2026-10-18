# Expected Impact Record — Support Agent

## Workload

- **WorkloadId:** `support-agent`
- **Period:** `2026-09`

## Work

- **Attempted Work Units:** 50,000 customer cases
- **Accepted Work Units:** 38,000 customer cases
- **Acceptance Rate:** 76%

## Cost

- **Effective Cost:** $80,000
- **Cost per Accepted Work Unit:** $2.11 per accepted case

> Effective Cost is assumed to come from FinOps / FOCUS for this prototype.

## Outcomes

### Handling Time

- **Metric:** Average handling time
- **Baseline:** 12.0 minutes
- **Observed:** 9.0 minutes
- **Change:** -25%
- **Evidence Status:** OBSERVED
- **Attribution Method:** before_after
- **Attribution Status:** ATTRIBUTED

### Escalation Rate

- **Metric:** Escalation rate
- **Baseline:** 18%
- **Observed:** 14%
- **Change:** -4 percentage points
- **Evidence Status:** OBSERVED
- **Attribution Method:** matched_comparison
- **Attribution Status:** ATTRIBUTED

### Conversion Rate

- **Metric:** Conversion rate
- **Baseline / Control:** 11%
- **Observed / AI-assisted:** 13%
- **Change:** +2 percentage points
- **Evidence Status:** INCREMENTAL
- **Attribution Method:** controlled_experiment
- **Attribution Status:** INCREMENTAL

## Economic Value

### Labor Capacity Value

- **Amount:** $150,000
- **Method:** modeled_from_time_saved
- **Derived From:** `handling_time`
- **Evidence Status:** MODELED

### Avoided Escalation Cost

- **Amount:** $60,000
- **Method:** modeled_from_escalation_reduction
- **Derived From:** `escalation_rate`
- **Evidence Status:** MODELED

### Incremental Revenue

- **Amount:** $90,000
- **Method:** controlled_experiment
- **Derived From:** `conversion_rate`
- **Evidence Status:** INCREMENTAL

## Decision Context

The workload shows:

- strong Accepted Work performance,
- observed and attributed operational improvements,
- modeled capacity and avoided-cost value,
- and incremental revenue evidence from a controlled comparison.

The modeled value claims should not be treated as realized ROI.

A downstream decision process could use this Impact Record to support actions such as **PROVE**, **OPTIMIZE**, or **SCALE**, depending on additional business, risk, and strategic context.
