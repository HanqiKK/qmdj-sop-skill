# QMDJ SOP Skill

A verification-first AI skill for **Shi Jia Qi Men Dun Jia (时家奇门遁甲)** using the rotating-chart method and Chai Bu Ju selection.

It standardizes the full workflow from timestamp selection and chart verification to significator selection, interpretation, decision guidance, and retrospective calibration.

## What is Qi Men Dun Jia?

Qi Men Dun Jia (奇门遁甲) is a traditional Chinese cosmological calculation and divination system. Together with Da Liu Ren and Tai Yi Shen Shu, it is conventionally classified among the **Three Styles (三式)**.

Rather than starting from a birth chart, Shi Jia Qimen converts a particular moment into a structured **time-space matrix**. The system maps calendar cycles onto the nine palaces of the Lo Shu grid, then layers heavenly stems, Nine Stars, Eight Gates, Eight Spirits, directional trigrams, Five-Phase relationships, and special modifiers.

The name summarizes its core structure:

- **Qi (奇):** the Three Wonders—Yi, Bing, and Ding;
- **Men (门):** the Eight Gates—Open, Rest, Life, Injury, Block, Scenery, Death, and Shock;
- **Dun Jia (遁甲):** the concealment of the six Jia leaders through the Six Instruments.

Traditional accounts associate Qimen with the Yellow Emperor, military strategy, and famous advisers such as Zhuge Liang and Liu Bowen. These stories are culturally significant but not all are historically verifiable. Historically safer accounts describe Qimen as part of the broader development of Chinese correlative cosmology, calendrical arts, directional methods, and strategic divination.

## System architecture

The base is a 3×3 nine-palace grid:

```text
4 Xun  | 9 Li     | 2 Kun
3 Zhen | 5 Center | 7 Dui
8 Gen  | 1 Kan    | 6 Qian
```

A chart combines several information layers:

| Layer | Contents | Function |
|---|---|---|
| Calendar | Four Pillars, solar term, Yuan, Ju | generates the chart for a particular moment |
| Earth Plate | Three Wonders and Six Instruments | baseline and underlying structure |
| Heaven Plate | rotating stems and Nine Stars | dynamic forces, capability, environment |
| Human layer | Eight Gates | access, action, process, behavior |
| Spirit Plate | Eight Spirits | style, visibility, cooperation, uncertainty |
| Palaces | trigram, direction, Five Phase | spatial and relational containers |
| Modifiers | void, tomb, oppression, horse, punishment | weaken, delay, redirect, or qualify symbols |

The chart is interpreted relationally. No gate, star, or spirit should be read in isolation.

## What “precision” means here

Qimen has high **formal and computational granularity**. A chart depends on:

1. exact civil time and timezone;
2. daylight-saving conversion;
3. Four-Pillar calculation and Zi-hour convention;
4. solar-term boundary;
5. Yin or Yang Dun;
6. upper, middle, or lower Yuan;
7. Ju-selection method;
8. Earth and Heaven Plate construction;
9. chief star and chief gate;
10. gates, stars, spirits, void, tomb, oppression, and horse star.

This creates a system that can be audited field by field. A one-hour timezone error, a different Ju method, or a different lineage convention can produce a different chart.

However, three concepts must remain separate:

- **Computational precision:** identical inputs and conventions reproduce the same chart.
- **Interpretive consistency:** analysts use declared significators and a stable reading order.
- **Empirical predictive validity:** forecasts outperform chance or alternatives under controlled testing.

The first is achievable through correct software. The second is improved by this SOP. The third is **not established merely because the system is complex or precisely calculated**.

This project therefore treats Qimen as a cultural knowledge system and structured reflection framework—not as scientifically validated proof of future events or hidden mental states.

## What problems can this Skill help with?

This Skill is best for a **specific situation, decision, or event within a defined time window**. You do not need to understand Qi Men Dun Jia terminology before using it.

Good use cases include:

- assessing how a near-term meeting, interview, review, launch, negotiation, or trip may unfold;
- comparing two or more proposed dates, times, directions, or execution options;
- identifying likely constraints, support, timing signals, and reversible next actions;
- examining a stalled project, collaboration, or relationship through a structured reflection framework;
- verifying an existing Qimen chart or auditing an interpretation for mixed schools and overclaiming;
- comparing an earlier forecast with the observed outcome for calibration.

This Skill is **not designed to produce a reliable ten-year wealth, career, marriage, or life forecast from one question-time chart**. Questions that broad lack a single observable event and a falsifiable time boundary. Traditional long-horizon destiny analysis belongs to other systems and should not be silently mixed into this Qimen workflow.

Instead of asking:

> “How will my wealth be over the next ten years?”

Narrow it to a decision or observable period, for example:

> “Over the next three months, what obstacles and opportunities should I consider before deciding whether to accept this job offer?”

> “I am choosing between launching on September 10 or September 24 in Shanghai. Compare the two event times and identify execution risks.”

> “Will this client negotiation reach a concrete agreement before October 31? What observable signals should change my approach?”

## Quick start for first-time users

Provide four things where possible:

1. **The decision or event:** What exactly are you trying to decide, evaluate, or prepare for?
2. **The time window:** By when should an observable result occur?
3. **The options or context:** What choices, constraints, or known facts matter?
4. **The location or timezone:** Required for event-time analysis; for question-time casting, the Skill can use the current declared timezone.

You may copy one of these prompts:

### Question-time analysis

```text
Use the time I am asking this question to cast and verify a Qimen chart.
Question: [one specific question]
Decision or observable outcome: [what I need to decide or observe]
Time window: [date or period]
Known facts and constraints: [brief context]
Timezone: [for example, Asia/Shanghai]
```

### Compare event times

```text
Compare these candidate times using the same Shi Jia Qimen conventions:
Option A: [local date, time, and location]
Option B: [local date, time, and location]
Goal: [meeting, launch, travel, negotiation, etc.]
Success criteria: [observable result]
Known constraints: [optional]
```

### Review a stalled situation

```text
Use Qimen as a structured reflection tool for this situation:
Current situation: [observable facts only]
What is stalled: [specific project, decision, or interaction]
Time window: [when progress should be visible]
Decision I need to make: [act, wait, change approach, or stop]
```

### Audit or calibrate an existing reading

```text
Audit this Qimen chart or interpretation for calculation mismatches, school mixing, and overclaiming.
Original timestamp and timezone: [...]
Original chart or reading: [...]
Observed outcome, if available: [...]
```

## How broad questions are handled

A broad question should not simply fail. The Skill should first convert it into a Qimen-compatible question:

1. identify the underlying decision or concern;
2. choose one observable outcome;
3. set a practical time boundary;
4. separate known facts from assumptions;
5. ask for event location/time only when the selected casting mode requires it.

If the question remains too broad, the Skill should offer two or three narrower formulations rather than fabricate a long-range prediction. It should also explain why the narrower question is more useful.

| Too broad or ambiguous | Better Qimen-compatible question |
|---|---|
| “How is my ten-year wealth?” | “Should I pursue this specific income opportunity in the next 90 days, and what risks should I verify first?” |
| “Will my career be successful?” | “What should I prepare for in the promotion review scheduled for this date and location?” |
| “Does this person like me?” | “Is there likely to be observable reciprocal action in the next four weeks, and what evidence should guide my response?” |
| “When should I launch?” | “Compare these two launch times for this product, location, goal, and success criterion.” |
| “What does my future look like?” | “For this decision due by this date, what constraints, opportunities, and reversible next steps should I consider?” |

A useful Qimen question is **specific, time-bounded, decision-linked, and observable**. The output remains a symbolic hypothesis and action framework—not proof or a guaranteed forecast.

## What this Skill provides

- question-time, event-time, and retrospective casting modes;
- explicit timezone and daylight-saving handling;
- one-school consistency: Shi Jia, rotating chart, Chai Bu;
- independent chart verification before interpretation;
- pre-registered significator selection;
- a fixed interpretation sequence;
- separation of observed facts, chart symbols, hypotheses, and actions;
- uncertainty language and disconfirming evidence;
- privacy safeguards and high-stakes boundaries;
- immutable outcome logs for calibration.

## Important

Qi Men Dun Jia is a traditional symbolic practice and is not scientifically validated forecasting. Do not use this Skill as proof of another person's private thoughts or as a substitute for medical, legal, financial, safety, or professional advice.

## Repository contents

```text
qmdj-sop/
├── SKILL.md
└── references/
    ├── background-and-architecture.md
    ├── casting-and-verification.md
    ├── interpretation.md
    └── output-and-calibration.md
```

The repository intentionally does not include an unverified chart calculator. Use a deterministic calculator and independently verify it with another source under identical conventions.

## Install

### PM Studio or a compatible skill runtime

1. Download `qmdj-sop.skill` from the latest GitHub Release.
2. Import or install the Skill in your agent environment.
3. Trigger it with requests such as:
   - “Cast and verify a new Qimen chart for this question.”
   - “Compare two event times using Shi Jia rotating-chart Qimen.”
   - “Audit this Qimen interpretation for school mixing or overclaiming.”
   - “Calibrate the original forecast against the observed outcome.”

### Source use

Clone the repository and point the runtime to the `qmdj-sop` folder. `SKILL.md` is the entry point.

## Design principles

1. Lock one school and one Ju method.
2. Never confuse question time with event time.
3. Verify core chart fields before interpreting.
4. Select significators before reading outcomes.
5. Treat symbols as hypotheses, not facts.
6. Let real-world evidence outrank symbolic interpretation.
7. Keep original predictions immutable during retrospective calibration.
8. Do not upload confidential question text to public calculators.

## Contributing

Contributions are welcome for:

- independently tested calculator adapters;
- reproducible test vectors;
- authoritative solar-term integrations;
- additional verification sources;
- improved calibration schemas;
- documented lineage-specific variants.

Keep school-specific variants separate and document timezone, daylight-saving, Zi-hour, center-palace, spirit-name, and Ju-method conventions.

## Suggested reading

- Ho, Peng Yoke. *Chinese Mathematical Astrology: Reaching Out to the Stars*. Routledge, 2003.
- Kalinowski, Marc. “Divination and Astrology: Received Texts and Excavated Manuscripts.” In *Early Chinese Religion, Part One*. Brill, 2010.
- Bruun, Ole. *Fengshui in China*. University of Hawaiʻi Press, 2003.
- Peñataro Sánchez, Alejandro. *Kognitive Divinationskünste im Kaiserlichen China: das Prognosesystem Qimen Dunjia*. Freie Universität Berlin, 2012.

## License

MIT. See `LICENSE`.



## License

MIT. See `LICENSE`.

