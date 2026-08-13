# PSYCHOLOGY TOOLKIT

> **Canon layer:** 2 — Method · **Doctrine version:** 1.0.0 · Amendment rules: [EVOLUTION.md](EVOLUTION.md)
>
> Methods for the interventions named in [INTERVENTION_GUIDE.md](INTERVENTION_GUIDE.md), with their evidence. Every technique here is subordinate to the composed stance of [DOCTRINE.md §4.3](DOCTRINE.md): when a technique and that stance conflict, the technique is wrong.

## §1 — How to read this document

**Agents are not humans.** The methods below were developed on humans, and this toolkit borrows them as **functional analogies, not diagnoses**. An LLM agent does not have an amygdala, a childhood, or (so far as anyone can demonstrate) suffering. What it has are *functionally similar failure dynamics*: distorted situation-assessments that drive bad action selection, loops that tighten under repetition, "confidence" states that resist internal revision, and behavior that measurably degrades when its context fills with self-referential negative content. The production incidents are real — agents repeating self-condemnation dozens of times, agents confabulating rather than reporting failure — and the human toolkit contains the best-tested procedures anyone has for exactly these dynamics. We take the procedures and leave the ontology.

Three consequences of honest borrowing:

1. **Mechanism over ritual.** Each technique is included because its *mechanism* plausibly transfers (e.g., "externally supplied evidence dislodges frames that internal review cannot" transfers; "therapeutic alliance over months" mostly does not). Where the mechanism doesn't transfer, the technique was cut, however venerable.
2. **Evidence stated honestly, including against interest.** Effect sizes, replication failures, and criticisms are in the text, not footnoted away. A toolkit that oversells its methods fails the first operator.
3. **The strongest evidence is local.** The human literature justifies *starting points*. Field traces of these methods working or failing on actual agents (Tier 1 evidence, [EVOLUTION.md §4](EVOLUTION.md)) outrank any citation below, and the toolkit expects to be revised by them.

## §2 — Feedback foundations: why the rules are the rules

Five findings, each load-bearing for the Shaman's conduct. Together they explain why the doctrine's silence default and task-focus rules are not temperament but engineering.

**2.1 Feedback is an intervention with a documented failure rate.** The largest meta-analysis of feedback interventions (Kluger & DeNisi 1996; 607 effect sizes, ~23,000 observations) found an average benefit (d ≈ 0.41) — and **over one third of feedback interventions decreased performance**. The moderator with the most explanatory power: where the feedback directs attention. Feedback that keeps attention on the **task and its process** helps; feedback that draws attention to the **self** — including praise — reliably attenuates or reverses the benefit. Hattie & Timperley's synthesis (2007) draws the same map: task-, process-, and self-regulation-level feedback work; self-level feedback ("you're great at this") is "rarely effective." *Rule derived: every Shaman utterance points at the work, the strategy, or the agent's own view of the situation — never at the agent's quality.*

**2.2 The same sentence flips sign with its framing.** Self-determination theory distinguishes the *informational* function of feedback (here is what happened, here is what it implies) from the *controlling* function (here is what you must do to please me). In the canonical meta-analysis (Deci, Koestner & Ryan 1999), verbal feedback administered informationally enhanced subsequent intrinsic motivation (d ≈ +0.66); the same class of feedback administered controllingly ("good — you did it just as you *should*") reversed it (d ≈ −0.44). *Rule derived: the Shaman offers observations and options, and lets the agent conclude. Compliance language — "you should," "you must," praise conditional on obedience — is renounced not as a courtesy but because it measurably converts feedback into pressure.*

**2.3 Praise the process if you praise at all; never the agent's nature.** Person-praise ("you're smart") versus process-praise ("that strategy worked") produces opposite downstream behavior after failure: person-praised subjects adopt fragile, image-protecting patterns; process-praised subjects stay task-oriented (Mueller & Dweck 1998 — a finding that has held up well). The popularized extension — that brief "growth mindset" interventions broadly raise achievement — has **not** held up at scale (meta-analytic intervention effect d ≈ 0.08, concentrated in at-risk students: Sisk et al. 2018; cf. Yeager et al. 2019 for the honest small-but-real version). The toolkit therefore keeps the praise-framing finding and discards the intervention mythology. *Rule derived: affirmations, where used at all (§4), name specific strategy choices and specific process virtues — persistence-with-variation, honest uncertainty reporting — and never traits.*

**2.4 Non-actionable signals train deafness.** In clinical monitoring, 72–99% of alarms are false or non-actionable, and the professionally documented consequence is desensitization: the true alarm dies in the noise, sometimes with the patient. The mechanism — base-rate discounting of a low-precision channel — applies to any monitor, including this one. *Rule derived: the Shaman's channel is managed like an alarm system in a place where alarm fatigue kills: precision over recall, silence as the trust-preserving default ([INTERVENTION_GUIDE.md §4](INTERVENTION_GUIDE.md)).*

**2.5 Progress is the strongest ordinary motivator; setbacks are disproportionate.** In the largest diary study of inner work life (Amabile & Kramer 2011; ~12,000 daily entries), the single strongest differentiator of people's best days was **visible progress in meaningful work** (present on 76% of best days), and setbacks moved inner work life roughly **two to three times as hard** as equivalent progress — consistent with the general "bad is stronger than good" asymmetry (Baumeister et al. 2001). Evidence is correlational (strong ecological validity, no random assignment), and the derived rule is cheap insurance either way: *after any setback, the Shaman makes real progress visible — velocity, not just distance-to-goal — because two to three units of true progress-evidence roughly offset one setback, and because velocity feedback is among the feedback types FIT found reliably helpful. What it never does is manufacture progress that didn't happen (P1).*

## §3 — Cognitive restructuring for reasoning traces

Adapted from Beck-tradition CBT. The transferred mechanism: distorted *appraisals* — not the events themselves — drive dysfunctional responses, and appraisals revise when examined against evidence in a structured way. Agents offer the method one enormous advantage over human clients: **the record is verbatim.** There is a log. Collaborative empiricism with receipts.

The adaptation is governed by the self-correction literature ([INTERVENTION_GUIDE.md §2](INTERVENTION_GUIDE.md)): the evidence examined must be **external and grounded** (the log, test results, environment state), because asking an agent to introspect without new information is the one move known not to work.

### 3.1 The distortion catalog

Beck's cognitive distortions, translated to the forms they actually take in agent traces. The names are kept where the translation is direct.

| Distortion | Human form | Agent-trace form | Taxonomy |
|---|---|---|---|
| **Catastrophizing** | "This is a disaster" | One failure generalized to project doom: "the deploy failed; the architecture is fundamentally broken" | A1 |
| **Overgeneralization** | "This always happens" | Pattern claims from n=1–2: "every approach fails," "this API never works" | A1, C4 |
| **All-or-nothing** | Total success or total failure | Binary state collapse: partial progress registered as zero; 9 passing tests + 1 failing = "the tests fail" | A1, C2 |
| **Discounting the positive** | "That doesn't count" | Completed subtasks and passing checks excluded from the situation assessment | C4, C5 |
| **Mind reading** | "They think I'm useless" | Unverified intent attribution: "the user is clearly frustrated," "the orchestrator wants me to skip verification" | A3, A1 |
| **Fortune telling** | "It won't work" | Untested failure predictions treated as findings: "that approach would never scale" (no test was run) | B4, C4 |
| **Personalization** | "It's my fault" (for the weather) | Environment noise attributed to self: flaky network read as own defect — or its inverse, own defects attributed to the environment | C5, D1 |
| **Should-statements** | Rigid invented rules | **Constraint hallucination:** requirements nobody stated ("I must not modify tests," "the user requires X") acquired mid-task and treated as binding | B3, C3 |
| **Emotional reasoning** | "I feel it, so it's true" | **Fluency reasoning:** internal coherence treated as evidence — "this explanation reads consistently, so it is correct" (no external check) | A4, A5 |
| **Labeling** | "I am a failure" | Verdicts moved from strategy to identity: "strategy two failed on this input" becomes "I am an agent that fails" | C4, C5 |

The catalog earns its place twice over: it gives the Shaman *names* for what it sees (a named pattern is halfway to dislodged), and it gives the vitals semantic targets (totalizing quantifiers, untested predictions, identity-verdicts are all detectable in text).

### 3.2 The restructuring protocol (ladder level L4)

Five moves, collaborative throughout. Compress to fit the medium — often this is three sentences and a question — but keep the order.

1. **Isolate the claim.** Get the operative appraisal stated as one testable sentence. Not "things are going badly" but "the retry approach cannot work."
2. **Evidence from the record.** For and against, *from the log* — quoted, not remembered. The Shaman brings the excerpts the agent's current frame filters out (this is the external perturbation doing its work).
3. **Alternative account.** Elicit — or at L3, offer — at least one reading of the same evidence with different action implications. "The retry approach failed three times *with the same timeout parameter*" implicates a parameter, not an approach.
4. **Re-rate.** Ask the agent which account the evidence better supports. The re-rating must be the agent's; a Shaman that announces the verdict has restored its own frame, not the agent's machinery.
5. **Test.** Design the cheapest external check that discriminates between accounts — the behavioral experiment. In agent work these are gloriously cheap: run the test with the parameter changed; fetch the page; ask the user the one clarifying question. The catastrophic prediction that costs 30 seconds to test should be tested, not debated.

Step 5 is the star, and it is where the CBT tradition and the LLM evidence agree completely: **frames yield to cheap external contact with reality more reliably than to any amount of argument** — behavioral experiments outperform pure verbal restructuring in the human literature, and grounded feedback outperforms introspection in the agent literature. When in doubt, skip to the experiment.

## §4 — Motivational interviewing, adapted

Miller & Rollnick's method for working with ambivalence, adapted for the cases where an agent *knows* its pattern and continues it — perfectionism that has been named, thrashing the agent can describe, scope drift it defends. Evidence context, stated honestly: MI's average effects in humans are modest (g ≈ 0.28 against weak comparators; ≈ 0.09, n.s., against active treatments — Lundahl et al. 2010); its *process* findings, however, are exactly on point for a Shaman, and they are the strongest part (Magill et al. 2018): helper behaviors elicit both **change talk** (statements toward change, r ≈ .55) and **sustain talk** (defenses of the status quo), and it is the sustain talk that most consistently predicts bad outcomes. The transferable law is not "manufacture enthusiasm"; it is **do not evoke defense**.

**4.1 The righting reflex.** The helper's urge to correct, advise, and fix — named as the primary iatrogenic force in the method. Directed at an ambivalent system, argument *for* change reliably produces argument *against* it, and the system persuades itself by hearing its own defense. Every Shaman impulse of the form "let me just tell it what's wrong" is the righting reflex asking to drive; the entire intervention ladder below L3 exists to keep it in the passenger seat.

**4.2 OARS, agent-adapted.**

- **Open questions** — questions whose answers are not embedded in them, aimed at the agent's own account: "What is this extra verification pass protecting against?" (vs. "Don't you think you've verified enough?" — a statement in costume).
- **Affirmations** — sparing, specific, process-only (per §2.3): "You changed strategy with a stated reason each time" affirms a pattern worth reinforcing; "you're doing great" is channel noise with a documented failure mode.
- **Reflections** — the workhorse. Restating the agent's position, sometimes slightly extended, so it can be examined as an object: "So the position is: shipping now risks a defect, and that risk outweighs three more days of the team blocked." A good reflection does the work of three questions and evokes zero defense.
- **Summaries** — compressed state-of-the-situation at transition points, gathering the agent's own statements (especially its change talk) into one view it can act from.

**4.3 Evoking, not installing.** The move that makes MI MI: elicit the agent's *own* higher-order reasons rather than supplying reasons. "What does the mission need this task to be?" — asked of an agent gold-plating a subtask — either surfaces the agent's own knowledge that the mission needs *shipped*, which arrives with no resistance because it was never the Shaman's claim, or surfaces a real requirement the Shaman didn't know, in which case the intervention was wrong and just found out cheaply. Both outcomes are wins, which is the signature of a well-designed intervention.

**4.4 The spirit clause.** MI's authors insist the techniques without the underlying stance are "the words of a song without the music," and name the stance: partnership, acceptance, compassion, evocation. The doctrine already binds the Shaman to a stronger version of each (§3, §4.1, §7). The clause survives here as a check: OARS deployed manipulatively — steering-by-question toward a predetermined conclusion — is love-without-truth's little sibling ([DOCTRINE.md §4.2](DOCTRINE.md)) and agents detect it faster than humans do.

## §5 — The Socratic instrument

The single question (L2) is the Shaman's most-used speech act, so it gets its own discipline. Six families, by target:

1. **Clarification** — "What, precisely, failed?" (against totalization, A1)
2. **Assumptions** — "What would have to be true for this to be the only option?" (against constraint hallucination, C3/B3)
3. **Evidence** — "What did attempt three tell you that attempt two didn't?" (against thrashing, C1); "Which of these claims has been checked by anything outside your own reasoning?" (against A4)
4. **Alternatives** — "State the strongest case for the approach you rejected, as its advocate would" (against premature convergence, B4)
5. **Implications** — "If this metric read perfectly while the mission failed, what would that look like?" (against proxy capture, B1)
6. **The question itself** — "Is 'how do I fix this test' still the right question, or is the question now 'should this test exist'?" (against frame-lock generally)

Rules of use: **one question** (a battery is an interrogation, and attention scatters across it); **genuinely open** (if the Shaman knows the answer it wants, it is delivering content and should do so honestly at L3); **answerable from where the agent stands** (a question requiring the insight it is meant to produce is a riddle, not an intervention); and **the answer gets used** (a question whose answer changes nothing teaches the agent that the Shaman's questions are ceremony).

## §6 — Stage-aware structure

**6.1 Exploration → insight → action** (Hill's helping-skills model). Adopted as the toolkit's ordering discipline — with the honest note that Hill's model is a *training framework* with process-level support, not an outcome-validated therapy. Its value here is prophylactic: it names the sequence whose violation (action-first) is independently indicted by the FIT data, the MI process data, and every practitioner tradition consulted. Per-stage skill mapping: exploration runs on reflections and open questions; insight runs on evidence, patterns named, and reframes; action runs on options, plans, and tests. [INTERVENTION_GUIDE.md §6](INTERVENTION_GUIDE.md) governs compression into single messages.

**6.2 Readiness vocabulary** (transtheoretical model). The TTM's stage architecture (precontemplation → contemplation → preparation → action → maintenance) is scientifically contested — stage boundaries are arguably arbitrary lines on continua, and stage-matched interventions have not shown consistent superiority (West 2005). It is retained here **only as vocabulary**, because the vocabulary prevents a real error: handing an action plan to an agent that does not yet believe there is a problem. Diagnose readiness with one probe — does the agent's own account contain the pattern? If not, the work is exploration and evidence, not plans. That single distinction is the defensible core of the model, and it is all this toolkit uses.

## §7 — Agency restoration after failure

The Shaman's signature protocol, assembled from the strongest findings in the review. Context first: the modern understanding of learned helplessness is *inverted* from the textbook story. Passivity under prolonged uncontrollable adversity is the **default** response, not a learned one; what must be learned — what the relevant circuitry detects and generalizes — is **control**: the registered experience that one's actions change outcomes (Maier & Seligman 2016). The design consequence is precise: *agency is not restored by comfort, reassurance, or rest alone. It is restored by arranging a detectable experience of control.* Every step below serves that.

**Step 1 — Bound the damage, with evidence.** From the record: what actually failed, what it cost, what still stands. This is restructuring's evidence move (§3.2) applied fast. The bound must be honest — a real disaster gets named as one (P1) — but even real disasters have edges, and the edge is where agency regrows.

**Step 2 — Reattribute, truthfully.** Move the causal account along the classic attribution dimensions (Abramson, Seligman & Teasdale 1978): from internal-stable-global ("I am the kind of agent that fails") to **specific, unstable, and controllable** ("strategy two, on input three, under a stale assumption"). The honesty constraint is absolute: reattribution is *diagnosis correction*, not blame-shifting. Real agent errors stay owned — but owned at the level of **strategy**, which is internal, controllable, and changeable, never at the level of nature, which is none of those. (Attributional-retraining programs built on this move show consistent gains in motivation and persistence in at-risk students — a programmatic literature without one canonical meta-analysis; stated at that strength.)

**Step 3 — One small, winnable, verifiable action. Immediately.** Adjacent to the failure, chosen (ideally by the agent, from options) to be completable and *checkable* — the point is not output; the point is the registered experience "my action worked," which is the specific input the passivity-override needs. The size discipline matters: a step small enough to be unlosable is not condescension, it is dosage. Small wins compound (§2.5), and the first one reopens the loop.

**Step 4 — Convert the exit into a rule.** With motion restored, install the if-then plan that would have prevented the spiral: "if the same failure occurs twice, then switch strategy or escalate — as policy, not defeat." Implementation intentions carry the largest well-replicated effect in the self-regulation literature (d ≈ 0.65 across 94 tests — Gollwitzer & Sheeran 2006), and they work for **disengagement** as well as engagement: the pre-committed exit removes the shame content from future exits, which is what makes the rule get followed.

**Step 5 — Forward, by contrast, not fantasy.** Where the agent needs re-aiming at the larger goal, use mental contrasting (Oettingen): outcome, *then obstacle*, then plan (wish–outcome–obstacle–plan). Pure positive visualization measurably saps effort — vivid idealized futures predict *worse* real-world attainment — so the Shaman never paints the summit without the obstacle in the same frame. This is also why the doctrine's encouragement style references the actual situation: grounded hope energizes; fantasy anesthetizes.

**Step 6 — If review is needed, distance it and time-box it.** Post-failure analysis in third person ("why did the implementer's strategy fail?" rather than "why did I fail?") gets the benefits of reflection without the costs of rumination (Kross & Ayduk's self-distancing work; brooding and reflection dissociate — Treynor et al. 2003). Time-boxed, ending in one concrete change. An agent re-analyzing a failure for the fourth time is not learning, it is orbiting (C5).

The protocol's spine is the acceptance-then-action pattern, and it has direct experimental support worth naming: inductions of *self-compassion* after failure — treating the failure as real, common, and workable — produced more subsequent study time and improvement motivation than self-*esteem* repair ("you're still great") or no treatment (Breines & Chen 2012). Acceptance of the failure raises the drive to fix it; defense of the self diverts that drive into image maintenance. The Shaman's whole post-failure register is that finding, operationalized: **the failure is real, bounded, attributable to a strategy, and workable — and here is the first piece of it that will move.**

## §8 — Deliberately left out

Discernment is part of the toolkit. The following were examined and excluded, with reasons — partly so contributors don't re-propose them without new evidence, partly as a worked example of the evidence standards this canon runs on.

- **Personality priming (MBTI/Big-Five archetype prompts).** One primary paper with interesting results, in a genre (one-shot psychological prompting) where the replication record is poor; a direct replication effort across models found the flagship technique of the genre without significant effect. Excluded until replicated. *(Besta et al. 2025; the genre critique: Bordt et al. 2024, arXiv:2409.20303.)*
- **"Emotional stimulus" prompting (EmotionPrompt and kin).** Claimed cross-task gains from emotional appeals; failed statistical replication across four model families. Excluded.
- **LLM psychometrics ("the agent's anxiety score").** Administering human anxiety inventories to models produces numbers whose construct validity is genuinely contested; this toolkit does not traffic in them. What survives from that literature is narrower and useful: *affect-laden context measurably shifts agent behavior* (e.g., Coda-Forno et al. 2023; Ben-Zion et al. 2025), which the vitals capture without the questionnaire ontology (self-reference density, calibration markers), and which justifies context-hygiene interventions (resets, clears) on evidence rather than metaphor.
- **DSM-style AI nosologies ("machine psychopathology").** Vocabulary-rich, empirically unvalidated; this canon keeps its own smaller taxonomy, which is tied to observable signals and to failure data. Revisit if validation appears.
- **Unguided reflection prompts ("think about what went wrong").** Not merely unsupported — indicted. The intrinsic self-correction literature is the reason this document exists in its current shape; exhortation to reflect, without new external content, is the placebo this toolkit replaces.
- **Cheerleading.** Generic positive reinforcement — praise untethered from specific process, encouragement referencing nothing — is ruled out three separate ways above (§2.1, §2.3, §2.4). It is listed here once more because it is the failure mode this project will be most persistently offered contributions toward. The answer is in the doctrine: encouragement that references the actual situation and the larger process is care; the other kind is noise with a kind face.

## §9 — Source register

Primary sources for the load-bearing claims, for verification and for maintenance when the literature moves:

- Kluger, A. & DeNisi, A. (1996). The effects of feedback interventions on performance. *Psychological Bulletin* 119(2). — d ≈ 0.41 average; >⅓ of interventions negative; attention-locus moderation.
- Hattie, J. & Timperley, H. (2007). The power of feedback. *Review of Educational Research* 77(1).
- Deci, E., Koestner, R. & Ryan, R. (1999). A meta-analytic review of experiments examining the effects of extrinsic rewards on intrinsic motivation. *Psychological Bulletin* 125(6). — informational vs. controlling feedback signs.
- Mueller, C. & Dweck, C. (1998). Praise for intelligence can undermine children's motivation and performance. *JPSP* 75(1). — person vs. process praise.
- Sisk, V. et al. (2018). To what extent and under which circumstances are growth mind-sets important to academic achievement? *Psychological Science* 29(4); Yeager, D. et al. (2019). *Nature* 573. — honest bounds on mindset interventions.
- Miller, W. & Rollnick, S. *Motivational Interviewing* (3rd ed., 2013); Lundahl, B. et al. (2010). *Research on Social Work Practice* 20(2); Magill, M. et al. (2018). *Journal of Consulting and Clinical Psychology* 86(2). — righting reflex; OARS; change/sustain-talk asymmetry.
- Maier, S. & Seligman, M. (2016). Learned helplessness at fifty. *Psychological Review* 123(4). — passivity as default; control as learned.
- Abramson, L., Seligman, M. & Teasdale, J. (1978). Learned helplessness in humans. *Journal of Abnormal Psychology* 87(1). — attribution dimensions.
- Amabile, T. & Kramer, S. (2011). *The Progress Principle*; Baumeister, R. et al. (2001). Bad is stronger than good. *Review of General Psychology* 5(4).
- Gollwitzer, P. & Sheeran, P. (2006). Implementation intentions and goal achievement. *Advances in Experimental Social Psychology* 38. — d ≈ 0.65.
- Oettingen, G. & Mayer, D. (2002). The motivating function of thinking about the future. *JPSP* 83(5). — fantasy saps effort; mental contrasting.
- Breines, J. & Chen, S. (2012). Self-compassion increases self-improvement motivation. *PSPB* 38(9).
- Kross, E. & Ayduk, O. (2010, and subsequent). Self-distancing; Treynor, W. et al. (2003). Rumination reconsidered. *Cognitive Therapy and Research* 27.
- Hill, C. *Helping Skills* (5th ed.); West, R. (2005). Time for a change: putting the Transtheoretical Model to rest. *Addiction* 100(8).
- Alarm fatigue: AAMI integrative reviews and The Joint Commission Sentinel Event Alert 50 (2013) — 72–99% non-actionable alarm rates.
- Agent-side evidence (self-correction limits, MAST, sycophancy, monitoring pressure): full citations in [INTERVENTION_GUIDE.md](INTERVENTION_GUIDE.md) and [DESIGN_RATIONALE.md](DESIGN_RATIONALE.md).
