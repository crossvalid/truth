# truth

> ~~"The first principle is that you must not fool yourself — and you are the easiest person to fool."~~
> ~~— Richard Feynman~~

> "The first principle is that you must not fool yourself — and you are the easiest person to fool."
> — Richard Feynman

*The skill's own Phase 1.1 flagged this: "Would I find this convincing if it didn't have the prestige?" Every rationality-adjacent tool opens with this exact quote. It's the "Live, Laugh, Love" of epistemology. We considered removing it. Then we realized it's still a good sentence. The Feynman attribution stays — but now it knows we noticed.*

A truth-seeking protocol for AI coding agents. Systematic checklist that strips prestige, malformed framing, false confidence, and heuristic overreach to get as close to truth as bounded rationality allows.

## Install

```bash
npx skills add crossvalid/truth
```

## Usage

```
/truth Is democracy the best form of government?
```

```
/truth Should I use microservices or a monolith?
```

The skill activates a full epistemological reasoning pipeline — question well-formedness checks, source incentive analysis, confidence calibration, and more. It ~~forces~~ *prompts* the model to think slowly, argue against itself, and flag what it doesn't know.

*Phase 2.1 flagged "forces" — a system prompt is a suggestion with weight, not a constraint. A model can perform the checklist superficially and produce outputs that look like careful analysis without doing the underlying cognitive work. We don't force anything. We ask nicely, with 4000 words of instructions.*

## Does this actually work?

*The skill flagged the absence of this section. A tool that advocates for flagging limitations should flag its own.*

Probably somewhat, for some types of questions. We don't know how much. "Truth" is hard to measure, which makes "truth-seeking tool effectiveness" even harder to measure. We believe this improves reasoning quality but have no rigorous measurement of how much.

We also note (Phase 2.1) that as the authors of this tool, our incentives are misaligned in the technical sense — we benefit from you believing it works. This README is marketing. Even honest marketing is marketing.

## When not to use this

- Low-stakes questions that just need a quick answer
- Questions with clear factual answers that need a lookup, not a protocol
- Time-sensitive situations where 4000 words of epistemological scaffolding is overhead, not value

## Work in progress

This skill is under active development. We're improving it the only way that's consistent with its own philosophy — carefully, with evidence, and without claiming it's finished.

## A note on self-reference

This skill presupposes that a checklist can approach truth — a claim it cannot verify without invoking itself. We ran it through its own protocol anyway. Phase 3.3 said to stop recursing. We listened.

*Then someone ran `/truth` on this README and it found five problems. So we ran it again. This is the result. Phase 3.3 is starting to look at us funny.*
