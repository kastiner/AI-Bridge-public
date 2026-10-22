# Synthetic example — apparent disagreement caused by measurement definitions

## Scenario

A computational researcher reports that marker X is "absent" because its normalized value is zero. An experimental researcher interprets "absent" as evidence that the protein is not present.

## Interpretation gap

| Perspective | Initial interpretation | Missing clarification |
|---|---|---|
| Computational | No transcript counts were observed after preprocessing | Detection threshold, filtering, and dropout |
| Experimental | The biological product is absent | Transcript measurement does not directly establish protein absence |

## Useful LLM role

- Rewrite the claim as a measurement statement.
- List the assumptions required to move from transcript non-detection to protein absence.
- Draft questions for both disciplines.

## Human decision

The participants decide which additional measurement, if any, is required. The LLM does not decide that the biological entity is absent.

## Reusable rule

Translate claims back to the measurement that produced them before debating their biological meaning.
