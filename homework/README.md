# Handwriting, transcription, and review

Recommended default: submit the original image. A verified transcription is an optional companion, never a replacement for the original mathematical record.

| Material | Purpose | Treatment |
| --- | --- | --- |
| `M001/raw/attempt-01-page-01.png` | Evidence of the learner's actual work | Preserve original pixels and page order |
| `M001/attempt.md` | Attempt metadata and learner feedback | Learner fills in time, obstacle, and assistance |
| `M001/transcribed/attempt-01.tex` | Searchable/typeset copy | Optional; initially unchecked, compare against raw |
| `M001/review.md` | Tutor feedback | Separate transcription uncertainty from mathematical error |
| `M001/raw/attempt-02-page-01.png` | Revised learner reasoning | New attempt; keep the earlier image |

Use one clearly legible page per image. Keep original screenshots or exports at their native resolution. If taking photos, avoid shadows and perspective distortion; preserve the source photo if producing a crop. Diagrams, arrows, crossed-out steps, and margin notes can matter. PNG is suitable for digital handwriting; converting a JPEG to PNG does not restore lost detail. A source PDF may also be preserved alongside page images.

## Why keep both when transcribing?

Images preserve notation and the actual reasoning trail. Text supports searching, Git diffs, reuse, and typesetting. Transcription can misread signs, indices, quantifiers, and diagram labels; plausible output is not evidence of faithful transcription. The original resolves disputes. No claim is made that Gemini is more accurate than another model for your handwriting; that would require checking representative pages.

## Transcription instructions

When using Gemini or another transcriber, request a faithful LaTeX transcription only. Preserve mathematical errors, missing steps, line order, and meaningful cancellations. Do not solve, simplify, complete, or repair the proof. Flag unreadable marks with an explicit placeholder and the page/region reference; list possible readings separately when helpful. Keep diagrams as references to the original image unless their content can be represented faithfully. Return uncertainties separately from the transcription.

Initially label the result `unchecked` in attempt.md and in a TeX comment. Compare it line by line to the PNG, especially minus signs, subscripts, inverse notation, equality/implication signs, and quantifiers. Change the label only after review. If a symbol remains ambiguous, ask the learner; do not infer it solely from what would make the mathematics correct.

Checking transcription means checking fidelity, not mathematical correctness. Keep later mathematical revisions in a new attempt. Rendering successfully also does not validate a proof.

Markdown with LaTeX equations is sufficient for short answers. Standalone .tex is useful for substantial derivations or documents intended for compilation. Neither is mandatory for receiving feedback.

No images or completed answers have been submitted yet; the paths above are naming examples.
