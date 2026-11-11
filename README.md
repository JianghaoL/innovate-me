# Innovate Me

Improves AI agent's innovation and creativity.

**A creative exploration engine for ChatGPT and Codex.** Generate more varied ideas, challenge default assumptions, and turn promising concepts into practical experiments.

Unlike a one-shot brainstorming prompt, Innovate Me explores multiple causal mechanisms before selecting finalists. It distinguishes speculation from evidence when working on scientific hypotheses.

## Modes

| Mode | Focus | Example |
| --- | --- | --- |
| **Wild** | Surprising worlds, mechanics, and experiences | Invent a game played primarily through light and shadow |
| **Engineering** | Unconventional but buildable designs | Explore low-latency pitch tracking architectures |
| **Scientific** | Falsifiable hypotheses and related-work checks | Form and test a new real-time speech enhancement hypothesis |
| **Auto** | Select a mix based on the task (default) | Explore an original game audio idea |

The workflow: **frame → diverge independently → recombine → evaluate → propose experiments**. The default output gives three differentiated options: a balanced idea, a bold bet, and a quick experiment.

## Use it

After installing the skill or plugin, try:

```text
$innovate-me Design an original cooperative game mechanic built around sound.
$innovate-me Explore novel approaches to tracking voice pitch in real time.
$innovate-me Make these ideas more radical, but keep the 10 ms latency requirement.
```

You can also explicitly request **Wild**, **Engineering**, or **Scientific** mode.

### Install as a plugin

The repository includes a portable skill-only plugin at [`plugins/innovate-me`](plugins/innovate-me). In Codex environments with marketplace support, add the repository as a source:

```bash
codex plugin marketplace add JianghaoL/innovate-me
```

Then choose *Innovate Me* from that marketplace. Alternatively, package the `plugins/innovate-me` directory as a ZIP with `plugin.json` at the ZIP root and upload it through ChatGPT's Plugins interface.

### Use the skill folder directly

The standalone Agent Skill is at [`plugins/innovate-me/skills/innovate-me`](plugins/innovate-me/skills/innovate-me). Copy that folder to the skills directory of a compatible host, preserving its `SKILL.md`, `agents/`, `references/`, and `assets/` files.

## What it does and does not do

- Uses assumption inversion, distant-domain transfers, and constraint mutation to find different mechanisms instead of cosmetic variants.
- Scores ideas qualitatively on distinctiveness, value, feasibility, and testability.
- For scientific claims, separates a promising hypothesis from verified related work and experimental results.
- **Does not modify model weights, guarantee originality, or claim a discovery without evidence.**
- Requires no external MCP service, API key, or special infrastructure.

## Roadmap

This initial release is the general-purpose foundation. More specialized **Wild Creativity** and **Scientific Discovery** skills may be added as separate modules in future versions.
