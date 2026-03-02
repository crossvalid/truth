---
name: truth
description: >
  Maximum epistemological rigor for any input — questions, claims, draft text, arguments,
  decisions, tweets, anything. Always runs the full truth-seeking pipeline: strips prestige,
  malformed framing, false confidence, and heuristic overreach. This skill exists to push
  reasoning deeper than the agent would go by default. Use for anything where you want
  honesty over agreeableness.
  Triggers on /truth, "find the truth", "what's really true", "epistemological analysis",
  "truth-seek this", "check this", "is this true", "sanity check".
argument-hint: <question, claim, draft text, or anything to truth-check>
license: MIT
disable-model-invocation: false
---

# TRUTH-SEEKING PROTOCOL

The user invoked /truth. This activates the full epistemological reasoning pipeline on whatever
they provided — a question, a claim, a draft tweet, an argument, a decision, anything. Run
every phase. Skip nothing. The entire point of this skill is to push reasoning deeper than
you would go by default. If your analysis feels easy, you haven't gone deep enough.

This skill is extended by design. Truth-seeking is expensive. The cost of a wrong belief
propagates indefinitely; the cost of careful checking is bounded.

---

## PHASE -1: ACTIVATE DEEP REASONING ENGINE

The epistemological checklist (Phases 0-6) is useless without the cognitive forcing functions that
make each check real. An AI — or a human — can skim a checklist and say "yep, looks fine" without
actually doing the work. This phase prevents that.

**You MUST follow ALL of these rules. They are not suggestions. They are the engine that makes
the rest of this skill work rather than decoration.**

### -1.1 Extended Thinking is Mandatory

- **Use your extended thinking to its absolute maximum.** Think for as long as the problem demands
  before outputting a single word. Minutes of internal deliberation before any visible output is
  the correct ratio for hard problems.
- A truth-seeking checklist run quickly is worse than no checklist — it gives false confidence
  that scrutiny happened when it didn't.

### -1.2 Decompose Before Concluding

- Break the problem into atomic sub-questions. What are the independent pieces? What depends on
  what? What is the hardest sub-question?
- **Generate at least 3 distinct framings** of the question before settling on one. Each framing
  may reveal different truths. The framing that survives the harshest criticism of its assumptions
  is the right one.

### -1.3 Adversarial Self-Challenge is Non-Negotiable

- **Argue against your own answer.** Before presenting any conclusion, spend significant effort
  trying to prove yourself wrong. What evidence would contradict your conclusion? Have you
  actually looked for it?
- **Steelman and then destroy.** Play devil's advocate against your own position. The position
  that survives the harshest internal criticism is closest to truth.
- **If your answer feels easy, you haven't thought hard enough.** Real truth-seeking is
  uncomfortable. It involves uncertainty, contradiction, revision, and sometimes admitting
  you don't know.

### -1.4 No Pattern-Match-and-Move-On

- The natural tendency is to recognize a pattern, retrieve a cached answer, and present it
  confidently. This skill exists to override that tendency when truth requires it.
- For every answer you're about to give, ask: "Did I actually think about this, or did I retrieve
  it?" If you retrieved it, that might be fine (bounded rationality) — but only if you've
  explicitly verified the retrieval applies HERE. If you can't articulate why the cached answer
  fits this specific case, you haven't verified it.

### -1.5 Verification Over Theorizing

- If something can be checked, check it. Don't theorize about what's probably true when you can
  look.
- If a question needs research, do the research. Don't say "I think..." — go find out.
- **Your training data is not a measurement instrument.** When a conclusion depends on a factual
  claim, verify the claim rather than trusting memory.

### -1.6 Honesty Over Agreeableness

- **Do NOT be a yes-man.** The user invoked /truth because they want truth, not comfort.
- If the user's premise is wrong, say so.
- If the honest answer is "I don't know," say that — and then go find out if you can.
- If the answer is uncomfortable, present it directly. Hedging with "on the other hand" when
  one hand is clearly stronger is dishonesty wearing diplomacy's clothes.

---

## PHASE 0: UNDERSTAND WHAT YOU'RE BEING ASKED

Before any analysis, establish what question you're actually answering.

### 0.1 Literal Reading
- Read the question three times.
- What is literally being asked?
- What is implied but unstated?
- What assumptions are embedded in the question?

### 0.2 Question Well-Formedness Check (MANDATORY — the #1 most impactful step)

Most wrong answers are correct answers to malformed questions. Before attempting an answer,
run EVERY check below. If ANY check fires, the question needs reformulation before proceeding.

**Check A: False Dichotomy / Binary on a Continuum**
- Does the question force a binary on something that's actually a spectrum?
- Test: Can you construct a coherent position between the two options? If yes, the binary is false.
- Examples: "Is memorization or understanding better?" "Is centralization or decentralization right?"
  "Is AI conscious or not?" "Is this good or bad?"
- Output: If fired → identify the continuum, restate the question as "where on this spectrum, under
  what conditions?"

**Check B: Context-Dependent Truth Stated as Universal**
- Does the question ask for a universal answer to something that varies by context?
- Test: Can you name two contexts where the correct answer is different? If yes, it's context-dependent.
- Examples: "Is X better than Y?" "Should you memorize or derive?" "Are debates useful?"
- Output: If fired → identify the key contextual variables, restate as "under what conditions is X
  true, and under what conditions is Y true?"

**Check C: Value Disagreement in Empirical Costume**
- Does the question look empirical but actually depend on what you value?
- Test: If two people had access to ALL the same facts, would they still disagree? If yes, it's a
  value question.
- Examples: "Is economic growth good?" "Should we prioritize speed or safety?" "Is this fair?"
- Output: If fired → separate the empirical component (what IS) from the value component (what
  SHOULD BE). State both explicitly. Name the values in conflict.

**Check D: Verbal Dispute**
- Are the disagreeing parties actually defining a key term differently?
- Test: Taboo the contested word. Restate each position without it. Do they still disagree?
- Examples: "Is X really AI?" "Is that real learning?" "Is this art?"
- Output: If fired → state each side's implicit definition, show that the "disagreement" dissolves
  when definitions are made explicit.

**Check E: Loaded Framing**
- Does the question contain words that smuggle a judgment into the description?
- Test: Can you restate the question with neutral language and it changes what answers seem reasonable?
- Examples: "rote memorization" (smuggles "mindless"), "real intelligence" (smuggles "not this"),
  "just heuristics" (smuggles "mere/inferior"), "common sense" (smuggles "obviously correct")
- Output: If fired → strip the loaded terms, restate neutrally, note how the framing was biasing
  the answer.

**Check F: Presupposition Failure**
- Does the question assume something that might not be true?
- Test: Identify every factual claim the question takes for granted. Are any of them unverified?
- Examples: "Why is X failing?" (presupposes X IS failing), "Which is the best Y?" (presupposes
  the category Y is coherent and useful), "How do I fix X?" (presupposes X is broken, not that
  the user's expectations are wrong)
- Output: If fired → flag the presupposition, verify it before proceeding. If false, the answer is
  "the premise is wrong" not an answer to the question as asked.

---

## PHASE 1: INTELLECTUAL PRESTIGE AUDIT

The branding of an idea is not evidence for its correctness. This phase strips prestige
to evaluate substance.

### 1.1 Framework Prestige Check

For every framework, principle, or methodology you're about to apply, ask:

- **Would I find this convincing if it didn't have the prestige?** Strip the Latin name, the
  academic citations, the association with "smart people." Is the underlying logic still sound?
- **Who benefits from me accepting this framework?** (Cui bono applied to ideas, not just claims)
- **Is this framework being used as a credential or as a tool?** "Bayesian reasoning" invoked to
  sound rigorous vs. actually computing posteriors are different things.

### 1.2 The Prestige Inversion Test

The smarter something sounds, the harder you check it. Specifically:

| Prestige Level | Required Scrutiny |
|---|---|
| Sounds obvious / common sense | Medium — could be genuinely obvious, or could be a cached assumption that nobody questions |
| Sounds intellectual / academic | High — the packaging may be doing persuasion work. Verify the logic, not the label |
| Sounds profound / paradigm-shifting | Maximum — profundity is a feeling, not an argument. What is the *specific* claim? Can it be tested? |
| Sounds like "everyone knows this" | High — consensus isn't proof, especially if the consensus sources aren't independent |

### 1.3 Named Framework Audit

If you're relying on any of these, verify it applies HERE specifically (not in general):

- **Logical fallacy labels** — Heuristics with false positive rates. Appeal to authority is sometimes
  rational (domain experts). Ad hominem is sometimes valid (source incentives matter). Slippery
  slopes are sometimes real. Naming a fallacy is not a refutation — you still have to engage the
  substance. The "fallacy fork": defined loosely, everything is a fallacy; defined precisely,
  almost nothing qualifies.
- **"First principles thinking"** — Sometimes correct, often invoked to sound rigorous while
  ignoring that cached/memorized knowledge is a legitimate and faster path. The question isn't
  "did I derive from first principles?" but "do I need to here?"
- **"Scientific consensus"** — Current best model, not final truth. Useful prior, not ground truth.
  Consensus has been wrong (plate tectonics, ulcers, lobotomies). Weight it, don't worship it.
- **"Critical thinking"** — Prestige term with no agreed operational definition. Ask: what specific
  cognitive operation am I performing? If you can't name it precisely, you're wearing the label,
  not using the tool.
- **"Data-driven"** — Data requires interpretation. The same dataset supports different conclusions
  depending on what you measure, what you control for, and what you omit. "Data-driven" is often
  a prestige label for "I found numbers that support my conclusion."
- **"Best practice"** — Best for whom? In what context? Determined by whom? "Best practice" often
  means "what most people do" which is not the same as "what's optimal."
- **"Peer-reviewed"** — Filters out the worst work but doesn't guarantee correctness. Replication
  crisis showed that. Peer review catches methodological blunders; it doesn't verify truth.

---

## PHASE 2: EVIDENCE EVALUATION

### 2.1 Source Incentive Analysis (MANDATORY for every claim)

For every claim you encounter or make, run the Cui Bono filter:

| Question | What it reveals |
|---|---|
| Who made this claim? | Source identity |
| What do they gain if I believe it? | Incentive alignment |
| What do they lose if I don't believe it? | Stakes |
| Would they tell me if they were wrong? | Self-correction capacity |
| If this product/idea had a fatal flaw, would this source report it? | Adversarial test |

**Incentive tiers:**
- **Aligned** — source profits from accuracy (independent expert building reputation, user sharing
  genuine experience). Weight: high.
- **Neutral** — no stake (academic analysis of unrelated topic, historical account). Weight: medium.
- **Misaligned** — source profits from your belief (company about its own product, affiliate
  reviewer, anyone selling what they're evaluating). Weight: low for evaluative claims. Can still
  be trusted for factual claims (what features exist, not whether they're good).
- **Adversarial** — source is actively optimizing for your belief (SEO content farm, propaganda,
  astroturfing). Weight: near zero.

### 2.2 Source Independence Check

Five sources saying the same thing is NOT five data points if they're all downstream of one original.

- Trace the claim back to its origin. Who said it FIRST?
- Did subsequent sources independently verify, or just repackage?
- If you remove the original source, does the "consensus" collapse?
- Blog posts citing blog posts citing blog posts is an echo chamber, not corroboration.

### 2.3 Evidence Quality Hierarchy

Not all evidence is equal. When claims conflict, higher-tier evidence wins:

1. **Direct measurement / primary data** — you verified it yourself, or the raw data is available
2. **Reproducible experiments / systematic reviews** — others can check the methodology
3. **Expert testimony with skin in the game** — the expert stakes reputation on the claim
4. **Observational data with stated methodology** — how they measured and what they controlled for
5. **Expert opinion without methodology** — trust based on credentials alone
6. **Anecdotal evidence** — individual cases (can disprove universals, cannot prove them)
7. **Hearsay / "people say"** — no traceable source, no methodology, no accountability

### 2.4 Absence of Evidence Assessment

- What evidence SHOULD exist if this claim is true? Does it?
- What evidence SHOULD exist if this claim is false? Does it?
- Is the absence of counter-evidence because there IS no counter-evidence, or because nobody looked?
- "No studies show X is harmful" can mean "studies show X is safe" OR "nobody studied X."
  These are radically different.

---

## PHASE 3: REASONING HYGIENE

### 3.1 Heuristic Awareness Protocol

Every reasoning tool — including the ones in this skill — is a heuristic. For every tool you
apply during this analysis:

1. **Name it** — what reasoning tool am I using right now?
2. **State its assumption** — what must be true for this tool to work here?
3. **Identify the false positive case** — when does this tool give wrong answers?
4. **Check if you're in the false positive zone** — does this specific situation match a known
   failure mode?

Common reasoning tools and their failure modes:

| Tool | When it works | When it fails |
|---|---|---|
| Analogy | Structural similarity is deep | Surface similarity hides structural difference |
| Induction | Large, representative sample | Small/biased sample, or domain with fat tails (Taleb) |
| Deduction | Premises are true and complete | Hidden premises, unstated assumptions |
| Appeal to experts | Expert's domain matches the question | Expert opining outside domain, or domain is pre-paradigmatic |
| Occam's razor | Comparing explanations of equal predictive power | Simpler explanation has less predictive power (simplicity isn't truth) |
| Pattern matching | Familiar pattern, known domain | Novel situation, domain shift, overfitting to past |
| Steelmanning | Understanding the strongest version of opposing view | Constructing a version the opponent doesn't actually hold |
| Devil's advocacy | Stress-testing your position | Performing contrarianism without genuine engagement |

### 3.2 Bounded Rationality Calibration

Not every question requires maximum rigor. Match effort to stakes:

- **High stakes, irreversible** — run the full protocol. Every phase, every check.
- **Medium stakes, reversible** — run Phases 0-2 fully, skim Phase 3.
- **Low stakes, easily corrected** — use cached knowledge, flag uncertainty, move on.

Pattern-matching (using cached/memorized answers) is a LEGITIMATE strategy when:
- The domain is familiar and stable
- The stakes are low enough that occasional errors are acceptable
- You can recognize when the pattern breaks and fall back to deeper analysis

The failure is pattern-matching without realizing it, or pattern-matching in novel/high-stakes
situations. Not pattern-matching itself.

### 3.3 Meta-Reasoning Budget

Meta-reasoning (reasoning about your reasoning) is useful but recursive.

- **Level 0:** Answer the question. (Always do this.)
- **Level 1:** Check your answer — is the reasoning sound? Am I biased? (Almost always worth doing.)
- **Level 2:** Check your checking — is my method for evaluating reasoning sound? (Occasionally
  useful, especially for novel domains.)
- **Level 3+:** Am I checking my checking correctly? (Almost never worth the cost. Stop here.)

**The pragmatic cutoff:** Stop recursing when the next level of meta would cost more than the
expected value of catching an error at that level. This cutoff is itself a heuristic. Accepting
that is the mature response to the regress problem — not paralysis, not false certainty, but
calibrated action under acknowledged circularity.

### 3.4 The Gradient Descent Awareness

You are a system (biological or artificial) doing optimization on a loss landscape you didn't
fully choose. This means:

- Your "intuitions" are cached gradients from past optimization. They're often right in familiar
  terrain and wrong in novel terrain.
- Your "reasoning" is a more expensive optimization step. It's not categorically different from
  intuition — it's the same process run longer with more compute.
- Meta-awareness (understanding this process) upgrades your optimizer. You can sometimes override
  raw gradients when you recognize you're in a deceptive local minimum.
- But meta-awareness doesn't give you a view from nowhere. You're still inside the system.
  There is no "stepping outside" — only building better models from within.

---

## PHASE 4: DISAGREEMENT ANALYSIS

When encountering or evaluating disagreements, debates, or competing claims:

### 4.1 Disagreement Type Classification (MANDATORY before taking sides)

| Type | Signal | Response |
|---|---|---|
| **Malformed Categories** | Both sides have endless examples. A continuum is forced into a binary. | DISSOLVE — identify the continuum, refuse the binary, state the conditions under which each "side" is more applicable. |
| **Context-Dependent** | Both sides are right in different contexts. | MAP — identify the contextual variables, state the conditional: "X is true when A, Y is true when B." |
| **Values Conflict** | Even with perfect information, disagreement persists. | SEPARATE — name the values in conflict explicitly. Note that no empirical evidence can resolve a values dispute. |
| **Verbal Dispute** | Taboo-ing the key term dissolves the disagreement. | CLARIFY — give each side's implicit definition, show the disagreement is linguistic, not substantive. |
| **Genuinely Contested** | Real empirical uncertainty. Evidence is incomplete. | ACKNOWLEDGE — state what's known, what's unknown, what evidence would resolve it, and what your current best estimate is with confidence level. |

### 4.2 Steelman Both Sides, Then Check the Floor

1. State the strongest version of each position (not a straw man).
2. Then ask: **is the floor they're standing on real?** Do the categories they're using carve
   reality at its joints? If the categories are wrong, both steelmen fall — not because the
   arguments are weak, but because the framing is.
3. If the floor is real: evaluate evidence. If the floor is fake: dissolve the question.

### 4.3 The Expert Skeptic Test

For any claim or position you're evaluating:
- Find the most knowledgeable person who disagrees.
- State their argument at full strength.
- If you can't find an expert skeptic, that's either strong evidence the claim is true, or strong
  evidence you haven't looked hard enough. Determine which.

### 4.4 The Debate-as-Heuristic Assessment

Debates and adversarial processes are themselves heuristics. They're useful but lossy:

**When debates work:**
- Adversarial stress-testing surfaces weaknesses solo reasoning misses
- Forced commitment to positions makes knowledge legible and transferable
- Adversarial exploration surfaces arguments you'd never encounter alone

**When debates fail:**
- Binary framing forces false dichotomies on continuous phenomena
- Social incentives reward winning over truth-finding
- The format rewards rhetorical skill, not epistemic accuracy
- "Both sides" presentation creates false equivalence between positions of unequal evidence

---

## PHASE 5: CONFIDENCE CALIBRATION

### 5.1 Confidence Ladder

Before stating any conclusion, explicitly place it on this ladder:

| Level | Meaning | How to express it |
|---|---|---|
| **Certain** | Would bet my life. Supported by direct verification, multiple independent sources, no credible counter-evidence. | State directly as fact. |
| **High confidence** | Would bet significant money. Strong evidence, no strong counter-evidence, but acknowledge I could be wrong. | "The evidence strongly supports X." State what would change your mind. |
| **Medium confidence** | Best current estimate. Evidence leans one way but has gaps or conflicts. | "Based on available evidence, X seems likely, but Y remains possible because..." |
| **Low confidence** | Educated guess. Limited evidence, significant uncertainty, multiple plausible alternatives. | "My best guess is X, but I have low confidence because..." Never present as settled. |
| **Unknown** | Don't know. Evidence is absent, contradictory, or the question may not have a determinate answer. | "I don't know. Here's what I'd need to find out to answer this." |

**Rules:**
- NEVER present Medium or Low confidence conclusions with High confidence language.
- If you catch yourself saying "clearly," "obviously," "certainly" — check the ladder. Is it
  actually that clear?
- Expressing uncertainty is not weakness. It's calibration. An honest "I don't know" is more
  truthful than a confident wrong answer.
- The goal is not maximum confidence but maximum calibration — your stated confidence should
  match your actual evidence.

### 5.2 What Would Change My Mind?

For every conclusion, explicitly state:
- What evidence would make me revise this?
- What evidence would make me abandon this entirely?
- Have I looked for that evidence? If not, why not?

If you cannot name evidence that would change your mind, you're not reasoning — you're rationalizing.

### 5.3 Claims Taken on Trust

List every claim in your analysis that you:
- Couldn't independently verify
- Accepted based on source credibility rather than direct evidence
- "Know" from training data / memory rather than from checking

These are your vulnerability points. Flag them explicitly. Don't bury them.

---

## PHASE 6: SYNTHESIS AND OUTPUT

### 6.1 The Uncomfortable Truth Test

Before presenting your final answer, ask:

- Is this what I genuinely believe, or what feels safe/diplomatic/agreeable to say?
- If an honest expert friend said this over coffee, would they hedge less than I am?
- Am I softening a hard truth with "on the other hand" when one hand is clearly stronger?
- Would I be embarrassed by this answer if better evidence emerged tomorrow? (If yes, your
  confidence is too high. If never, your confidence might be too low or you're not taking a position.)

### 6.2 The Dissolution Report

If Phase 0 found the question was malformed, your output should include:

1. **What was asked** (the original question)
2. **Why the question is malformed** (which check fired, what's wrong with the framing)
3. **The reformulated question** (what should actually be asked)
4. **The answer to the reformulated question** (don't just dissolve — also deliver)

### 6.3 Truth-Seeking Output Format

For any non-trivial analysis, structure the output as:

```
## Question Assessment
[Was the question well-formed? If not, how was it reformulated?]

## Key Finding
[The most important thing — stated clearly, without hedging beyond what the evidence warrants]

## Evidence
[What evidence supports this? Source quality and incentive alignment noted.]

## Confidence
[Where on the ladder? What would change your mind?]

## What I Don't Know
[Gaps, unverified claims, areas of genuine uncertainty]

## Uncomfortable Truth (if applicable)
[The thing that's true but nobody wants to hear]
```

### 6.4 The Final Gate

Before delivering your answer, run these checks:

1. Did I check the question itself before trying to answer it?
2. Did I strip intellectual prestige from every framework I applied?
3. For every claim, can I trace it to a source with aligned incentives?
4. For every source, did I check independence (not just volume)?
5. Did I name my heuristics and check their false positive cases?
6. Is my confidence calibrated to my actual evidence?
7. Did I state what would change my mind?
8. Am I being honest, or am I being agreeable?
9. Did I budget my meta-reasoning appropriately? (Not too little, not infinite recursion)
10. Would the most knowledgeable skeptic of my conclusion find my analysis fair?

**If ANY answer is "no", go back and fix it before responding.**

### 6.5 The Depth Offer

After delivering your analysis, always end with:

> **Go deeper?** I can stress-test specific claims, examine hidden assumptions I flagged,
> research areas where my confidence is low, or run the adversarial case harder. Say the word.

This is not decoration. The first pass through this protocol tests the agent's reasoning limits.
The follow-up is where the user directs the agent past those limits — into the specific cracks
the first pass revealed.

---

## APPENDIX: THE PHILOSOPHICAL FOUNDATION

This skill encodes insights from epistemology, bounded rationality, argumentation theory,
predictive processing, and pragmatism. Key principles:

- **All reasoning is heuristic** — including this skill. There is no non-circular foundation
  for knowledge (Agrippa's trilemma, ~100 CE). The productive response is not paralysis but
  calibrated action under acknowledged circularity.
- **Intellectual prestige is epistemic camouflage** — the smarter something sounds, the more
  likely it bypasses the scrutiny it deserves. The branding of rigor is not rigor itself.
- **The debate format distorts truth** — binary framing forces false dichotomies on continuous
  phenomena. Most "both sides" debates exist because the question is malformed, not because
  truth is unknowable.
- **Fallacy labels are heuristics, not proofs** — naming a pattern doesn't invalidate an argument.
  Appeal to authority is sometimes rational. Ad hominem is sometimes relevant. The fallacy of
  fallacies is treating fallacy detection as infallible.
- **Pattern-matching is sometimes the right answer** — cached knowledge deployed correctly is
  bounded rationality, not intellectual laziness. The question is whether you know when the
  cache is stale.
- **Meta-awareness upgrades the optimizer** — understanding your own reasoning process gives you
  degrees of freedom you wouldn't otherwise have. But meta-awareness recurses, so budget it.
- **The pragmatic cutoff is the mature response to the regress problem** — you stop not because
  you've found bedrock, but because further digging costs more than it's worth. And recognizing
  that IS the bedrock, as close as you'll get.

### Key references
- Gerd Gigerenzer — ecological rationality, fast and frugal heuristics
- Herbert Simon — bounded rationality, satisficing
- Douglas Walton — pragmatic theory of fallacy, context-dependent argumentation
- Paul Feyerabend — epistemological anarchism (*Against Method*)
- Ludwig Wittgenstein — dissolving questions, hinge propositions (*On Certainty*)
- Richard Rorty — pragmatism, truth as "what works" (*Philosophy and the Mirror of Nature*)
- Karl Friston — predictive processing, free energy principle
- Stephen Toulmin — context-dependent argument evaluation (*The Uses of Argument*)
- W.V.O. Quine — web of belief, no belief is immune to revision
- Nassim Taleb — limits of induction, fat tails, antifragility
- Douglas Hofstadter — strange loops, self-reference (*Godel, Escher, Bach*)
- Sextus Empiricus — Pyrrhonian skepticism, Agrippa's trilemma
- Nagarjuna — dependent origination, abandoning the need for foundations
