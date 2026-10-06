# Cognitive Engineering & Research — A Primer for Newcomers

> **Who this is for:** anyone landing on Project-A4 with zero prior background. You should not need to read a textbook before you can understand what this project is about. By the end of this document, you should be able to follow the rest of the repo's docs, research notes, and code comfortably.

---

## Table of Contents

1. [What Is Cognitive Engineering & Research?](#1-what-is-cognitive-engineering--research)
2. [The Fields This Pulls From](#2-the-fields-this-pulls-from)
3. [Core Concepts You Need to Know](#3-core-concepts-you-need-to-know)
4. [How Research Becomes Engineering](#4-how-research-becomes-engineering)
5. [A Suggested Reading Path (Beginner → Capable)](#5-a-suggested-reading-path-beginner--capable)
6. [Glossary](#6-glossary)
7. [Where to Go Deeper](#7-where-to-go-deeper)

---

## 1. What Is Cognitive Engineering & Research?

**Cognitive engineering** is the practice of designing systems, tools, and interfaces around how the human mind actually works — not how we assume or wish it worked.

Think of it this way:

- A **bridge engineer** designs around the physical properties of steel and concrete — load limits, stress, fatigue.
- A **cognitive engineer** designs around the properties of human thought — attention limits, memory capacity, decision-making biases, reaction time, error patterns.

**Cognitive research** is the scientific side: studying how people actually perceive, remember, decide, and act, usually through controlled experiments, data collection, and modeling.

Put together, **Cognitive Engineering & Research** means: *study how minds really work, then use that evidence to build better tools, interfaces, processes, or models.*

This is intentionally broad — it's less "one field" and more a **practice that draws from several fields at once.**

---

## 2. The Fields This Pulls From

You don't need to master all of these — just recognize them when you see them referenced in this repo.

| Field | What it studies | Example question it answers |
|---|---|---|
| **Cognitive Psychology** | Mental processes: memory, attention, perception, reasoning | "Why do people forget instructions after 20 seconds?" |
| **Cognitive Neuroscience** | The brain activity behind cognition (often via EEG/fMRI) | "Which brain regions activate during decision-making?" |
| **Human Factors / Ergonomics** | How humans interact with systems, safely and efficiently | "Why do pilots miss a particular warning light?" |
| **Human-Computer Interaction (HCI)** | How people use software/interfaces | "Why do users abandon this signup form?" |
| **Behavioral Economics / Decision Science** | How people actually make choices (vs. how they "should") | "Why do people choose the riskier option when framed differently?" |
| **Cognitive Modeling / AI** | Building computational models of thought processes | "Can we simulate how someone solves a puzzle?" |

Project-A4 may touch one, several, or all of these over time — check [`docs/ARCHITECTURE.md`](ARCHITECTURE.md) and [`docs/ROADMAP.md`](ROADMAP.md) for current scope.

---

## 3. Core Concepts You Need to Know

These show up constantly in cognitive research — understanding them unlocks most papers and discussions in the field.

### Cognition
The mental action of acquiring knowledge through thought, experience, and the senses. It's the umbrella term for "thinking" in all its forms: perceiving, remembering, deciding, reasoning, learning.

### Attention
The brain's limited capacity to focus on some information while filtering out the rest. Core finding: humans can only consciously attend to a small amount of information at once — this is *why* interfaces, warnings, and instructions can fail even when technically "correct."

### Memory (Working vs. Long-Term)
- **Working memory** — what you can hold "in mind" right now (very limited, roughly 3–7 items).
- **Long-term memory** — what's stored for later retrieval (effectively unlimited, but retrieval isn't guaranteed).

### Mental Models
The internal, simplified picture a person builds of how something works (a device, a system, another person's intentions). Good design matches the system's real behavior to the user's mental model; mismatches cause errors.

### Cognitive Load
The total amount of mental effort being used in working memory at a given moment. Overload leads to mistakes, slower decisions, and missed information — a central concern in both research and design.

### Heuristics & Biases
Mental shortcuts people use to make fast decisions (heuristics), which can lead to predictable errors (biases). Example: people tend to overestimate risks that are vivid or recent (*availability heuristic*).

### Human Error vs. System Error
A foundational idea in human factors: when something goes wrong, the *system* is usually a bigger factor than individual carelessness. Good cognitive engineering designs systems that are forgiving of normal human limitations, rather than just blaming the user.

---

## 4. How Research Becomes Engineering

This is the core loop that connects the "Research" and "Engineering" sides of this repo (see [`/research`](../research) and [`/src`](../src)):

```
 Observe & Study            Extract Principle           Build & Test
 ───────────────            ──────────────────          ────────────
 Run an experiment     →    "Users miss alerts     →    Design an alert
 or review existing         placed outside their        system that uses
 literature on a                central vision"          central-vision
 cognitive phenomenon                                    placement + sound

                                     ↓
                            Document the finding
                            under /research with
                            sources cited
                                     ↓
                            Reference it when
                            building anything
                            under /src
```

Every tool or implementation in this repo should, ideally, trace back to a documented finding — not just intuition. That traceability is part of what makes this a *research-grounded* engineering project rather than a guesswork one.

---

## 5. A Suggested Reading Path (Beginner → Capable)

If you have genuinely zero background, here's a reasonable order to build it up — no need to rush, and you don't need to finish this before contributing small things.

1. **Start conceptual, not technical.** Read a plain-language overview of cognitive psychology (any reputable intro source — university lecture notes, Wikipedia's "Cognitive psychology" overview, or similar) just to get comfortable with the vocabulary in [Section 3](#3-core-concepts-you-need-to-know).
2. **See it in action.** Browse a few real datasets or studies (see [Section 7](#7-where-to-go-deeper)) to see what "data" looks like in this field — it grounds the abstract concepts.
3. **Read one real paper, slowly.** Pick a short, approachable paper from OSF or Google Scholar on a topic you're curious about (e.g. "attention and interface design"). Don't worry about understanding every statistic — focus on: what question did they ask, what did they find, why does it matter.
4. **Connect it to engineering.** Look at how HCI/human-factors guidelines (e.g., Nielsen Norman Group's usability articles) translate research findings into concrete design rules.
5. **Start contributing small.** Document a finding, fix a doc typo, or ask a clarifying question in an issue — you don't need to be an expert to start participating.

---

## 6. Glossary

| Term | Meaning |
|---|---|
| **Cognition** | Mental processes involved in acquiring and using knowledge |
| **EEG** | Electroencephalography — measures electrical brain activity via scalp sensors |
| **fMRI** | Functional MRI — measures brain activity via blood flow changes |
| **Working memory** | Short-term, limited-capacity mental "workspace" |
| **Cognitive load** | Mental effort currently being used |
| **Heuristic** | A mental shortcut used to make fast judgments |
| **Bias (cognitive)** | A systematic, predictable deviation from rational judgment |
| **Mental model** | A person's internal, simplified understanding of how something works |
| **Human factors** | The study of how humans interact with systems, tools, and environments |
| **Reproducibility** | The ability for others to repeat a study/experiment and get consistent results |

---

## 7. Where to Go Deeper

Once you're past the basics, these are real, open resources referenced elsewhere in this project:

- [OpenCogData (NIMH)](https://github.com/nimh-dsst/opencogdata) — real, open cognitive task datasets, good first stop
- [Open Science Framework (OSF)](https://osf.io) — raw data and materials from published cognitive/behavioral studies
- [OpenNeuro](https://openneuro.org) — open brain imaging data (EEG/fMRI), once you're ready for the neuroscience side
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/) — approachable behavioral/decision-making datasets

For contribution standards once you're ready to add your own research or notes, see [`CONTRIBUTING.md`](../CONTRIBUTING.md) and [`research/README.md`](../research/README.md).

---

*This primer is a living document — if something here is unclear to a genuine beginner, that's a bug. Open an issue or a PR to improve it.*
