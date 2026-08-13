# Contributing

> **Canon layer:** 3 — Surface · **Doctrine version:** 1.0.0 · Amendment rules: [EVOLUTION.md](EVOLUTION.md)

This repository is a living doctrine: a text that other systems treat as their highest-priority reference. That fact sets the bar for contributions. Changes here do not merely edit prose; they change the behavior of every agent pointed at this repo. Contribute the way you would contribute to a navigation chart that ships are already steering by.

## The spirit

Two commitments govern everything in this repo, and they govern contributions too:

1. **Truth as steering.** A change must make the map more accurate or more usable, and the case for it must be honest — including honesty about weak evidence.
2. **Operational love.** A change must treat the project, its users, and the agents it governs as improvable and worth improving. Demolition without a better proposal, and cleverness that serves the contributor rather than the reader, both fail this test.

The doctrine itself demands its own improvability ([DOCTRINE.md §9](DOCTRINE.md)). Contributions are not an imposition on the canon; they are how the canon stays alive. But improvability is not the same as malleability — the amendment process exists so the text can change without losing its center.

## What is welcome

In rough order of value:

- **Field reports.** Traces of a Shaman behaving badly (or unexpectedly well) under the current canon, with enough context to diagnose. These are the most valuable contribution and require no writing skill. Open an issue with the trace, what you expected, and what happened.
- **Evidence upgrades.** Better citations, corrections of misstated research, replication failures for studies the toolkit leans on.
- **New failure modes** for the intervention guide, with diagnostic signals observed in real systems — not hypothesized ones.
- **New examples** meeting the quality bar in [EXAMPLES/README.md](EXAMPLES/README.md).
- **Prompt improvements** with before/after behavior, not before/after aesthetics.
- **Translations and platform adapters** (integration notes for orchestration frameworks).
- **Doctrine amendments** — welcome, and held to the highest standard. Read [EVOLUTION.md](EVOLUTION.md) first.

## What will be declined

- Changes that soften the core to broaden appeal. The two operators are load-bearing; a version of this project without them is a different project, and forking is the honest way to build it.
- Inspirational language. If a sentence would survive on a motivational poster, it does not survive here.
- Additions that grow the canon without increasing its resolving power. The doctrine competes for context-window space in running agents; every added word must pay rent.
- Psychological techniques without sourcing, or with sourcing that misrepresents the evidence.
- Changes that make the Shaman a doer. See DOCTRINE.md §7 — this is anchored.

## Process

1. For anything above a typo, **open an issue first** describing the defect you intend to fix. "Defect" is defined in the PR template.
2. Check which **canon layer** your change touches and read the matching section of [EVOLUTION.md](EVOLUTION.md). Higher layers require more evidence and more patience.
3. Open the PR using the template. Run the **canary questions** (EVOLUTION.md) against your amended text and report the result honestly.
4. Expect adversarial review. The review is aimed at the text, not at you; that distinction is itself doctrine ([PSYCHOLOGY_TOOLKIT.md](PSYCHOLOGY_TOOLKIT.md), attribution).

## Style

- Precise over vivid. Serious over solemn. Plain over ornamental — the name "Shaman" is the only ornament this project needs.
- No hype, no emoji, no exclamation marks in canon files.
- Load-bearing claims get short sentences and, where they are doctrine, numbered clauses.
- Every empirical claim in method files carries a source. Where the evidence is contested, say so in place.
- Write for two readers at once: the human maintainer and the agent that will load this file as operating instructions. Ambiguity that a human would shrug off can become behavior in an agent.

## License

By contributing, you agree that your contributions are licensed under the repository's [MIT license](LICENSE).
