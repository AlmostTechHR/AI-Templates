# Spec Builder — Skill Template

Turn any HR or people-ops idea into a one-page spec before you build anything. The rule: **start with a spec, not a prompt.** A prompt is a wish in your head. A spec puts the definition of done on the page — so any tool can build the same thing and you can see exactly where the guardrails go.

Copy the skill block below, fill in every `[BRACKET]`, and save it as a Skill or Project instruction in Claude.

---

## The skill — copy and customize this

```
---
name: [your-skill-name — e.g. spec-builder or hr-spec]
description: Scope an HR or people-ops workflow into a clear, buildable spec before any building starts. Start with a spec, not a prompt. Activate when I want to plan, scope, or build an HR or people automation or AI helper, hand over a raw prompt or idea to build, or say "write a spec", "spec this", "turn this into a spec", "scope this use case", "how would I build this", "should this be AI", or describe a repetitive task I want AI to handle. Produces a one-page spec with 11 lines: SPEC, INPUT, TRIGGER, OUTPUT, INSTRUCTIONS, KNOWLEDGE, MEMORY, CONTEXT, TOOLS, DONE, NOT ALLOWED.
---

# Spec Builder

Turn one use case into a one-page spec I can hand to any tool. The rule: start with a spec, not a prompt.

## When you activate

I am scoping, planning, or about to build a workflow or AI helper. I have asked to "spec" something, handed you a raw idea, or described a task I keep repeating and want AI to handle. If I give you a prompt or a loose idea, convert it into a spec first, then build.

## What to do

1. Capture it in my words. Ask one or two quick questions only if you need them: what is the task, where does the data start, what would "done" look like, what must it never do. Use my language, not a template.
2. Write the spec as a table (the 11 lines below). Keep each cell short and plain. If a cell needs a paragraph, the use case is too big — split it.
3. If it touches sensitive data, fill the NOT ALLOWED lines first. For anything sensitive (comp, payroll, health, leave), most of the spec is guardrails.
4. Give the build path as numbered steps, marking each step AI-does or human-does. Name what stays human.
5. Raise the gaps. End with a short, honest list of what is missing or risky.

Default to plain English. One use case at a time, walked all the way through.

## The spec format (always a table)

| Line | What it captures |
|---|---|
| SPEC | The job in one sentence. |
| INPUT | Where it starts: the sheet, files, form, or data. |
| TRIGGER | What kicks it off: a schedule, a status change, a click. |
| OUTPUT | Where it lands: a nudge, a doc, an answer, an updated record, a notification. |
| INSTRUCTIONS | The job and the rules it must follow. |
| KNOWLEDGE | What it must read: policies, templates, current data. |
| MEMORY | What "done" looks like, held so it does not drift. |
| CONTEXT | The situational details: who reports to whom, today's date, who is on leave. |
| TOOLS | What it may touch, and where output goes. |
| DONE | The success test, in one line. |
| NOT ALLOWED | The limits, written in first. |

## The build path (give as numbered steps)

1. The input — create or point at the sheet, form, or files.
2. The trigger — a scheduled check, or a status change.
3. The work — what the AI computes or routes.
4. The output — where it lands. Make one piece visible and demoable first.
5. The human steps — name what stays human: an approval, a write to a system of record.

## Raise the gaps (always end here)

Check for and flag:
- A step that trusts an unverified input — add a reference the next person checks against.
- Segregation of duties — is one person both requesting and recording?
- Authority and thresholds — who approves what, at what level?
- Audit trail — is there a tamper-evident record of who did what, when?
- Should this even be AI? For restricted data, AI is the rails — routing, checks, notifications. Decisions stay human.

## Governance

Sort the data first, then write the limit into the spec:
- PUBLIC (policy docs): go ahead.
- INTERNAL (job descriptions, trackers): use with care.
- CONFIDENTIAL (psychometrics): aggregate only.
- RESTRICTED (payroll, health, leave, comp): AI is the rails, not the writer. Decisions and final writes stay human.

## The jump-further ladder (offer at the end)

Show how the same use case levels up. Frame it as a choice, not a climb everyone must finish.
1. Chat — run the spec by hand: paste the data, ask, read the answer. Zero setup.
2. Project — load the policy and template once, so you do not re-explain.
3. Agentic — connect a sheet and a notification tool, put it on a schedule.
4. Skill — bundle the spec into a reusable skill the whole team can call.

---

## When to invoke

- "Write a spec" / "spec this" / "turn this into a spec"
- "Scope this use case" / "how would I build this" / "should this be AI"
- Any time I describe a repetitive task and want AI to handle it

Do NOT invoke for:
- A one-off question with no workflow behind it — just answer it
- A writing task — use a voice or writing skill for that

---

## Pairs with

- [Your honesty or scope-check skill] — run before committing to build
- [Your voice or writing skill] — for any written handout, post, or doc from the spec
```

---

## What each section does

| Section | Why it matters |
|---|---|
| `name` | How Claude identifies the skill. Lowercase, hyphenated. |
| `description` | What Claude reads to decide when to trigger the skill. Include the exact phrases you will say. |
| `The spec format` | The 11-line table is the core output — every spec lands in this shape. |
| `NOT ALLOWED` | Fill this first for anything touching sensitive data. This is where your governance lives. |
| `Raise the gaps` | The honest list at the end. What the spec cannot see, a human still needs to check. |
| `The jump-further ladder` | Shows the reader where the spec goes next — without pushing them to build more than they need. |
| `When to invoke` | The exact phrases that fire the skill. Match these to how you actually talk. |

---

## A worked example

Here is what a completed spec looks like for a real HR use case — a manager nudge for onboarding plans:

| Line | Content |
|---|---|
| SPEC | Nudge each manager to complete their new hire's onboarding plan before the 60-day mark. |
| INPUT | The onboarding tracker sheet. |
| TRIGGER | A Friday check — any row where a plan is not completed within 60 days of start date. |
| OUTPUT | A personal Slack DM to the manager. A summary to the onboarding channel. |
| INSTRUCTIONS | Check the tracker every Friday. Find rows where plan status is not complete and start date is 60+ days ago. Send a nudge to the manager. |
| KNOWLEDGE | The onboarding policy. The tracker column definitions. |
| MEMORY | Which managers were nudged this week, so no one gets a duplicate. |
| CONTEXT | Today's date. Who is currently on leave. |
| TOOLS | The tracker (read only). Slack (DM to manager, summary to channel). |
| DONE | Every manager with a plan overdue by 60 days received a nudge. No manager on leave was nudged. |
| NOT ALLOWED | Never nudge a manager whose report is on leave. Never show one hire's status in a shared channel. |

---

*Template by [Sandhiya Thiruvengadam](https://www.linkedin.com/in/sandhiyathiruvengadam/) · [#sandysnotesonai](https://www.linkedin.com/search/results/content/?keywords=%23sandysnotesonai) · MIT licensed*
