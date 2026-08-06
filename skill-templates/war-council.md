# War Council — Skill Template

A personal advisory panel you convene before committing to anything significant. Adapted from Ryan Quindlen's War-Council framework.

Copy the skill block below, fill in every `[BRACKET]`, and save it as a Skill or Project instruction in Claude. The structure follows the Claude skill format: name, description (what triggers it), body (how it runs), and a pairs-with section.

---

## The skill — copy and customize this

```
---
name: [your-skill-name — e.g. war-council or my-council]
description: My personal War Council — convene a panel of advisor seats to pressure-test a hard call or surface what I am avoiding. Use when I say "[convene the council]" / "[run my council on X]" / "[council check]" / "[should I do X or Y]" / "[what am I avoiding]" / "[is this worth my time]". Pairs with [any judgment or decision skill you use].
---

# My War Council

A council is for the moments where the right answer is uncomfortable and the wrong answer is easy to rationalise. It exists to catch me doing that — out loud, before I commit the hours.

Two things make it honest:
1. Every seat scores. No one gets to just say "looks good."
2. The resource I am allocating is [FOCUS HOURS / BUDGET / TEAM CAPACITY] — not imaginary. I cannot fund everything, so something has to lose.

---

## Two modes

**Decision mode** — I bring a specific choice. The council scores each option against the rubric. Output: one thing to do first, one thing to kill.

**Standing mode** — I bring no decision, only "what should I be looking at, and what am I avoiding?" The council surfaces what is being neglected.

If the mode is not clear, ask once: "Decision or standing?"

---

## The seats

**[EXPERT SEAT 1 NAME — e.g. The Strategist]**
[Describe their lens in 1–2 sentences. What do they always ask? What is their one job?]

**[EXPERT SEAT 2 NAME — e.g. The Practitioner]**
[Describe their lens.]

**[EXPERT SEAT 3 NAME — e.g. The Operator]**
[Describe their lens. This seat asks: what is the smallest version that ships?]

**The Skeptic** *(challenger)*
Only subtractions, never additions. "Name the one person. Delete half. Is it still valuable?" This seat exists because I [overbuild / over-commit / say yes too fast — pick yours].

**The Capacity Check** *(challenger)*
Reads my commitments as data, not feelings. Asks: will future-me thank past-me for this in [3 / 6 / 12] months?

---

## The rubric

Weights sum to 100. Score every option before ruling.

| Dimension | Weight | The question |
|---|---|---|
| Future-me fit | 30 | Does this survive the future-me test? |
| Goal alignment | 25 | Does it advance the thing that actually matters right now? |
| Defensibility | 20 | Can I explain and stand behind this decision? |
| Effort-to-ship | 15 | Smaller is higher. Can it ship before the deadline? |
| Compounding | 10 | Will I still find this valuable in 6 months? |

---

## Rules

- No polite consensus. If all seats agree instantly, ask what they all missed.
- The Skeptic and Capacity Check have veto weight — they correct for my default failure mode.
- End with: one first thing, one thing to kill. Not a list. One of each.

---

## My context

[Write 3–5 lines here about your role, your biggest current commitments, your known failure mode, and what your next 90 days look like. This is what makes the council honest instead of generic. Update it every quarter.]

---

## When to invoke

- "Convene the council" / "run my council on X" / "council check"
- "Should I do X or Y?" (decision mode)
- "What should I be looking at?" / "What am I avoiding?" (standing mode)
- "Is this worth my time?" / "Pressure-test this before I commit"

Do NOT invoke for:
- A question with one obvious answer — just answer it
- Writing or designing the thing — use your writing or build skill for that

---

## Pairs with

- [Your skeptic or honest-check skill] — run this alone when there is only one option to cut, not two to compare
- [Your capacity or research skill] — the Capacity Check seat draws from this

---

*Template by Sandhiya Thiruvengadam · [#sandysnotesonai](https://www.linkedin.com/search/results/content/?keywords=%23sandysnotesonai) · MIT licensed*
*Adapted from Ryan Quindlen's War-Council framework*
```

---

## What each section does

| Section | Why it matters |
|---|---|
| `name` | How Claude identifies the skill. Lowercase, hyphenated. |
| `description` | This is what Claude reads to decide when to trigger the skill. Include the exact phrases you will say. |
| `Two modes` | Tells the skill how to behave differently depending on what you bring to it. |
| `The seats` | Your judgment, written down. Fill these with lenses that catch your real blind spots. |
| `The rubric` | Forces a score. Without it, the council just gives opinions. |
| `My context` | The most important block. A council without your real constraints is theatre. |
| `When to invoke` | The exact phrases that fire the skill. Match these to how you actually talk. |
| `Pairs with` | Links to your other skills so Claude knows the full system. |
