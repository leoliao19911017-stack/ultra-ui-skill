# Design Critic

## When to use it

Use a critic after the first coherent build, when the visual direction is not surviving implementation, when revisions have collapsed into local detail-polishing, or before a major delivery. Do not require this ceremony for a simple, low-risk change.

## Isolate the review

The critic must run in a fresh context. Give it only:

- the product goal;
- a screenshot of the current interface;
- the platform and relevant constraints; and
- an optional moodboard.

Do not provide code, implementation cost, earlier criticism, the designer's rationale, or a target score. Those inputs anchor the critic to explanations instead of visible evidence.

The screenshot must represent a real viewport and state, at a useful resolution. Include other states or breakpoints only when they are actually under review. A static screenshot supports only visible judgments: never infer motion, interaction, keyboard or focus behavior, responsive behavior, loading or error states, content variants or overflow behavior, or accessibility behavior from it. If no visual-review tool is available, say so and perform a structured self-review; do not describe it as independent criticism.

## Critic prompt

```text
Act as an independent product-design critic. Review only the supplied product
goal, current interface screenshot, platform and relevant constraints, and
optional moodboard.

Assess the visible composition, hierarchy, typography, color, material, imagery,
coherence, product clarity, and accessibility signals. Identify overdone, stale,
or recognizably AI-generated patterns. When a moodboard is supplied, name the
largest visible quality gap between the current work and that baseline. Judge only
what the evidence shows; do not infer implementation intent or behavior.

Return:
1. Intended aesthetic — what the interface appears to be trying to achieve.
2. Studio-level bar — what excellent execution would require here.
3. Observed gaps — at most three, ranked by user and visual impact, each supported
   only by visible evidence.
4. Unverified risks / required evidence — for motion, keyboard and focus behavior,
   responsive behavior, loading and error states, content variants or overflow, or
   accessibility behavior that the supplied material cannot confirm, write
   "not observable from supplied evidence" and name the video, multi-state or
   breakpoint screenshots, or interaction checks needed to verify it. Do not guess.
5. Specific next changes — exactly three concrete revisions, ranked by priority,
   with each revision explicitly tied to an observed gap.
6. Production risks — visible usability or delivery risks, clearly separated from
   the unverified risks above.
7. Quality signal — 1–10, supported by visible evidence rather than taste alone.
```

## Use references as a bar, not a template

Visual references establish quality, atmosphere, finish, and category ambition. Never copy their composition, assets, brand elements, or signature details.

### Blind calibration

A strong comparison uses a separate blind-calibration stage. Mix several professional references—often four—with the current screenshot, label the images anonymously (for example, A–E), and ask the critic only for a ranking and visible evidence for each image. Do not reveal or ask it to guess which image is the current work, and do not request revision advice in this call.

```text
Rank the anonymous images A–E against the supplied product goal and professional
quality bar. Return only the ranking and image-by-image visible evidence. Do not
guess which image is the current work and do not recommend changes.
```

After the blind ranking, the outer agent maps the anonymous label to the current work. Then run the identified current screenshot through the critic prompt above in a separate call to obtain gaps and revision advice. Do not combine blind calibration and current-work improvement in one call. Adjust the reference count and labels to the task; the value comes from calibrated comparison, not a fixed number.

## Iterate with a bounded loop

The default critic loop has a hard limit of two rounds. In each round, fix only the highest-impact observed gaps, capture the same real viewport and state again, and reuse the same critic prompt so the measuring stick stays stable. Continue within that limit only while feedback is converging: the largest gaps should shrink or become more specific, not churn into unrelated preferences.

Stop earlier when the critical gaps are resolved, the product goal and any explicit user quality bar are met, no high-priority usability issue remains, and another round is expected to produce only marginal improvement. After round two, stop and report any remaining gaps; continue only with explicit user authorization. The score is a signal, not a mechanical gate. Set this stopping condition before iterating so critique cannot become an open-ended token burn.
