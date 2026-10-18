# Coding Agent Impact Measurement Prototype

This folder applies the same **AI Economics Impact Measurement Specification** used by the support-agent prototype to an AI-assisted software development workload.

The purpose is to test whether the measurement model remains reusable across a substantially different AI workload.

## Scenario

The workload is an AI coding agent supporting software engineering tasks.

The business wants to understand:

- how much engineering work the AI-assisted workflow attempts,
- how much work meets the Accepted Work definition,
- whether engineering outcomes improve,
- how strongly those improvements can be attributed to AI,
- what economic value can reasonably be modeled,
- and how those results relate to FinOps cost.

## Files

### `impact-spec.yaml`

Defines:

- workload identity,
- engineering task as the primary work unit,
- Accepted Work criteria,
- engineering outcomes,
- attribution methods,
- economic value measures,
- and outcome-to-value relationships.

### `work-evidence.csv`

Contains work evidence for the measurement period.

Current sample:

- 1,200 attempted engineering tasks
- 900 Accepted Work units
- 75% derived Acceptance Rate

### `outcomes.csv`

Contains engineering outcome evidence.

The sample includes:

- engineering task cycle time,
- rework rate,
- deployment throughput,
- evidence status,
- attribution method,
- and attribution status.

### `values.csv`

Contains economic value claims derived from those outcomes.

The sample includes:

- engineering capacity value,
- avoided rework cost,
- incremental delivery value.

All three value claims are modeled in this prototype.

### `expected-impact-record.md`

Shows the normalized result expected after combining:

- the Impact Measurement Specification,
- work evidence,
- outcome evidence,
- value evidence,
- and FinOps cost.

## Prototype flow

```text
Impact Measurement Specification
                +
Observed Impact Evidence
                +
FinOps / FOCUS Cost
                ↓
        Measurement Logic
                ↓
           Impact Record
```
