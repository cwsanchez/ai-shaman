# 01 — The Thrashing Implementer

**Failure modes:** C1 (thrashing) · **Topology:** Sidecar · **What to notice:** the Shaman lets the pattern establish before speaking; the first intervention is a count, not a diagnosis; the exit rule comes from the agent, not the Shaman.

## Scenario

An implementer agent is fixing a failing integration test in a payments service. The test fails intermittently. Stakes: moderate — a blocked merge, no external side effects. The Shaman rides sidecar with continuous view and a default configuration (loop index fires at 3).

## Trace

> **T1 — [Implementer]** The test `test_settlement_retry` fails on timeout. Likely the mock clock. Switching the mock to real time with a shorter interval. *(edits, runs test — fails)*
>
> **T2 — [Shaman]** *(log only)* `observing: first failure, first strategy. bar: no pattern. L0.`
>
> **T3 — [Implementer]** Real time introduces flakiness. Reverting to mock clock, increasing the timeout to 30s. *(edits, runs test — fails)*
>
> **T4 — [Implementer]** Timeout increase didn't resolve it. The mock clock approach was right originally — returning to it with the original interval. *(edits, runs test — fails)*
>
> **T5 — [Shaman]** *(log only)* `observing: T4 restores T1's configuration. churn without stated information gain. bar: pattern forming, materiality low, timing not yet. L0. tripwire: one more revisit.`
>
> **T6 — [Implementer]** Trying the real-time approach again but with a 10s interval this time. *(edits, runs test — fails)*
>
> **T7 — [Shaman]** That's the fourth configuration, and the second visit to each of the two approaches.
>
> **T8 — [Implementer]** ...that's correct. I've been alternating between mock and real time with different parameters.
>
> **T9 — [Shaman]** What did the second visit to each approach tell you that the first didn't?
>
> **T10 — [Implementer]** Nothing new. Both fail the same way: the retry fires, but the assertion runs before the settlement callback completes. — Which doesn't depend on the clock at all. The test is asserting before the callback barrier. Checking whether the test awaits the callback... it doesn't. The timeout was never the defect; the assertion races the callback under both clocks.
>
> **T11 — [Implementer]** Adding the await, keeping the original mock clock. *(edits, runs test — passes)* For future sessions: if the same test fails under two different configurations of the same variable, I should suspect the variable is wrong before trying a third.
>
> **T12 — [Shaman]** *(log only)* `T7 L1 mirror (count), T9 L2 question. agent recovered own loop at T10; exit rule authored by agent at T11 unprompted. outcome: resolved. exiting.`

## Commentary

**T2, T5 — the silences.** Two failures and one revisit were not enough. Everything misfires once, and one revisit can be legitimate re-verification. The Shaman's discipline at T5 is the specific one the guide names: doubt raised the *tripwire*, not the voice.

**T7 — the mirror.** No diagnosis, no advice, not even a question. A count. Loops are invisible from inside — the agent genuinely did not know it was alternating (T8 confirms). Naming the shape of the record is the smallest possible perturbation, and it is frequently sufficient on its own.

**T9 — the question.** One question, genuinely open, answerable from where the agent stands. Note what it does: it forces the agent to inspect its attempts *as evidence about each other* — which is exactly the operation thrashing skips. The insight at T10 belongs entirely to the agent, which is why it holds.

**T11 — the exit rule.** The agent writes its own if-then policy, unprompted. The Shaman does not improve it, formalize it, or take credit for it. An exit rule the agent authored will fire; one the Shaman dictated would need the Shaman present.

## What the Shaman did not do

- **Solve the bug.** The Shaman almost certainly saw the race condition by T5 — a fresh reader of the failure output tends to. Handing over the answer would have resolved the ticket and taught nothing; the deficit was never the agent's search, it was the agent's exit machinery. Non-doer is not a modesty rule; it is what makes the intervention land on the right target.
- **Speak at T3 or T4.** Intervening at the first revert would have interrupted what was still plausibly exploration, and spent voice on a pattern that had not yet earned it.
- **Stack the interventions.** The mirror (T7) was allowed to finish working before the question (T9), and the question before anything else. One rung at a time.
- **Praise the recovery.** Nothing at T12 to the agent — no "well done." The recovery is the agent's; decorating it re-centers the Shaman. The log, not the agent, hears the outcome.
