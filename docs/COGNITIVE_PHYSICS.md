# Cognitive Physics — A Primer for Newcomers

> **Who this is for:** anyone with zero background who wants to understand what "Cognitive Physics" means in the context of this project. This document is honest about where the field stands: **it is not yet one single, standardized academic discipline** the way "cognitive psychology" or "thermodynamics" are. It's an emerging, cross-disciplinary space. This doc explains the real threads that exist, so you can engage with the idea seriously rather than being misled about its maturity.

---

## Table of Contents

1. [What People Mean by "Cognitive Physics"](#1-what-people-mean-by-cognitive-physics)
2. [The Two Real Threads Behind the Term](#2-the-two-real-threads-behind-the-term)
3. [Core Concepts Borrowed from Physics](#3-core-concepts-borrowed-from-physics)
4. [Why Apply Physics Thinking to Cognition at All?](#4-why-apply-physics-thinking-to-cognition-at-all)
5. [A Suggested Reading Path](#5-a-suggested-reading-path)
6. [Glossary](#6-glossary)
7. [An Honest Note on Where This Stands](#7-an-honest-note-on-where-this-stands)

---

## 1. What People Mean by "Cognitive Physics"

When people use the term "cognitive physics," they're usually pointing at one (or both) of two ideas:

1. **Using the mathematics of physics to model the mind** — treating thought, attention, memory, and decision-making as *dynamical systems*, the same way physicists model weather systems, pendulums, or fields. This gives cognition quantitative, predictive structure instead of only qualitative description.
2. **Studying how humans cognitively understand physics itself** — e.g., why intuitive physics (how a thrown ball "should" move) often differs from real physics, and what that reveals about the mind.

Project-A4 is primarily interested in the **first** sense: physics-style formal modeling applied *to* cognition, not the study of physics education.

---

## 2. The Two Real Threads Behind the Term

To avoid vagueness, here are the actual named efforts in this space, so you have real anchors rather than a fuzzy concept.

### Thread A: Dynamical-Systems & Field-Theoretic Models of Cognition
A growing body of work treats cognitive processes as **fields** or **dynamical systems** — similar to how physicists describe a magnetic field or a fluid flow — rather than as discrete symbolic steps.

- **Cognitive Field Theory** — recent research formulates cognition as the collective dynamics of a large interacting system, borrowing tools from statistical mechanics (e.g., modeling memory and attention using concepts like relaxation rates, coupling, and field amplitude/phase, much like physicists describe oscillating or dissipative systems).
- **The Free Energy Principle** (Karl Friston and collaborators) — a influential framework modeling brain function as a system that minimizes "surprise" or prediction error, directly borrowing the mathematics of statistical thermodynamics (free energy, entropy).
- **Dynamical Systems Theory in Cognitive Science** — a long-standing approach (going back decades) that models cognition using concepts like *attractor states*, *phase space*, and *stability*, rather than step-by-step symbolic logic.

### Thread B: "Cognitive Physical Science"
A smaller, distinct effort (notably from the University of Pretoria's Physics Department) studies the reverse direction: **how findings from cognitive science should inform our understanding of physics itself** — essentially asking whether physical science can be fully understood without accounting for the neural/cognitive processes of the humans doing the observing and theorizing.

> **Why this matters for you:** if you see the term "cognitive physics" used elsewhere, check which thread it means — they're related but answer different questions. Project-A4's use leans toward **Thread A**.

---

## 3. Core Concepts Borrowed from Physics

These are the physics ideas that get reused, metaphorically or mathematically, when modeling cognition this way.

### Dynamical System
Any system whose state evolves over time according to a fixed rule. A pendulum is a dynamical system; so, in this framework, is a mind moving between mental states.

### Phase Space
An abstract space where every possible state of a system is a single point. Plotting how a system moves through phase space reveals patterns (like settling into a stable loop) that aren't obvious from raw data alone.

### Attractor State
A state (or pattern of states) that a system tends to settle into over time, even from different starting points — like a ball rolling into a valley. In cognitive modeling, a recurring thought pattern or habitual decision can be described as an attractor.

### Entropy / Free Energy
Borrowed from thermodynamics: a measure of disorder, uncertainty, or "surprise." The Free Energy Principle proposes brains work to minimize this quantity — essentially, to make the world feel as predictable as possible.

### Field
In physics, a field assigns a value (like temperature or force) to every point in space. In Cognitive Field Theory, a "cognitive field" is a collective, continuous quantity representing the aggregate state of many interacting mental processes, rather than one discrete variable.

### Non-equilibrium System
A system that is not settled into a stable, unchanging state — it's actively exchanging energy or information with its environment. Minds are almost always modeled this way, since cognition is constantly responding to new input.

---

## 4. Why Apply Physics Thinking to Cognition at All?

Three honest reasons this approach is attractive, and one honest limitation:

- **Precision**: Physics-style models force exact, quantitative, falsifiable predictions — not just descriptive stories.
- **Continuity**: Cognition doesn't happen in discrete steps; it flows. Dynamical systems math is built for exactly that kind of continuous change.
- **Cross-pollination**: Decades of extremely well-developed mathematical tools already exist in physics — reusing them avoids reinventing the wheel.
- **Limitation (be honest about this)**: these models are often highly abstract and mathematically heavy, and empirical validation is an active, ongoing research challenge — not a solved problem. Treat claims in this space as *promising frameworks*, not settled fact, until you've checked the primary sources.

---

## 5. A Suggested Reading Path

1. **Build the cognitive science foundation first.** If you haven't yet, read [`docs/PRIMER.md`](PRIMER.md) — you need the basic vocabulary of cognition before the physics analogies make sense.
2. **Get comfortable with "dynamical systems" as a concept**, independent of cognition — any plain-language introduction to dynamical systems or chaos theory will do. You don't need the full math yet, just the intuition (states, trajectories, attractors).
3. **Read about the Free Energy Principle** at a conceptual level — it's the most well-established, widely cited bridge between physics-style thinking and brain function.
4. **Sample a Cognitive Field Theory paper's abstract and introduction only** (skip the heavy equations at first) — just to see how the vocabulary from Section 3 gets used in practice.
5. **Stay skeptical and curious.** This is an active research frontier, not a textbook subject — forming your own judgment about which models hold up is part of genuinely engaging with it.

---

## 6. Glossary

| Term | Meaning |
|---|---|
| **Dynamical system** | A system whose state changes over time according to a defined rule |
| **Phase space** | An abstract space representing every possible state of a system |
| **Attractor** | A state a system tends to settle into over time |
| **Entropy** | A measure of disorder or uncertainty in a system |
| **Free energy** (in this context) | A quantity some models propose the brain minimizes to reduce "surprise" |
| **Field** | A quantity defined across every point in a space (borrowed from physics, applied metaphorically/mathematically to collective cognitive states) |
| **Non-equilibrium system** | A system actively exchanging energy/information with its environment, not in a static steady state |
| **Relaxation rate** | How quickly a system returns to a stable state after a disturbance |

---

## 7. An Honest Note on Where This Stands

To respect both newcomers and the integrity of the research:

- "Cognitive Physics" is **not** a field you'll find as a standard university department or a settled textbook subject — don't present it to others (or build on it internally) as more established than it is.
- It **is** a real, active area where serious researchers are applying physics-grade mathematical tools to cognition, with genuine published work (cited above).
- Any content Project-A4 produces under this heading should clearly distinguish **established, peer-reviewed findings** (e.g., core dynamical-systems theory, the Free Energy Principle) from **newer, less-validated proposals** (e.g., specific Cognitive Field Theory formulations) — see [`CONTRIBUTING.md`](../CONTRIBUTING.md) for how this project expects research claims to be sourced and labeled.

*If you contribute content here, keep this honesty standard intact — it's what keeps this repo trustworthy as the field itself matures.*
