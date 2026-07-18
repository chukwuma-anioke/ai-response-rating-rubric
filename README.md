# AI Response Rating: A Rubric-Based Evaluation Exercise

A self-directed annotation project. I used Claude to design a 5-point rubric for rating the factual accuracy of AI-generated answers, wrote annotation guidelines with edge-case rules, and applied the rubric to a set of 20 question–answer pairs, recording a score and a written justification for each.

The goal was to practice the core skills of AI training and evaluation work: applying a fixed rubric consistently, separating factual accuracy from writing quality, catching hallucinations, and justifying every judgment in one or two sentences.

## What's in this repo

| File | What it is |
|---|---|
| `RUBRIC.md` | The 5-point scoring rubric with anchors and examples for each score |
| `GUIDELINES.md` | Annotation guidelines: scope, edge-case rules, and what to do when unsure |
| `items.csv` | 20 question–answer pairs to be rated |
| `ratings.csv` | My score, justification, and error flags for each item |
| `hard-cases.md` | Items where the rubric was hard to apply, and how I resolved them |
| `consistency-check.md` | A re-rating of a sample one week later, with agreement results |

## How the dataset was built

The answers in `items.csv` were generated and curated specifically for this exercise. Some are fully correct, and others contain seeded problems: factual errors, outdated information, fabricated specifics, partial answers, and confident non-answers. Building the set this way means each item has a known ground truth to check my ratings against, and it avoids using any material from client platforms, which contributor agreements prohibit sharing.

## What I learned

- The hardest ratings are not wrong answers but partially right ones. The rubric needed an explicit rule for "correct core claim, wrong supporting detail" (see `GUIDELINES.md`, rule 4).
- Fluent writing pulls ratings upward. Scoring accuracy blind to style takes deliberate effort, which is why the rubric forbids rewarding tone.
- A justification requirement changes the rating itself. Having to defend a score in one sentence caught several ratings I would otherwise have given on gut feel.

## Method notes

Each item was rated in a single pass, justification first, score second. One week later I re-rated a random sample of items without looking at my original scores and recorded the agreement rate in `consistency-check.md`.
