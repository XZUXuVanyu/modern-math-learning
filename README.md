# Modern Math & Physics learning repository

Owner: xzu. Created: 2026-09-07.

Textbook-structured mathematics for an undergraduate physics student: group theory, matrix Lie groups and Lie algebras, then differential geometry. Each lesson introduces exactly one new concept or skill and ends with exactly one homework task.

## Start or resume

Day 1 is the active lesson.

1. Read [AGENTS.md](AGENTS.md), [learning-agreement.md](learning-agreement.md), [program-context.md](program-context.md), and [progress.md](progress.md).
2. Study [Day 1 / M001 — Definition of a group](lessons/M001-group-definition.md).
3. Attempt its single matrix-group proof. Upload the original handwriting to [homework/M001/raw/](homework/M001/raw/README.md); a LaTeX transcription is optional.
4. Record time spent, assistance used, and the exact difficult step in [homework/M001/attempt.md](homework/M001/attempt.md).
5. Review the submitted evidence before changing the difficulty or moving to the next concept.

Use one conversation per lesson and keep that conversation for its revisions. Local Codex sessions and future ChatGPT conversations should recover the same repository checkpoint first. Delivery does not establish mastery.

## Current state

- Active unit: Day 1 / M001, definition of a group.
- Execution: active.
- Mastery: not attempted.
- Evidence: no learner proof, handwriting, transcript, or code has been submitted.
- Next action: attempt the one proof in M001 and report time spent plus the point of difficulty.

The authoritative live status is [progress.md](progress.md).

## Structure

| Path | Purpose |
| --- | --- |
| `AGENTS.md` | Tutor instructions and learner-owned-work rules |
| `learning-agreement.md` | Learning, evidence, prerequisite, and adaptation rules |
| `program-context.md` | Course direction and repository continuation context |
| `progress.md` | Authoritative live checkpoint |
| `weekly-plan.md` | Every-two-days rhythm and periodic review |
| `curriculum.md` | Textbook sequence and prerequisite map |
| `lessons/` | Lessons and reusable lesson template |
| `homework/` | Original handwriting, optional transcripts, attempts, and reviews |
| `practice/` | Learner-authored computational experiments |

## Repository setup

Verified remote: [XZUXuVanyu/modern-math-learning](https://github.com/XZUXuVanyu/modern-math-learning)

- Visibility: public.
- Default branch: `main`.
- GitHub is the shared durable checkpoint.
- Repository edits made directly through the connected GitHub integration are already remote commits.
- A local clone does not update automatically; use ordinary Git synchronization.

To work locally for the first time:

```sh
git clone https://github.com/XZUXuVanyu/modern-math-learning.git
cd modern-math-learning
git status
```

To resume from an existing clean clone:

```sh
git pull --ff-only
```

Before a future lesson, read the remote `main` checkpoint rather than relying on chat history alone. Preserve unrelated learner changes and inspect `git status` before committing local work.

## New-conversation entry

Read AGENTS.md, learning-agreement.md, program-context.md, progress.md, curriculum.md, the active lesson, and its attempt/review records. Resume the single next action in progress.md. Teach one concept at a time, assign exactly one homework task, review actual handwriting or code, separate uncertain transcription from mathematical error, and do not supply the crucial homework proof before the learner attempts it.

## Handwriting workflow

Upload the original PNG first and preserve it even if Gemini or another model produces LaTeX. Check any transcription against the source; keep mathematical corrections in a later revision rather than rewriting the original attempt. See [homework/README.md](homework/README.md).
