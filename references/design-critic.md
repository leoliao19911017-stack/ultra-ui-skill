# Design Critic

## When to use it

Use a critic after the first coherent build, when the visual direction is not surviving implementation, when revisions have collapsed into local detail-polishing, or before a major delivery. Do not require this ceremony for a simple, low-risk change.

## Isolate the review

The critic must run in a fresh context. Give it only:

- the product goal;
- the target audience;
- the platform and relevant constraints;
- a screenshot of the current interface; and
- optional visual references.

Do not provide code, implementation cost, earlier criticism, the designer's rationale, or a target score. Those inputs anchor the critic to explanations instead of visible evidence.

The screenshot must represent a real viewport and state, at a useful resolution. Include other states or breakpoints only when they are actually under review. If no visual-review tool is available, say so and perform a structured self-review; do not describe it as independent criticism.

## Critic prompt

```text
Act as an independent product-design critic. Review only the supplied goal,
audience, platform constraints, screenshot, and optional references.

Assess composition, hierarchy, typography, color, material, imagery, motion,
coherence, product clarity, and accessibility. Identify overdone, stale, or
recognizably AI-generated patterns. When references are supplied, name the
largest quality gap between the current work and that professional baseline.
Judge what is visible; do not infer implementation intent.

Return:
1. Intended aesthetic — what the interface appears to be trying to achieve.
2. Studio-level bar — what excellent execution would require here.
3. Largest gaps — at most three, ranked by user and visual impact.
4. Specific next changes — concrete revisions tied to those gaps.
5. Production risks — usability, accessibility, responsive, content, or motion risks.
6. Quality signal — 1–10, supported by visible evidence rather than taste alone.
```

## Use references as a bar, not a template

Visual references establish quality, atmosphere, finish, and category ambition. Never copy their composition, assets, brand elements, or signature details.

A strong comparison mixes several professional references—often four—and the current screenshot, then asks the critic to rank or compare them without disclosing which is the current work. Adjust the count to the task; the value comes from calibrated comparison, not a fixed number.

## Iterate with a bounded loop

Start with one or two rounds. In each round, fix only the highest-impact gaps, capture the same real viewport and state again, and reuse the same critic prompt so the measuring stick stays stable. Continue only while feedback is converging: the largest gaps should shrink or become more specific, not churn into unrelated preferences.

Stop when the critical gaps are resolved, the product goal and any explicit user quality bar are met, no high-priority usability issue remains, and another round is expected to produce only marginal improvement. The score is a signal, not a mechanical gate. Set this stopping condition before iterating so critique cannot become an open-ended token burn.
