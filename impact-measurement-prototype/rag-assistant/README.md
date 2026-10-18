# RAG Assistant Impact Measurement Prototype

This folder applies the same **AI Economics Impact Measurement Specification** used by the support-agent and coding-agent prototypes to an enterprise RAG / knowledge-assistant workload.

The goal is to test whether the measurement model remains reusable when the primary work unit is less tangible than a customer case or engineering task.

## Scenario

The workload is an enterprise knowledge assistant answering user questions using retrieval-augmented generation.

The business wants to understand:

- how many questions the assistant attempts,
- how many answers meet the Accepted Work definition,
- whether users complete tasks more successfully,
- whether time and escalation decrease,
- what economic value can reasonably be modeled,
- and how those results relate to FinOps cost.

## Files

### `impact-spec.yaml`

Defines:

- workload identity,
- user question as the primary work unit,
- Accepted Work criteria,
- business outcomes,
- attribution methods,
- economic value measures,
- and outcome-to-value relationships.

### `work-evidence.csv`

Contains work evidence for the measurement period.

Current sample:

- 20,000 attempted user questions
- 15,000 Accepted Work units
- 75% derived Acceptance Rate

### `outcomes.csv`

Contains outcome evidence for:

- task completion rate,
- time to answer,
- escalation rate,
- evidence status,
- attribution method,
- and attribution status.

### `values.csv`

Contains modeled value claims for:

- employee productivity,
- avoided escalation cost,
- task completion improvement.

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
