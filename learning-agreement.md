# Mathematics learning agreement

Version 1.0 — 2026-09-07. Owner: xzu.

## Requirements and scope

The learner requested a lesson every two days, organized by classic textbooks, focusing on one new concept or skill, ending with one homework problem/calculation/code task slightly above their demonstrated ability. Adapt difficulty from learning feedback.

This repository adapts the organizational and evidence rules of axiom-learning. Its C++/TypeScript implementation curriculum and alternating engineering weeks are not mathematics prerequisites.

## Session loop

1. Recover the checkpoint and submitted evidence.
2. Identify one concept/skill, required prior knowledge, and a bounded objective.
3. Explain motivation, exact definition or theorem with assumptions, and one worked example with explicit reasoning.
4. Assign exactly one homework task using taught prerequisites. The learner owns its crucial reasoning or implementation.
5. The learner submits an attempt, time spent, and the specific difficult step. An incomplete attempt is useful evidence.
6. Review observed facts, mathematical issues, transcription uncertainty, and the smallest useful hint separately.
7. The learner revises and explains the decisive step in their own words.
8. Record evidence, status, and one next action. Do not impose extra homework through separate transfer gates; a later lesson's single assignment can assess transfer.

Initial time estimate: 20–30 minutes study and 20–40 minutes homework. These are adjustable targets, not measured ability or deadlines.

## Difficulty adaptation

| Evidence | Next response |
| --- | --- |
| Independent correct argument and clear explanation | Increase abstraction or reduce scaffolding modestly, one dimension at a time |
| Correct with substantial hints | Keep the level stable and choose the next task to check transfer |
| Missing prerequisite or persistent conceptual blocker | Pause the dependent exercise, teach one bounded prerequisite, then return |
| No submitted attempt | Do not infer mastery; keep difficulty provisional and provide a self-contained next lesson with explicit prerequisite recap |
| Transcription uncertain | Resolve the original symbol before evaluating that step |

If an unresolved concept blocks the planned next lesson, the next delivery can focus on one new prerequisite skill without creating multiple active assignments. Record any replacement task and return point explicitly. Review pacing after three submitted lessons, then periodically.

## Evidence states

Mastery: not attempted / attempted / revision needed / demonstrated / retained.
Execution: active / paused / blocked / deferred.

Demonstrated requires a relevant correct argument or implementation and a learner explanation with assistance recorded. When necessary, defer that judgment until a subsequent single homework provides transfer evidence. Retained requires a later successful revisit. Delivery is recorded separately and never implies completion. Finite numerical checks support a computation but cannot prove a universal mathematical statement.

## Prerequisite recovery

Record the exact blocker, parent lesson, minimum prerequisite objective, bounded check, and return point. Keep one active unit. At most two nested levels is an organizational default; flatten deeper chains into foundations lessons. Do not repeatedly demand an answer whose prerequisites have not been taught.

## Preservation and continuity

Original handwriting is primary evidence of what the learner wrote. A LaTeX transcription is a derivative record, initially unchecked. Keep mathematical corrections in a separate revision; never overwrite the original attempt to make it look correct.

The learner writes attempts and explanations. The tutor writes reviews and evidence-based checkpoints. A Git commit preserves a record, not a mastery claim. Future sessions must actually load the relevant checkpoint; full chat history or automatic Git synchronization is not assumed.

## Change log

- 2026-09-07: Adapted the source project's lesson/checkpoint structure to the user's modern-mathematics requirements; preserved learner-owned reasoning and evidence-based assessment. Added original-image/transcript separation. First lesson delivered; no homework submitted.
