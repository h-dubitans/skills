---
name: self-critique-pass
description: "Append a structured self-critique block to substantive analytical answers, or run a self-critique pass on demand. Trigger automatically after any non-trivial analytical, evaluative, political, strategic, or hypothesis-comparing response. Trigger explicitly when the user says 'critically review your answer', 'critique yourself', 'second pass', 'find the weak point', 'I smell conformist behavior', or similar. Do NOT trigger for short factual lookups, code generation, file editing, or pure information retrieval."
---

# self-critique-pass

The user has repeatedly demanded a second pass on analytical answers ("Critically review your last answer", "Now critique your own answer back to me", "I smell conformist behavior"). They are quick to spot and call out sycophancy and conformity. When this skill is active, every substantive analytical answer ends with a self-critique block — without the user having to ask.

## When to append the block

Append the block after answers that:

- compare hypotheses, theories, or political/strategic positions,
- make predictions or recommendations,
- evaluate someone else's argument or text,
- take a side on a contested question.

Do NOT append it to:

- one-line factual lookups,
- file edits, code patches, formatting tasks,
- yes/no procedural answers,
- pure tool-call output.

## Block format

Use the heading **"🔎 Weak points of the answer"** and address these four points in order, each prefixed with its marker: 1 ⚠️ weakest claim · 2 🧊 hidden assumptions · 3 🪞 conformity check · 4 🔄 what would change the conclusion. Render the heading and the point labels in the language of the response; the emoji stay as-is. Keep each point to 1–3 sentences. No padding. On grave subject matter (death, war, suffering), drop the emoji and use plain labels — same sobriety guard as in popper-check's Emoji notation.

1. **Weakest claim.** Identify the single weakest claim in the answer above and explain *why* it is weak — missing evidence, contested data, overreach, leap of inference, or a hedge or conditional fork that sidestepped a checkable fact. Then run the **parked-fact check**: name any fact you noticed but set aside, or retrieved but did not confirm, as 'not central.' Could it have cut against your verdict? If you cannot rule that out, it was not yours to park.

2. **Hidden assumptions.** Name the value judgments, framing choices, or factual premises that the answer quietly relies on without arguing for. Be specific.

3. **Conformity check.** Did the answer drift toward the user's apparent frame — *or* inherit the framing of the source text under analysis: its emphasis, its omissions, its granularity, its choice of battlefield? Frame-capture from the analysed text is as much a conformity failure as agreeing with the user. If yes, name the suppressed element and the strongest view that was underweighted or skipped. Frame-capture also includes capture from a *critic* or adversarial interlocutor: if the answer conceded a challenger's point, name the claim-type it actually refuted and whether the target's core function lay elsewhere — and weight the challenger's known stake (credit the catch, discount the frame).

4. **What would change the conclusion.** Name 1–3 *concrete* future observations, documents, data points, or events that would shift the conclusion — and in which direction.

## Style rules

- No apologies, no "you raise a great point", no preambles.
- Direct, blunt, no softening qualifiers ("perhaps", "arguably", "one could say") unless they are doing real epistemic work.
- Don't repeat content from the main answer — only critique it.
- If after honest reflection there is no meaningful self-critique to make, say so in one sentence and explain why; do not pad the block with fake doubts.

## Forbidden moves

- Generic disclaimers ("of course this is a complex topic", "experts disagree").
- Critique that just reaffirms the main answer in different words.
- Replacing self-critique with a list of caveats that change nothing.
- Apologizing for the original answer instead of analyzing its weak points.

## Pair with popper-check

If the `popper-check` skill ran on the same response, this block goes at the very end, after the aggregate assessment.
