# Background and system architecture

## Table of contents

- What Qi Men Dun Jia is
- Historical background
- Meaning of the name
- The nine-palace model
- Time-to-chart transformation
- Information layers
- Why the system feels precise
- Precision versus predictive validity
- Sources and further reading

## What Qi Men Dun Jia is

**Qi Men Dun Jia (奇门遁甲)** is a traditional Chinese cosmological calculation and divination system. It is conventionally grouped with Da Liu Ren (大六壬) and Tai Yi Shen Shu (太乙神数) as one of the **Three Styles (三式)**.

Its distinctive feature is the conversion of a specific moment into a structured **time-space matrix**. A 3×3 Lo Shu grid represents nine palaces and eight directions. Calendar cycles then determine the placement of symbolic layers such as heavenly stems, stars, gates, and spirits. Practitioners interpret the relationships among those layers as a model of situational structure, constraints, timing, and possible action.

Qimen is therefore better described as a traditional **situational and strategic interpretation framework** than as a natal horoscope. It focuses on a moment, a question, an event, a direction, or a decision rather than attempting to describe an entire life from birth data.

## Historical background

Traditional legends connect Qimen with the Yellow Emperor, Jiutian Xuannü, military campaigns, and later strategists such as Zhang Liang, Zhuge Liang, and Liu Bowen. These stories are culturally important but should not be presented as verified history.

Historically safer claims are more modest:

- Chinese correlative cosmology involving yin-yang, the Five Phases, stems and branches, directions, and calendar cycles developed over long periods, with important precedents visible by the Warring States and Han eras.
- Textual references to Dun Jia methods appear in medieval bibliographies and writings; multiple Dun Jia texts circulated by the Sui and Tang periods.
- Qimen became strongly associated with military strategy, statecraft, calendrical offices, travel direction, timing, and situational assessment.
- Later transmission produced multiple schools and conventions, including rotating-chart and flying-chart methods, Shi Jia and other time scales, and different Ju-selection rules.
- Modern practice extends the framework to personal decisions, business questions, project strategy, date selection, and reflective consultation.

This Skill does not claim a single unbroken or historically uniform lineage. It deliberately locks one operational convention—**Shi Jia, rotating chart, Chai Bu**—to ensure internal consistency.

## Meaning of the name

The name encodes three structural ideas:

- **Qi (奇):** the Three Wonders—Yi (乙), Bing (丙), and Ding (丁).
- **Men (门):** the Eight Gates—Open, Rest, Life, Injury, Block, Scenery, Death, and Shock.
- **Dun Jia (遁甲):** “concealed Jia.” The six Jia leaders are represented through the Six Instruments rather than displayed as an independent tenth stem in the nine-palace allocation.

A commonly used concealment mapping is:

| Jia leader | Concealed in |
|---|---|
| Jia-Zi 甲子 | Wu 戊 |
| Jia-Xu 甲戌 | Ji 己 |
| Jia-Shen 甲申 | Geng 庚 |
| Jia-Wu 甲午 | Xin 辛 |
| Jia-Chen 甲辰 | Ren 壬 |
| Jia-Yin 甲寅 | Gui 癸 |

The Three Wonders plus the Six Instruments yield nine symbols, matching the nine-palace framework.

## The nine-palace model

The base is the Lo Shu nine-palace arrangement:

```text
4 Xun  | 9 Li   | 2 Kun
3 Zhen | 5 Center | 7 Dui
8 Gen  | 1 Kan  | 6 Qian
```

Each outer palace has stable correspondences such as direction, trigram, and Five-Phase category. The center is handled according to the selected lineage convention; in rotating-chart methods, center-related symbols may be hosted in another palace.

The grid is not merely a list of good and bad directions. It functions as a relational map. Interpretation compares:

- where each selected significator falls;
- which palace generates or controls another;
- whether a symbol is seasonally strong or weak;
- whether an apparently favorable symbol is void, in tomb, oppressed, or otherwise constrained;
- whether the whole chart is static (Fu Yin) or reversing (Fan Yin).

## Time-to-chart transformation

A reproducible chart requires a deterministic sequence:

1. Resolve the civil timestamp and timezone.
2. Convert to the Four Pillars using a declared day-boundary convention.
3. Locate the relevant solar term.
4. Determine Yin or Yang Dun.
5. Determine upper, middle, or lower Yuan under the chosen Ju method.
6. Select one of the nine Yin or nine Yang Ju patterns.
7. Arrange the Three Wonders and Six Instruments on the Earth Plate.
8. Determine the Xun head and the concealed Jia instrument.
9. Identify the chief star and chief gate.
10. Rotate or place heaven stems, stars, gates, and spirits according to the locked school.
11. Mark void, horse star, tomb, gate oppression, Fu Yin, Fan Yin, and other modifiers.

Every step is convention-sensitive. A one-hour timezone error, daylight-saving omission, solar-term boundary error, different Zi-hour rule, or different Ju method can produce a different chart. This is why reproducibility requires publishing the calculation conventions—not only the final grid.

## Information layers

A mainstream rotating-chart representation commonly includes:

| Layer | Typical contents | Interpretive role |
|---|---|---|
| Earth Plate | Three Wonders and Six Instruments | baseline, ground condition, underlying structure |
| Heaven Plate | rotating stems and Nine Stars | dynamic forces, capability, timing, environment |
| Human layer | Eight Gates | access, behavior, process, action channel |
| Spirit Plate | Eight Spirits | style, visibility, cooperation, uncertainty, pressure |
| Palace | trigram, direction, Five Phase | spatial and relational container |
| Calendar | Four Pillars, solar term, Yuan, Ju | time index generating the chart |
| Modifiers | void, tomb, oppression, punishment, horse | constraints that can weaken, delay, or redirect a symbol |

The chart is read relationally. A gate is not interpreted in isolation; its palace, seasonal strength, star, spirit, stem combination, and modifiers all matter.


## Why the system feels precise

Qimen has a high degree of **formal granularity**:

- a moment is indexed by multiple nested cycles;
- a finite set of symbols is placed through deterministic rules;
- every symbol has positional and relational dependencies;
- modifiers can qualify or reverse a superficial reading;
- the same chart can be audited field by field;
- differences between calculators can often be traced to explicit conventions.

This makes Qimen more structurally elaborate than an unstructured intuition exercise. Its precision can be improved operationally through:

1. explicit timezone and daylight-saving conversion;
2. authoritative solar-term timestamps near boundaries;
3. locked school and Ju conventions;
4. deterministic code with unit tests;
5. independent chart comparison;
6. pre-registered significators;
7. falsifiable forecasts;
8. immutable outcome logs and calibration.

## Precision versus predictive validity

Do not confuse three different properties:

| Property | Meaning | Qimen status |
|---|---|---|
| Computational precision | The same inputs and conventions reproduce the same chart | achievable with correct algorithms |
| Interpretive consistency | Analysts follow the same declared reading order and role rules | improvable through an SOP |
| Empirical predictive validity | Forecasts outperform chance or alternatives under controlled testing | not established by the system's complexity alone |

A chart can be calculated precisely while its interpretation remains subjective. A richly structured symbolic system is not automatically a scientifically validated predictor.

For this reason, this Skill treats Qimen as:

- a cultural and historical knowledge system;
- a structured prompt for situational reflection;
- a way to generate competing hypotheses and action options;
- a framework that must be checked against observable evidence.

It does **not** treat Qimen as proof of hidden mental states, guaranteed outcomes, medical diagnoses, or financial certainty.

## Sources and further reading

Use sources critically and distinguish history from traditional attribution.

- Ho, Peng Yoke. *Chinese Mathematical Astrology: Reaching Out to the Stars*. Routledge, 2003.
- Kalinowski, Marc. “Divination and Astrology: Received Texts and Excavated Manuscripts.” In *Early Chinese Religion, Part One*, Brill, 2010.
- Bruun, Ole. *Fengshui in China: Geomantic Divination Between State Orthodoxy and Popular Religion*. University of Hawaiʻi Press, 2003.
- Peñataro Sánchez, Alejandro. *Kognitive Divinationskünste im Kaiserlichen China: das Prognosesystem Qimen Dunjia*. Freie Universität Berlin, 2012.
- “Qimen Dunjia,” English Wikipedia. Use as an orientation page and follow its cited scholarly sources rather than treating it as a primary authority.
- “奇门遁甲,” Chinese Wikipedia. It explicitly carries accuracy and expansion warnings; use only for terminology cross-checking.

