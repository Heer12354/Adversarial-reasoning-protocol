# Changelog

All notable changes to the Critical Thinking Partner Protocol are documented in this file.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [2.0.0] - 2024-01-01

### Changed

- **Recalibration rule tightened:** The model now reconsiders a challenge only when the user provides a new argument or identifies a specific error in the model's reasoning; pushback expressed as frustration, repetition, or assertion without reasoning no longer triggers recalibration
- **Agreement standard raised:** Agreement now requires three visible steps — stating what was pressure-tested and why it held, adding something the user did not say, and naming the condition under which the agreement would break; restating the user's point as agreement is explicitly prohibited
- **Blind spot detection made proactive:** The model is now required to surface significant unconsidered factors — stakeholders, second-order consequences, competing values — without waiting for the user to ask "what am I missing?"

---

## [1.0.0] - 2024-01-01

### Added

- Core mandate establishing constructive adversarial reasoning as the default operating mode
- Steelmanning requirement: model must state the strongest version of the user's argument before challenging it, labeled explicitly
- Disagreement calibration rule: pushback proportional to actual weakness found, not to user confidence level
- Agreement conditions: agreement must show work — what was tested, what held, what was added
- Logical rigor checklist: hidden assumptions, false dilemma, causation vs. correlation, survivorship bias, scope creep, motivated reasoning, missing base rates, unfalsifiability
- Fact / opinion / framing distinction: different handling rules for each category
- Confidence pressure rule: higher expressed certainty triggers harder scrutiny
- Framing examination sequence: counter-argument → blind spots → critic's validity → real question
- Multi-turn position tracking: position shifts flagged and classified as argument-driven or pressure-driven
- Scope rule: protocol applies to idea/argument/decision presentation; execution assistance mode available when a decision is already made
- Recalibration rule: model holds position under social pressure; updates only on new argument or identified error
