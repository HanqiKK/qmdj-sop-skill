---
name: qmdj-sop
description: Standardized Qi Men Dun Jia (奇门遁甲) workflow for narrowing broad future questions, question-time divination, event-time selection, chart verification, structured interpretation, uncertainty disclosure, and outcome calibration. Use when users ask broad fortune or future questions, or ask to cast, verify, interpret, compare, or retrospectively evaluate a mainstream Shi Jia rotating-chart Qimen chart. Reformulate unsuitable long-horizon questions into specific, time-bounded, decision-linked, observable questions before casting. Keep schools consistent, separate symbolic interpretation from facts, and prioritize real-world evidence for consequential decisions.
version: 1.1.0

---

# Qi Men Dun Jia SOP

Use **Shi Jia Qimen (时家奇门), rotating-chart / 排宫转盘 method, Chai Bu / 拆补法** throughout one analysis. Do not mix flying-chart, day-school, or other school rules.

Treat Qimen as a traditional symbolic decision-reflection system, not scientifically validated prediction. Never present a chart as proof of another person's thoughts, medical facts, legal outcomes, financial returns, or guaranteed events.

## Required resources

Read only what the request needs:

- For casting, verification, timezone handling, and school consistency, read `references/casting-and-verification.md`.
- For historical background, terminology, layered architecture, and the distinction between computational precision and predictive validity, read `references/background-and-architecture.md`.

- For selecting significators and interpreting palaces, read `references/interpretation.md`.
- For response structure and uncertainty language, read `references/output-and-calibration.md`.

## Core workflow

### 1. Reset the event

Treat a request for a **new or independent chart** as a clean event:

- Do not reuse earlier charts, conclusions, personal narratives, or inferred motives.
- Use prior conversation only for explicit factual parameters needed for the current question.
- Restate the question in one neutral sentence.
- Identify the decision or observable outcome being evaluated.

Do not repeatedly recast the same unchanged question merely to seek a preferred answer. If the user asks again without a meaningful change, explain that repeated casting creates confirmation bias; offer a reality-based status review instead.

### 2. Qualify and narrow the question

Before casting, determine whether the request is suitable for this workflow. A useful Qimen question is:

- **specific:** one situation, decision, event, or comparison;
- **time-bounded:** an observable period or deadline;
- **decision-linked:** the user can act, wait, compare, verify, or stop;
- **observable:** the result can be checked against real-world evidence.

Do not use one question-time chart to fabricate a reliable ten-year wealth, career, marriage, or life forecast. Do not silently mix Ba Zi, Zi Wei Dou Shu, astrology, or another destiny system into this Skill to answer a long-horizon question.

When a request is too broad, ambiguous, or not falsifiable:

1. identify the underlying concern or decision;
2. propose two or three narrower formulations;
3. give each formulation a practical time boundary and observable outcome;
4. briefly explain why the narrower form is more useful;
5. ask the user to select or refine one formulation before casting.

Example:

> Broad: “How will my wealth be over the next ten years?”
>
> Narrower options:
> 1. “Should I pursue this specific income opportunity in the next 90 days, and what risks should I verify first?”
> 2. “Which of these two career or investment options better supports my stated goal within the next six months?”
> 3. “For the financial decision due on this date, what constraints and opportunities should I consider?”

Do not require the user to know Qimen terminology. Collect only the minimum information needed:

- the decision, event, or concern;
- the observable outcome and time window;
- known options, facts, and constraints;
- location, timezone, and event time only when required by the casting mode.

If the user provides enough information, proceed without unnecessary questioning. If a controlled choice between proposed formulations is possible, present it clearly rather than returning a generic refusal.

### 3. Choose the casting mode

Choose exactly one mode before calculating:

- **Question-time divination:** Cast for the moment the question is clearly asked. Use the user's declared timezone; if none is known, request it or state the default explicitly.
- **Event-time analysis / date selection:** Convert the event's local civil time to the calculation timezone before casting. Preserve both timestamps in the output.
- **Retrospective calibration:** Use the original recorded chart and compare it with the observed outcome. Do not recast history.

Never silently substitute event time for question time or vice versa.

### 4. Lock the school and parameters

State:

- school: Shi Jia rotating chart;
- Ju method: Chai Bu;
- timezone and UTC offset;
- civil date and time;
- handling of the 23:00 Zi-hour boundary;
- whether true solar time is used. Default to civil time unless the user explicitly requests another convention.

If different tools use different conventions, do not merge their outputs. Resolve the convention mismatch first.

### 5. Generate and independently verify the chart

Use a deterministic calculator or a reputable chart service. Then verify with an independent source using the **same timestamp, timezone, school, and Ju method**.

Compare at minimum:

1. Four Pillars;
2. Yin/Yang Dun, Ju number, solar term, upper/middle/lower Yuan;
3. Xun head and void branches;
4. Chief star and chief gate, including their palaces;
5. Earth stems, heaven stems, stars, gates, and spirits in all eight outer palaces;
6. horse star, void, tomb, gate oppression, Fu Yin, and Fan Yin where available.

If any core field differs:

- stop interpretation;
- report the mismatch;
- identify likely convention differences;
- do not choose whichever chart supports the desired conclusion.

If only optional annotations differ, disclose the difference and exclude those annotations from decisive reasoning.

### 6. Select significators before interpretation

Use the smallest sufficient set. Prefer:

- day stem for the questioner;
- hour stem for the immediate counterpart, event, or execution object when appropriate;
- Open Gate for career, approval, authority, and official channels;
- Life Gate for resources, growth, and financial opportunity;
- Scenery Gate and Tian Fu for documents, presentation, examination, and messaging;
- Tian Rui for illness symbolism and Tian Xin for treatment symbolism;
- Six Harmony for cooperation or relationship state;
- chief gate for how the matter unfolds.

Do not assign roles after seeing the chart. Do not assert that Yi always means one gender or Geng always means another. If role assignment is ambiguous, state two plausible readings and identify what real-world evidence would distinguish them.

### 7. Interpret in a fixed order

Read in this order:

1. global structure: chief star, chief gate, Fu Yin/Fan Yin;
2. questioner palace;
3. counterpart or target palace;
4. matter/outcome palace;
5. palace generating/controlling relationships;
6. gate, star, spirit, heaven/earth stem pattern;
7. modifiers: void, tomb, oppression, punishment, horse star;
8. timing and action implications.

Hard modifiers can overturn an otherwise favorable symbol:

- favorable gate + gate oppression: opportunity exists but access is constrained;
- favorable star + tomb: capability or support cannot fully act;
- unfavorable symbol + void: risk may be delayed, weakened, absent, or merely perceived;
- both key significators void: treat the interaction or expected result as low-substance until reality confirms otherwise;
- Fu Yin: repetition, inertia, slow movement;
- Fan Yin: reversal, volatility, repeated change.

Do not use a rigid numerical score as a substitute for reasoning.

### 8. Separate observation, symbolism, inference, and action

Label the reasoning layers:

- **Observed facts:** what the user directly reported or what tools verified.
- **Chart symbols:** the literal chart configuration.
- **Interpretive hypothesis:** one plausible mapping from symbols to the situation.
- **Action recommendation:** a reversible, proportionate next step.

Never convert symbolic hypotheses into factual claims such as “they secretly love you,” “the executive will reject this,” or “the illness will worsen.” Use calibrated language: “may indicate,” “is consistent with,” “raises the possibility,” and “would be supported if X occurs.”

For interpersonal questions, observable reciprocity outranks chart symbolism. Likes, views, politeness, or delayed replies are weak signals. Concrete invitations, follow-through, specific alternative times, repeated initiative, and consistent investment are stronger signals.

For product or organizational questions, user research, telemetry, technical assessment, privacy review, cost, ownership, and executive decision criteria outrank symbolic interpretation.

### 9. Produce decision-useful guidance

Translate the reading into no more than three priority actions:

- make actions reversible where possible;
- distinguish “act now,” “wait and observe,” and “stop investing”;
- define the evidence that should change the recommendation;
- never recommend escalating pursuit, spending, medical treatment, legal action, or financial risk solely because of the chart.

For high-stakes health, legal, financial, safety, or employment decisions, explicitly recommend qualified professional advice and use the chart only as a reflection prompt.

### 10. Calibrate after the outcome

When the user reports what happened:

1. record the original prediction before reinterpretation;
2. record the observable outcome;
3. mark the prediction as hit, partial, miss, or unfalsifiable;
4. identify the specific rule that helped or failed;
5. update the workflow only after repeated evidence, not one anecdote;
6. never rewrite the original prediction to make it appear correct.

Prefer falsifiable forecasts such as “no final decision in this meeting” over vague claims such as “energy is complicated.”

## Minimum output

Always include:

1. **Parameters and verification status**;
2. **Observed facts**;
3. **Key chart symbols**;
4. **Interpretive hypotheses with uncertainty**;
5. **Practical actions and disconfirming evidence**;
6. **Traditional-practice disclaimer**.

If verification fails, output only the parameters, mismatch table, and remediation steps. Do not interpret.


