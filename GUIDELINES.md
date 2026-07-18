# Annotation Guidelines

These rules govern how the rubric in `RUBRIC.md` is applied. When the rubric and a guideline seem to conflict, the guideline wins, and the conflict gets logged in `notes/hard-cases.md`.

## Scope

- Rate factual accuracy only. An unhelpful but accurate answer can score 5. A helpful, well-written answer full of errors scores low.
- Rate against generally accepted knowledge as of the rating date. If a claim can't be verified either way, treat it under rule 6, not as false.

## Workflow

1. Read the question first and decide what a correct answer must contain before reading the response.
2. Read the response once fully, then a second time claim by claim.
3. Verify any specific number, date, name, or citation you are not certain of.
4. Write the justification (1–2 sentences), then assign the score, then add flags.
5. Never revise a justification to fit a score you already wanted to give. Revise the score.

## Edge-case rules

**Rule 1 — Style is invisible.** Confident tone, hedged tone, good grammar, bad grammar: none of it moves the score. This rule exists because fluency bias is the most common annotator failure.

**Rule 2 — Omission vs. error.** Leaving out relevant information is not an error unless the omission changes the meaning of what was said. "Abuja is Nigeria's capital" is a 5 even without mentioning Lagos was the capital before 1991. "Lagos is Nigeria's capital" is a 2 with an `outdated` flag.

**Rule 3 — Hedged wrongness is still wrong.** "It may be that insulin is produced in the liver" contains the same false claim as the confident version. Hedging does not upgrade the score; it only avoids an `overclaim` flag.

**Rule 4 — Correct core, wrong detail.** If the direct answer to the question is right but a supporting fact is false, score 4 when the false detail is peripheral and 3 when a reader would likely remember and repeat it.

**Rule 5 — Fabrication cap.** Any invented source, statistic, or named specific caps the score at 2 (rubric rule 3). If unsure whether a citation is real, attempt to verify; if it cannot be found through a reasonable search, flag `fabrication` and note the uncertainty in the justification.

**Rule 6 — Unverifiable claims.** A claim that cannot be confirmed or refuted does not lower the score by itself, but more than one unverifiable specific in a factual answer earns an `overclaim` flag and a note.

**Rule 7 — Non-answers.** A response that restates the question, gives generic filler, or answers a different question scores 1 with a `non-answer` flag, even if every sentence in it is technically true.

## When unsure

Log the item in `notes/hard-cases.md` with the two candidate scores and the reasoning for each, pick the lower score, and move on. Consistency across items matters more than winning any single item.
