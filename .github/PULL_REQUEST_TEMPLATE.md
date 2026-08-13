<!-- This repository is a living doctrine. Pull requests are amendments.
     Read CONTRIBUTING.md and EVOLUTION.md before opening one. -->

## What this changes

<!-- One paragraph. What does this change, and what defect in the current canon does it correct?
     "Defect" includes: factual error, internal inconsistency, vagueness that has caused
     misbehavior in practice, missing coverage, and better evidence than what the text rests on. -->

## Canon layer touched

<!-- Check the highest (most protected) layer your change touches.
     See EVOLUTION.md for what each layer requires. -->

- [ ] Layer 3 — Surface (`EXAMPLES/`, `README.md`, `DESIGN_RATIONALE.md`, tooling, wording fixes)
- [ ] Layer 2 — Method (`PROMPT.md`, `INTERVENTION_GUIDE.md`, `PSYCHOLOGY_TOOLKIT.md`, `MULTI_AGENT.md`)
- [ ] Layer 1 — Doctrine (`DOCTRINE.md` body, core `GLOSSARY.md` definitions)
- [ ] Layer 0 — Core (anchored clauses, marked ⚓ in `DOCTRINE.md`) — follow the full process in EVOLUTION.md before opening this PR

## Evidence

<!-- What supports this change? In descending order of weight:
     1. Interaction traces showing the current text producing bad behavior (attach or link)
     2. Published research (cite it)
     3. Operational experience described concretely
     4. Argument from the doctrine's own principles
     Layer 1 and above require evidence of type 1-3, not taste. -->

## Canary check

- [ ] I re-read the canary questions in EVOLUTION.md and answered each one under the amended text.
- [ ] All canaries still pass.
- [ ] *(or)* A canary fails, and this PR explicitly proposes revising that canary through the Layer 0 process.

## Consistency

- [ ] Terms are used as defined in `GLOSSARY.md` (or the glossary is updated in this PR).
- [ ] Cross-references between files remain correct.
- [ ] The tone rules hold: precise, serious, no hype, no filler.
