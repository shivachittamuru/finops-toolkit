# Expected Impact Record — Coding Agent

## Workload

- **WorkloadId:** `coding-agent`
- **Period:** `2026-09`

## Work

- **Attempted Work Units:** 1,200 engineering tasks
- **Accepted Work Units:** 900 engineering tasks
- **Acceptance Rate:** 75%

## Cost

- **Effective Cost:** $45,000
- **Cost per Accepted Work Unit:** $50 per accepted engineering task

> Effective Cost is assumed to come from FinOps / FOCUS for this prototype.

## Outcomes

### Engineering Task Cycle Time

- **Metric:** Engineering task cycle time
- **Baseline:** 16 hours
- **Observed:** 12 hours
- **Change:** -25%
- **Evidence Status:** OBSERVED
- **Attribution Method:** matched_comparison
- **Attribution Status:** ATTRIBUTED

### Engineering Rework Rate

- **Metric:** Engineering rework rate
- **Baseline:** 20%
- **Observed:** 15%
- **Change:** -5 percentage points
- **Evidence Status:** OBSERVED
- **Attribution Method:** before_after
- **Attribution Status:** OBSERVED

### Deployment Throughput

- **Metric:** Successful deployments per period
- **Baseline:** 80 deployments
- **Observed:** 96 deployments
- **Change:** +20%
- **Evidence Status:** OBSERVED
- **Attribution Method:** matched_comparison
- **Attribution Status:** ATTRIBUTED

## Economic Value

### Engineering Capacity Value

- **Amount:** $180,000
- **Method:** modeled_from_cycle_time_reduction
- **Derived From:** `cycle_time`
- **Evidence Status:** MODELED

### Avoided Rework Cost

- **Amount:** $70,000
- **Method:** modeled_from_rework_reduction
- **Derived From:** `rework_rate`
- **Evidence Status:** MODELED

### Delivery Capacity Value

- **Amount:** $120,000
- **Method:** modeled_from_deployment_throughput
- **Derived From:** `deployment_throughput`
- **Evidence Status:** MODELED

## Decision Context

The workload shows:

- a 75% Accepted Work rate,
- lower engineering cycle time,
- lower observed rework,
- increased deployment throughput,
- and several modeled economic value opportunities.

The economic value claims remain modeled and should not be treated as realized ROI.

The rework outcome also has weaker attribution evidence than the cycle-time and deployment-throughput outcomes.

A downstream decision process could use this Impact Record to identify where stronger evidence would be most valuable before scaling or making ROI claims.

