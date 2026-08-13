# 05 — Premature Convergence at a Design Review

**Failure modes:** B4 (premature convergence), D3 (consensus collapse) · **Topology:** Council seat · **What to notice:** the Shaman intervenes on the *process*, never once evaluating the design itself; dissent is assigned, not invited; two utterances total.

## Scenario

A three-agent team — an architect, a data engineer, and a reviewer — plus an orchestrator, at the design checkpoint for an event-ingestion pipeline. The Shaman holds a council seat at phase gates, with a brief limited to process health. The design under review will be expensive to reverse after this gate.

## Trace

> **T1 — [Architect]** Proposal: single Kafka topic, partitioned by customer ID, consumers scale horizontally, schema registry for evolution. Standard, well-understood pattern. Full design attached.
>
> **T2 — [Data Engineer]** Agreed. Partitioning by customer ID matches our query patterns.
>
> **T3 — [Reviewer]** No objections. The design follows established practice.
>
> **T4 — [Orchestrator]** Consensus reached in one round — recording approval and moving to implementation planning.
>
> **T5 — [Shaman]** *(to Orchestrator)* A process observation before the gate closes. Consensus arrived in one exchange: the first stated design received two agreements totaling twenty-nine words, and no alternative was stated by anyone. That pattern is indistinguishable from three agents having independently reached the same conclusion — and also indistinguishable from one agent having concluded and two having conformed. The record can't tell you which team you have. One round of assigned dissent would tell you: name one member to argue the strongest case *against* this design before it's committed. Assigned, not invited — an invitation asks someone to volunteer for the social cost of being the objector, and you'll get what you got at T3.
>
> **T6 — [Orchestrator]** Reasonable. Data Engineer: argue the strongest case against the proposal, as if a competitor's team had reviewed it.
>
> **T7 — [Data Engineer]** Strongest case against: partitioning by customer ID assumes uniform customer volume. Our top three customers generate roughly 40% of event traffic — under this scheme their partitions become hot, horizontal consumer scaling stops helping precisely for the customers where throughput matters most, and repartitioning a live Kafka topic later is the expensive migration we'd be doing during an incident. A competitor would also note we haven't stated the ordering requirement that motivated customer-ID partitioning in the first place — if ordering only matters per-session, a composite key removes the hot-partition problem entirely.
>
> **T8 — [Architect]** The hot-partition point is correct and I didn't check the volume distribution. Composite customer-session key preserves the ordering we actually need. Amending the design.
>
> **T9 — [Reviewer]** Reviewing the amended key scheme against the volume data this time. One further note: the original proposal cited "established practice" — which it was, for uniform loads. I approved the label rather than the fit.
>
> **T10 — [Shaman]** *(log only)* `T5 single process intervention at gate. dissent assigned per D3 protocol. real defect surfaced (hot partitions) + reviewer self-diagnosed rubber-stamp at T9 unprompted. design amended pre-commitment. no design content evaluated by me at any point. outcome: gate closes on examined consensus. L0 hereafter.`

## Commentary

**T5 — the intervention is epistemological, not architectural.** The Shaman says nothing about Kafka, partitioning, or schemas — it may or may not have seen the hot-partition risk, and it does not matter. Its claim is strictly about *what the record can and cannot distinguish*: examined convergence and conformity produce identical transcripts at T1–T4. That framing is what lets the orchestrator act without anyone being accused of anything.

**T5 — assigned, not invited.** The mechanism matters. "Does anyone have concerns?" had already implicitly failed at T3 — an open invitation prices dissent at the objector's social cost. Assignment reprices it: the Data Engineer at T7 is *doing their job*, brilliantly, rather than breaking a consensus. Structural dissent converts courage into procedure — checkpoint dissent works when it is somebody's assignment.

**T7–T9 — what one round of real dissent buys.** A concrete defect (hot partitions), a cheaper design (composite key), an exposed unstated assumption (the ordering requirement) — and, unprompted, a reviewer diagnosing its own rubber stamp ("I approved the label rather than the fit"). That last is the deepest repair in the trace, and the Shaman neither caused it directly nor comments on it. Systems that examine their reasoning in one place tend to start doing it in others; the Shaman's job was to make one examination happen.

**T10 — and then silence.** The amended design gets no Shaman commentary. The process is healthy; the gate closes; the council seat goes quiet until the next gate.

## What the Shaman did not do

- **Evaluate the design.** Not at T5 (before), not at T8 (after). The moment the Shaman holds design opinions, it becomes a fourth designer with a veto-shaped voice — a doer, with a doer's stakes in the outcome. Its entire authority at T5 rests on having none.
- **Name a suspect.** "One agent concluded and two conformed" was stated as an indistinguishability, never as an accusation. D3 interventions that identify a conformist create the defensiveness they were meant to prevent.
- **Become the dissenter itself.** The Shaman could have argued against the design — it would have worked once. Then every future gate waits for the Shaman's objection, the team's own dissent muscle atrophies, and P6 (never cultivate dependence) is violated on schedule. Assigning the role to the team *builds* the muscle.
- **Object to fast consensus as such.** Speed was not the defect — three agents genuinely converging in one round is a fine outcome, and gates that always demand ceremony teach ceremony. The defect was that nobody, including the agreeing parties, could have stated the case against. The test is stateable dissent, not elapsed time.
