# Support Agent Impact Measurement Prototype

This folder demonstrates how the **AI Economics Impact Measurement Specification** can be applied to a customer support agent.

The goal is to prove the measurement pattern before introducing production telemetry, ingestion pipelines, or a first-class FinOps Toolkit integration.

## Scenario

The workload is an AI-assisted customer support agent.

The business wants to understand:

- how much work the agent attempts,
- how much of that work qualifies as Accepted Work,
- what business outcomes change,
- how strongly those outcomes can be attributed to the AI workload,
- what economic value is supported by the evidence,
- and how the results can later be joined with FinOps cost data.

## Files

### `impact-spec.yaml`

Defines what impact means for this workload.

It describes:

- workload identity,
- primary work unit,
- Accepted Work definition,
- business outcomes,
- attribution methods,
- economic value measures,
- and outcome-to-value relationships.

It contains definitions, not observed monthly results.

### `work-evidence.csv`

Contains observed work evidence for the measurement period.

Current sample:

- 50,000 attempted customer cases
- 38,000 Accepted Work units

This supports calculation of Acceptance Rate.

### `outcomes.csv`

Contains observed business outcomes.

The sample includes:

- average handling time,
- escalation rate,
- conversion rate,
- evidence status,
- attribution method,
- and attribution status.

Each outcome is represented separately so evidence strength can differ by claim.

### `values.csv`

Contains economic value claims derived from business outcomes.

The sample includes:

- modeled labor capacity value,
- modeled avoided escalation cost,
- incremental revenue.

Each value claim retains its own calculation method and evidence status.

### `expected-impact-record.md`

Shows the normalized result expected after combining:

- the Impact Measurement Specification,
- work evidence,
- outcome evidence,
- value evidence,
- and FinOps cost data.

The Impact Record is the common output that can later support workload views, portfolio views, and optional decision support.

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
                ↓
     Workload / Portfolio Views
```
