# Casting and verification

## Table of contents

- Casting modes
- Timezone rules
- School lock
- Verification checklist
- Mismatch handling
- Tool assessment

## Casting modes

### Question time

Use the exact moment the question becomes clear. Record timezone and UTC offset. A chart is valid for the question as framed at that moment; materially different questions require a fresh chart.

### Event time and date selection

Use the event location's civil time as the source timestamp, then convert it explicitly to the calculator's timezone. Show both timestamps. Account for daylight-saving time using an IANA timezone such as `America/Los_Angeles`; do not assume a fixed offset throughout the year.

Date selection requires the **actual expected event hour**. A noon placeholder cannot determine the quality of a morning or afternoon event because Qimen changes by two-hour branch.

### Retrospective review

Preserve the original chart. Compare the original forecast with observable outcomes. Do not recast after learning the result.

## Time boundaries

- State whether 23:00 begins the next day for day-pillar purposes.
- Use civil time by default.
- Use true solar time only if explicitly requested and consistently supported by both calculators.
- On solar-term transition days, obtain an authoritative solar-term timestamp; approximate astronomy code is insufficient near the boundary.

## School lock

Use only:

- Shi Jia Qimen;
- rotating-chart / 排宫转盘;
- Chai Bu / 拆补 Ju selection.

Do not combine annotations from flying-chart, Zhi Run, Mao Shan, day-school, or custom lineage methods unless producing an explicit comparison. In a comparison, keep each chart separate.

## Verification checklist

Create a table with columns `field`, `source A`, `source B`, and `status`.

Core fields:

- civil timestamp and timezone;
- Four Pillars;
- solar term and Yuan;
- Yin/Yang Dun and Ju;
- Xun head and void;
- chief star and palace;
- chief gate and palace;
- eight outer-palace heaven stems;
- eight outer-palace earth stems;
- gates;
- stars;
- spirits.

Optional fields:

- hidden stems;
- twelve growth stages;
- horse star;
- tomb;
- gate oppression;
- punishment;
- named stem combinations.

Pass only when all core fields match.

## Mismatch handling

Common causes:

1. wrong timezone or daylight-saving conversion;
2. question time confused with event time;
3. different Ju method;
4. different 23:00 day boundary;
5. rotating chart versus flying chart;
6. center-palace hosting differences;
7. solar-term boundary approximation;
8. spirit naming variants such as Bai Hu/Gou Chen and Xuan Wu/Zhu Que.

When core fields differ, stop. Report the mismatch and ask the user to select conventions if necessary.

## Assessing calculators

Prefer tools that disclose:

- school and Ju method;
- timezone behavior;
- Four Pillars and solar term;
- complete palace data;
- reproducible output or JSON;
- version or source code;
- no requirement to expose personal questions.

Do not hard-code a third-party website as an authority. Services can change, disappear, or implement undisclosed conventions. Treat them as independent checks, not ground truth.

Do not send confidential question text to a public calculator. Only transmit the timestamp and non-sensitive calculation parameters required for chart generation.
