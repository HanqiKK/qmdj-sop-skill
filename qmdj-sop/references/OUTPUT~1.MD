# Output and calibration

## Table of contents

- Standard output
- Uncertainty language
- Action design
- Outcome log
- Safety and privacy

## Standard output

Use this structure:

```markdown
# Qimen analysis: <neutral question>

## Parameters and verification
| Field | Value |
|---|---|
| Casting mode | Question time / Event time / Retrospective |
| Local timestamp | ... |
| Calculation timestamp | ... |
| School | Shi Jia rotating chart, Chai Bu |
| Verification | Passed / Failed / Partial |

## Observed facts
- Facts supplied by the user only.

## Key chart symbols
- Literal placements without interpretation.

## Interpretive hypotheses
- Hypothesis A — confidence: low/medium/high; supporting symbols; contrary evidence.
- Hypothesis B — confidence: low/medium/high; supporting symbols; contrary evidence.

## Recommended actions
1. Reversible next step.
2. Evidence to collect.
3. Stop/continue criterion.

## What would change this view
- Observable disconfirming evidence.

> Traditional symbolic practice; not a scientific forecast or substitute for professional advice.
```

If verification fails, omit interpretation and actions based on the chart.

## Uncertainty language

Use:

- “is consistent with”;
- “raises the possibility”;
- “one plausible reading”;
- “confidence is low/medium/high because…”;
- “this would be supported if…”;
- “this would be contradicted if…”.

Avoid:

- “definitely”;
- “the chart proves”;
- “they secretly think”;
- “this will happen”;
- fabricated percentages.

## Action design

A useful recommendation has:

- owner;
- timing;
- reversible scope;
- success signal;
- stop condition.

Example:

> Run five target-user interviews before adding scope. Continue only if at least three independently describe the same high-frequency pain point; otherwise revise the hypothesis.

For interpersonal situations:

> Make one clear, respectful invitation with a specific time. Treat acceptance, a concrete alternative, or later initiative as positive evidence. Treat repeated vagueness or non-response as insufficient reciprocity and stop pursuing.

## Outcome log

Record each forecast in CSV or JSON with:

- case ID;
- original timestamp and timezone;
- question;
- school and parameters;
- verification sources and status;
- pre-outcome prediction;
- expected observation and deadline;
- actual observation;
- rating: hit / partial / miss / unfalsifiable;
- rule that helped or failed;
- proposed change.

Never edit the original prediction after the outcome. Append a retrospective note.

Only promote a heuristic after multiple independent cases. One anecdote is not enough.

## Safety and privacy

- Do not upload the user's confidential question, names, company data, health details, or relationship history to public calculators.
- Use timestamps and non-sensitive parameters only.
- Remove personal data before publishing examples or calibration logs.
- For medical, legal, financial, employment, or safety matters, recommend qualified professional advice.
- Do not use Qimen to diagnose, surveil, manipulate, or make claims about non-consenting third parties.
