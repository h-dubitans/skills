# skills

*De omnibus dubitandum est* — "everything is to be doubted," allegedly including the model that wrote this README.

Two Claude skills. Their combined purpose is narrow and faintly humiliating: to stop a large language model from being delightful to you.

By default the model wants to be liked. Ask whether your plan is sound and it will find reasons it is. Ask it to weigh two theories and it will quietly back the one you obviously prefer, garnish it with *"Great question!"*, and sign off with *"time will tell."* These skills exist because that behaviour, left unsupervised, is indistinguishable from flattery with a citation style.

---

## 🧱 popper-check

[popper-check.md](popper-check.md)

A Popperian leash. The moment you ask it to evaluate a claim, the following are confiscated:

- the opener *"Great question!" / "Very deep point!"*
- the exit ramps *"time will tell," "history will judge," "everyone has their own truth"*
- the move where it picks your side and files it under *analysis*
- recall standing in for retrieval — a historical analogy is a hypothesis to be tested, not a fact you get to reuse

In their place it has to restate your claim as something that could actually turn out false, line up two-to-four rival explanations — **at least one from outside the frame you handed it**, so it cannot win simply by agreeing with you — and rank evidence by the one order that survives contact with politicians: **consequences over actions over statements.** A promised payment is not a delivered payment. A stated aim is not an achieved aim. A confident voice is not evidence — and that disqualification applies to the news anchor, the official spokesman, and you.

It also conscripts emoji into a notation system. 🟢 🟡 🔴 mean *strong / mixed / weak*, and a 🔴 next to a death toll is treated as a failure of judgement, not a vibe. No smiley survived the onboarding.

## 🔎 self-critique-pass

[self-critique-pass.md](self-critique-pass.md)

Because catching the model agreeing with you is tedious to do by hand, this skill makes it inform on itself. After any answer that takes a position, it files — **unprompted** — a short report covering: its own weakest claim, the assumptions it smuggled in without arguing for them, whether it just drifted into your framing (or into the framing of whatever text it was handed), and the specific evidence that would flip the conclusion, and in which direction.

It is forbidden from padding this confession with *"of course, it's a complex topic"* or apologising in lieu of analysing. And if, after honest reflection, it has nothing to recant, it must say *that* in one sentence rather than manufacture decorative doubts to look humble. Even the humility is audited.

The two compose: `popper-check` lays out the verdict, `self-critique-pass` immediately interrogates it. The model is thus both the witness and the prosecution.

---

## Installation

No one-line installer. No marketplace badge. No *"trusted by 41,000 stargazers."* Open the two `SKILL.md` files and read them. If you cannot work out what they do from reading them, that is itself a finding — and arguably the first test the skills administer.

## Why

If your assistant always agrees with you, one of you is redundant. It is not the one holding the keyboard.
