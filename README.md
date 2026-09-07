# Modern Math & Physics learning repository

Owner: xzu. Created: 2026-09-07.

Textbook-structured mathematics for an undergraduate physics student: group theory, matrix Lie groups and Lie algebras, then differential geometry. One new concept or skill and one homework task per lesson.

## Start or resume

1. Read [AGENTS.md](AGENTS.md), [learning-agreement.md](learning-agreement.md), [program-context.md](program-context.md), and [progress.md](progress.md).
2. Open the active lesson: [M001 — Definition of a group](lessons/M001-group-definition.md).
3. Attempt its single homework. Upload original handwriting to [homework/M001/raw/](homework/M001/raw/README.md); LaTeX transcription is optional.
4. Record your time spent and obstacle in [homework/M001/attempt.md](homework/M001/attempt.md). Receive feedback, revise, and checkpoint.

Use one conversation per lesson, continuing it for revisions. Local CLI sessions should read the same records. Receiving a lesson does not establish mastery. Actual submissions, review evidence, and the current checkpoint determine progress.

## Structure

| Path | Purpose |
| --- | --- |
| `AGENTS.md` | Tutor instructions and learner-owned work |
| `learning-agreement.md` | Learning, evidence, prerequisite, and adaptation rules |
| `program-context.md` | Goals, source-project mapping, and continuation context |
| `progress.md` | Authoritative live checkpoint |
| `weekly-plan.md` | Every-two-days schedule and weekly review |
| `curriculum.md` | Textbook sequence and prerequisite map |
| `lessons/` | Lesson 1 and reusable lesson record |
| `homework/` | Original handwriting, optional transcripts, attempts, and reviews |
| `practice/` | Learner-authored computational experiments |

## Local and remote setup

The delivered ZIP contains this directory with its initialized Git history. Extract it and open a terminal in `modern-math-learning`. The repository already has an initial commit on `main`; do not run another initialization.

```sh
git status
git log -1 --oneline
```

The remote has **not** been created. The connected GitHub tools could read the source repository but exposed no repository-creation action; this session also had no authenticated GitHub CLI. No `origin` has been configured, so there is no fictitious remote.

With Git and the [GitHub CLI](https://cli.github.com/) installed on your computer, authenticate if necessary, then create and push a private remote:

```sh
gh auth login
gh repo create XZUXuVanyu/modern-math-learning --private --source=. --remote=origin --push
```

Run the create command once, only if that remote name is available. `--private` is a suggested initial visibility, not a recorded user preference. If you deliberately want public course records, use `--public` instead. The command uses the existing local commit. See the [official command reference](https://cli.github.com/manual/gh_repo_create).

Alternatively, create an empty GitHub repository named `modern-math-learning` under your account without a generated README, license, or gitignore, and share its URL in this conversation so the prepared files can be uploaded using the existing connection.

After a successful upload, record the verified URL in `program-context.md` and ask to link the scheduled lesson task to the remote checkpoint. The current automation has not been changed to depend on a nonexistent repository.

## New-conversation entry

Read AGENTS.md, learning-agreement.md, program-context.md, progress.md, curriculum.md, and the active lesson and attempt records. Resume the next action recorded in progress.md. Teach one concept at a time and give exactly one homework task. Review my actual handwriting/code, keep uncertain transcription separate from mathematical errors, and do not supply the crucial homework proof or implementation before my attempt.

## Handwriting workflow

Upload the original PNG first. Preserve it even if using Gemini or another model to transcribe it. Check any transcription against the source; place mathematical corrections in a separate revision. See [homework/README.md](homework/README.md).
