# Creative Direction

## Frame the work

Before exploring, record the product, audience, primary job, real content, platform, brand commitments, accessibility needs, performance budget, and implementation constraints. Treat explicit user choices as constraints, not invitations to redesign the assignment.

## Generate meaningful alternatives

Explore at least three directions that differ in structure, typographic logic, visual metaphor, material treatment, color logic, and interaction principles. A palette swap or a new font on the same layout is one direction, not several.

Ideas that sound risky can be prototyped cheaply before being rejected. Novelty never excuses ignoring usability, accessibility, product constraints, or the user's explicit requirements.

If the user has already selected a direction, deepen and validate it instead of forcing the project back into open exploration. Reopen direction work only when the chosen approach conflicts with the product goal or stated constraints.

### Optional seed string

Use a long random seed string only when familiar patterns keep pulling the work toward the default distribution. Generate it locally, then privately extract possible segmentation, repetition, numeric emphasis, or rhythm. The seed is an inspiration constraint, not product content: it must not enter the interface, copy, data, or any default deliverable. Keep it private by default; provide it only when the user explicitly asks for it or when an authorized audit or reproduction workflow requires it.

PowerShell (optional):

```powershell
-join (1..64 | ForEach-Object { [char](Get-Random -InputObject ((48..57) + (65..90) + (97..122))) })
```

POSIX (optional):

```sh
od -An -N32 -tx1 /dev/urandom | tr -d ' \n'; printf '\n'
```

### Cross-domain inspiration

Borrow the rules of another field: its cadence, hierarchy, tolerances, sequencing, or material logic. Translate those rules into interface behavior. Do not paste on the field's surface symbols or decorative clichés.

## Convert taste reactions into constraints

Do not debate whether a reaction is technically precise. Translate it into an observable implication and a deliberate avoidance.

| Reaction | Design implication | Explicit avoidance |
| --- | --- | --- |
| “More editorial” | Strong scale contrast, deliberate reading order, fewer simultaneous focal points | Dashboard density and interchangeable cards |
| “Too soft” | Sharper edges, firmer spacing, higher-contrast type, decisive states | Pastel haze, inflated radii, low-contrast controls |
| “Make it feel alive” | State-linked motion and responsive feedback | Ambient motion with no interaction meaning |
| “More premium” | Better proportion, restraint, typography, imagery, and finish | Gold accents, gloss, or luxury clichés by default |
| “Less busy” | Consolidate actions and establish one dominant path | Hiding necessary information without improving hierarchy |

## One complete brief example

Input: “Industrial console, highly tactile; not cartoonish or tacky skeuomorphic; no gray gradients.”

- **Composition:** A dense but legible work surface organized around one primary operating zone, with persistent system status and a narrow contextual rail. Use alignment and grouping to communicate machinery-like order rather than filling a card grid.
- **Components:** Robust switches, segmented modes, calibrated sliders, explicit alarms, and readouts with large click targets. Controls should reveal state through position, label, and contrast—not ornamental chrome.
- **Material:** Matte enamel, powder-coated metal, etched markings, and restrained inset depth expressed through borders, texture, and light direction. Keep effects subtle enough to preserve clarity.
- **Color:** Warm off-black and bone as the base, with safety amber and signal red reserved for operational meaning; use solid tonal steps instead of gray gradients.
- **Type:** A compact grotesk for instructions and a tabular technical face for values. Use casing, weight, and spacing to separate command, status, and annotation.
- **Motion:** Short, mechanical transitions tied to control engagement, mode changes, acknowledgement, and system response. No floating, bouncy, or decorative loops.
- **Avoidances:** Cartoon knobs, fake screws, glossy plastic, faux wear, excessive shadows, novelty gauges, gray gradients, and nostalgia that weakens usability.

## Direction check

For each direction, write one sentence stating its thesis, how it differs from common category peers, its largest risk, and the cheapest way to validate that risk.
