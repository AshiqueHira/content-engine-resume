# 03 · Social Media Manager AI review

**Purpose:** Have an independent critic check the work twice: the concept before anyone spends time on design, and the finished post before it is published.
**Runs as:** the separate subagent `smm-reviewer` ([.claude/agents/smm-reviewer.md](../.claude/agents/smm-reviewer.md)). The agent that wrote the work must not review it. Always hand off to `smm-reviewer`.

## Two review gates

| Gate | When | Mode | Reads | Writes | On `revise` |
|---|---|---|---|---|---|
| Concept review | After 02, before 04 | `concept` | `01-strategy`, `02-content-concept/concept.md` | `03-smm-ai-review/review.md` | Back to 02 |
| Output review | After 05, before 06 | `output` | `05-output/<post>/` (captions and images), approved concept | `05-output/<post>/review.md` | Back to 02, 04 or 05, as each change is routed |

**Verdict rule (both gates):** `pass` if every score is ≥ 4. Otherwise `revise`. After 2 revise loops, `escalate` to a human.

## How to invoke
- Concept: *"Use the smm-reviewer agent in concept mode."*
- Output: *"Use the smm-reviewer agent in output mode on `05-output/2026-10-09-my-topic/`."*

The criteria, the evidence rules and the output templates for each mode live in the agent file, so edit them there.
