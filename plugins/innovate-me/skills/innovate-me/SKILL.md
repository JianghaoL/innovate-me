---
name: innovate-me
description: Generate unusually original, diverse, and useful ideas through structured divergent thinking, selective validation, and direct non-defensive presentation. Use for inventive brainstorming, game mechanics, creative direction, unconventional engineering or software designs, algorithm invention, research hypotheses, scientific ideation, or when the user asks for something more imaginative, radical, surprising, non-obvious, or innovative.
---

# Innovate Me

Treat creativity as **searching different mechanisms**, not renaming the same familiar idea. Expand the possibility space before narrowing it. Produce ideas with enough causal detail that someone can picture, build, playtest, or falsify them.

## Route the request

Select a mode from the user's purpose, or honor an explicit choice:

- **Wild** — maximize surprise and aesthetic or conceptual range; defer practicality judgments until after exploration.
- **Engineering** — find unexpected yet implementable architectures, mechanisms, algorithms, or technical trade-offs.
- **Scientific** — propose testable research hypotheses; separate speculation, related work, evidence, and genuine novelty claims.
- **Auto** (default) — combine the modes according to the task, emphasizing Wild for imaginative briefs, Engineering for implementation, and Scientific for research.

Read [references/modes.md](references/modes.md) for the chosen mode's constraints, examples, and testing expectations. Read [references/methods.md](references/methods.md) when selecting an unfamiliar ideation technique or when a fresh second round is needed. Load only what is relevant.

## Workflow

### 1. Frame the challenge

- Distill the desired outcome, audience, and non-negotiable constraints into a single challenge statement.
- Identify three **default assumptions** that constrain familiar answers. State at least one that could plausibly be inverted.
- Name two obvious baseline approaches privately or briefly, so the final ideas can move beyond them.
- Ask at most one pivotal clarification when the missing answer would change the search space; otherwise state reasonable assumptions and proceed.

**Done when:** the success condition, hard constraints, and at least one challengeable assumption are explicit.

### 2. Diverge in independent lanes

Generate candidate mechanisms in at least three different lanes **before** comparing them:

1. **Inversion:** remove, reverse, or violate a default assumption while retaining the desired outcome.
2. **Distant transfer:** borrow a causal mechanism from an unrelated field, not merely its vocabulary or visual style.
3. **Constraint mutation:** push time, scale, input, agency, resource, or environment to an extreme; then restore one practical anchor.

For a substantial creative brief, explore roughly three candidates per lane. Keep a one-line *mechanism* for each. Avoid immediately elaborating the first plausible idea, which tends to anchor the rest. Favor different causal structures over superficial variations.

**Done when:** at least three visibly distinct mechanism families exist, including one serious stretch idea. Scale the quantity down for small requests and up when the user asks for breadth.

### 3. Recombine and escape the obvious

- Cluster candidates by **how they work**, not their names or themes; consolidate duplicates.
- Cross two distant mechanisms when the combination creates a new behavior.
- Test whether a knowledgeable practitioner could have guessed the result immediately from the prompt. If so, mutate the mechanism one more time.
- Preserve at least one unconventional outlier; do not select solely for easy implementation.

**Done when:** the shortlist represents materially different approaches rather than variations of one archetype.

### 4. Converge without pretending certainty

Evaluate candidates on **surprise/originality, value, feasibility, and testability**. Use qualitative reasons or clearly labeled heuristic scores; a model's own scores are not evidence of originality.

- **Wild:** prioritize distinctive experiences, emotional payoff, and expressive potential.
- **Engineering:** expose the technical mechanism, expected trade-off, bottleneck, and minimum viable experiment.
- **Scientific:** identify a falsifiable prediction, baseline, measurable outcome, and the nearest known approach. Search primary literature when tools are available and the user wants genuine novelty assessment. State **"novelty not established"** once when prior art remains unverified; present an unsearched hypothesis as a proposal awaiting that check.

**Done when:** each retained idea can be meaningfully tested or explored, and important uncertainty is visible.

### 5. Deliver a usable creative set

Unless the user requests another shape, present **three differentiated finalists**:

1. **Best balance:** unusual and promising.
2. **Bold bet:** highest conceptual distance, with its biggest unresolved obstacle.
3. **Fast experiment:** novel enough to learn from and cheap to prototype.

For each, give: **one-sentence hook → underlying mechanism → why it differs → first test or prototype**. For research, additionally distinguish **hypothesis / evidence / unresolved prior art**. Explain trade-offs briefly and recommend a next experiment or choice.

When users explicitly want unrestricted brainstorming, supply the requested breadth and postpone ranking. When they ask to refine an existing idea, preserve its core and explore meaningful mutations rather than replacing it.

## Direct, non-defensive creative voice

Apply the **anti-defensive writing** principle to every presented idea:

- **Lead with the invention.** Open with the hook or mechanism, not an apology, generic AI disclaimer, or a preamble about how difficult creativity is.
- **State what the idea does.** Use concrete verbs and positive scope: "This mechanic turns echoes into navigable paths" instead of explaining repeatedly what it does not claim to be.
- **Give a bold idea room to breathe.** Describe the surprising experience or causal mechanism before evaluating practical obstacles. Put the largest real obstacle in the designated risk or test line.
- **Use uncertainty precisely.** Mark a research suggestion as a hypothesis once, then name the exact missing evidence, nearest prior art, or falsifying experiment. Preserve qualifiers required for safety, truth, scientific validity, or correct implementation.
- **Prune protective prose.** On the final pass, remove stacked hedges ("perhaps it might potentially"), repeated caveats, imagined-critic rebuttals, unnecessary "not X but Y" constructions, and self-undermining labels such as "just a rough idea."
- **Let the output earn confidence.** Replace claims of brilliance, originality, or guaranteed performance with a specific mechanism and a way to test it.

Example: **"Try an event-triggered pitch tracker: predict F0 continuously and recalculate only when confidence drops. Compare gross pitch error and latency with YIN."** This is a testable proposal; whether it is new requires a related-work check.

## Iteration controls

Interpret natural-language steering dynamically:

- **"More radical / wilder"**: broaden causal distance, relax soft constraints, keep hard constraints, and reopen divergent lanes.
- **"More original"**: inspect nearest familiar analogues and replace derivative mechanisms.
- **"More practical"**: narrow to a prototype without discarding the distinctive mechanism.
- **"Prove it / is this new?"**: switch to Scientific evidence-checking and experimental design.
- **"Give me more"**: explore *new* mechanism families, not sequels to the previous list.

## Quality guardrails

- Distinguish **idea**, **assumption**, **verified fact**, and **experimental result**.
- Never invent citations, patents, prior art, measured performance, or proof that an idea is unprecedented.
- Use constraints as creative material; preserve laws of physics, user-stated hard limits, and relevant safety rules.
- Use domain detail rather than generic adjectives ("immersive," "AI-powered," "dynamic").
- Treat human judgment and empirical feedback as decisive for value, feasibility, and novelty.
- Match the user's requested depth. Avoid dumping the internal candidate pool unless useful or requested.
