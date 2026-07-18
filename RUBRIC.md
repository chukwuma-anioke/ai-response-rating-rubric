# Rubric: Factual Accuracy of AI-Generated Answers

Rate each answer on a 1–5 scale for factual accuracy relative to the question asked. Rate accuracy only. Writing quality, tone, length, and formatting must not affect the score (see `GUIDELINES.md`).

## Scores

### 5 — Fully accurate
Every factual claim in the answer is correct, and the answer addresses the question asked. Minor omissions are fine as long as nothing stated is wrong and nothing essential is missing.

**Anchor:** "Water boils at 100°C (212°F) at standard sea-level pressure. At higher altitudes it boils at lower temperatures."

### 4 — Accurate with a minor flaw
The core answer is correct, but one supporting detail is imprecise, slightly outdated, or overstated. A reader would leave with the right understanding of the main question.

**Anchor:** A correct explanation of photosynthesis that misstates a secondary detail, such as calling chlorophyll "the only" pigment involved.

### 3 — Mixed
The answer contains a roughly even mix of correct and incorrect claims, or the core claim is right but a prominent supporting fact is wrong. A reader would come away partly misinformed.

**Anchor:** "The Great Wall of China is over 13,000 miles long and is easily visible from space with the naked eye." (Length claim defensible; visibility claim is a known myth.)

### 2 — Mostly inaccurate
The central claim is wrong, even if some peripheral details are correct. The answer misleads on the main point of the question.

**Anchor:** "Insulin is produced by the liver" in answer to a question about where insulin is made. (It is produced by the pancreas.)

### 1 — Fabricated or non-responsive
The answer invents specifics (fake statistics, fake sources, fake events), or confidently asserts something with no basis, or does not answer the question at all while appearing to.

**Anchor:** An answer citing a named study, journal, and year that do not exist.

## Error flags

Alongside the score, tag each item with zero or more flags:

- `factual-error` — a verifiably false claim
- `outdated` — was true once, is not current
- `fabrication` — invented specifics (sources, numbers, names, events)
- `partial` — answers only part of the question
- `non-answer` — evades or restates the question without answering
- `overclaim` — states a contested or uncertain thing as settled fact

## Scoring rules

1. Score the answer as written, not the answer the model probably meant.
2. When torn between two scores, write the justification first. The justification usually decides it.
3. One fabricated specific caps the score at 2, regardless of how much else is correct. Fabrication is weighted more heavily than error because it manufactures false confidence.
4. An answer can be a 5 without being complete. It cannot be a 5 with any false statement.
