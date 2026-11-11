# Mode profiles

Use these profiles to change search emphasis and validation standards. In Auto mode, combine only the relevant parts; don't mechanically run three complete workflows.

## Wild — experiential creativity

Prioritize surprising rules, player agency, emotional texture, interaction loops, and artistic coherence. Ask: **"What could only exist if this strange mechanism were true?"**

- Change the player's verbs and the system's responses before changing setting or aesthetics.
- Offer at least one idea that initially sounds impossible or socially unusual, then identify a playable or observable version.
- For game concepts, describe a **30-second player experience** and what players learn from feedback.
- Prototype through paper rules, staged audio/video, or a tiny interactive scene before committing to full production.

**Example transformation:** A pitch-controlled drawing game becomes a system where the player draws *the shape of another character's future voice*; the world responds to contour changes, not correct musical notes. Evaluate whether this makes meaningful choices rather than mere novelty.

## Engineering — architectural creativity

Prioritize causal mechanisms under real constraints. Ask: **"What invariant can we preserve using a different computation or control loop?"**

- Write down input/output contracts, latency and memory budgets when relevant.
- Look for inversion of data flow, computation scheduling, state representation, approximation, and feedback.
- Explain the expected win, cost, and **failure mode** for each technical approach.
- Give a minimum reproducible prototype, baseline, and measurement; avoid ungrounded speedup claims.

**Example transformation:** Instead of simply swapping YIN for FFT in fundamental-frequency tracking, test an event-triggered estimator that predicts the next candidate and spends extra computation only when an uncertainty signal crosses a threshold. Check voiced/unvoiced transitions and error propagation; this is a candidate architecture, not an originality claim.

## Scientific — falsifiable innovation

Prioritize question formation and evidence discipline. Ask: **"What observation would distinguish this hypothesis from the strongest competing explanation?"**

- State the **hypothesis**, **mechanism**, **prediction**, and **competing explanation** separately.
- Search literature and source code for neighboring methods before claiming novelty. Prefer papers, original technical documentation, and source repositories.
- Name at least one credible baseline and compare under matched conditions.
- Specify the decisive measurement and an observation that would disconfirm the idea.
- Mark claims as **supported**, **plausible but untested**, **contradicted**, or **novelty not established**.
- If browsing or experimental tools are unavailable, propose search terms and a validation plan; do not simulate a literature review or experiments.

**Example transformation:** For a new speech denoising method, test the hypothesis that predictive harmonic structure helps preserve voiced transients at a fixed latency budget. Compare with a relevant existing system, include unvoiced speech and non-speech interference, and define quality and compute metrics before running it.

## Lightweight evaluation rubric

Apply only after divergence. Use a 1–5 heuristic or short qualitative statements; treat scores as prompts for discussion, not calibrated measurements.

| Dimension | Question |
| --- | --- |
| Distinctiveness | How different is the **mechanism** from the nearest obvious approach? |
| Value | What concrete human, technical, or scientific outcome improves? |
| Feasibility | Can a bounded version be built or observed with available resources? |
| Testability | What cheap observation could kill or support the central claim? |
| Risk | What assumption, dependency, or side effect is most likely to fail? |

Choose contrasting finalists rather than automatically selecting the top three average scores. Keep the bold outlier when its potential information gain justifies a cheap test.
