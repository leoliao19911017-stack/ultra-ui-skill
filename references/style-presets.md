# Style Presets

Selectable, named visual directions. Each preset is a **complete art-direction system** — structure, typography, material, color logic, and interaction — not a palette or a font swap.

## How to use this file

1. **Ask which preset**, or infer one from the brief and say which you chose and why.
2. **Load only the chosen preset** plus the universal checklist at the bottom.
3. **Treat the preset as a starting constraint, not a ceiling.** Deepen it against the real product; do not flatten it into "just use these colors."
4. **Reject the preset** when it conflicts with the product goal, brand commitments, or explicit user requirements. All three axes below must survive contact with the actual brief.

A preset is a *direction with a thesis*. If two presets start producing the same output, that is a failure of application, not a sign the presets are similar.

## Two axes of choice

Presets are organized on two independent axes — pick one from each, or pick a named pair from the combinations table:

- **Axis A — Register**: how formal and how dense is the expression? (Editorial / Industrial / Editorial-technical / Warm-humanist / Brutalist / Luxe-restrained)
- **Axis B — Domain metaphor**: what other field's rules does the interface borrow? (出版 / 工厂 / 地图 / 实验室 / 档案库 / 剧场 / 工程图纸)

## Preset index

| # | Preset | Register | Metaphor | Typical fit |
| --- | --- | --- | --- | --- |
| P1 | `Decision Desk` 决策编辑台 | Editorial | 出版编辑部 | Data collaboration, research, B2B tooling |
| P2 | `Control Plane` 运营控制平面 | Industrial | 工业控制系统 | Ops, monitoring, infrastructure, real-time |
| P3 | `Shared Atlas` 共享数据地图 | Editorial-technical | 地图学 | Spatial data, relationships, exploration |
| P4 | `On Roster` 在册名册 | Archive | 档案库/名册 | People, roster, inventory, catalogs, staff |
| P5 | `Lab Bench` 实验台 | Editorial-technical | 实验室记录 | Scientific, analytics, experiment tooling |
| P6 | `Contract` 合同/勘验单 | Brutalist | 法律文书 | Legal, compliance, audit, certificates |
| P7 | `Atelier` 工坊 | Warm-humanist | 手工作坊 | Craft, wellness, community, education |
| P8 | `Marquee` 剧场场刊 | Luxe-restrained | 剧场节目单 | Events, media, entertainment, launches |
| P9 | `Blueprint` 工程图纸 | Industrial | 工程制图 | Technical specs, hardware, developer tools |
| P10 | `Terminal Ledger` 终端账本 | Industrial | 会计账簿/终端 | Finance, ledgers, transactions, CLIs |

---

## P1 · Decision Desk 决策编辑台

**Thesis.** The interface is a working editorial desk: sources come in, get reconciled, and go out as a published decision. Hierarchy is set by reading order, not by container count.

- **Composition:** Horizontal work surface with one dominant operating zone; persistent status rail at the edge. Alignment and grouping carry the structure — no card grid.
- **Type:** Editorial display face for headlines, tabular/mono for values and metadata, hairline rules to separate sections.
- **Material:** Paper stock, ink, marginalia. Flat surfaces; depth only from rule weight and ink density.
- **Color:** Warm off-white base, ink black, one cobalt or oxidised-blue accent reserved for provenance and links.
- **Motion:** Page-turn calm. Progressions resolve top-to-bottom; state changes acknowledge quickly.
- **Avoidances:** Dashboard tiles, gradient blobs, floating panels, decorative charts, excessive rounding.
- **Risk / cheap validation:** Can feel like a magazine rather than a tool — prototype the primary repeat action first and confirm it reads as an instrument.

## P2 · Control Plane 运营控制平面

**Thesis.** The product is a live system with states; the interface shows the system's condition and lets you act on it. Density is legitimate when it maps to real machinery.

- **Composition:** Full-width pipeline or console; status is always visible; the primary action zone is unambiguous and centred.
- **Type:** Compact grotesk for instructions; tabular figures for readings; casing and weight separate command / status / annotation.
- **Material:** Matte enamel, powder-coated metal, etched markings. Inset depth expressed through borders and light direction, not gloss.
- **Color:** Warm off-black, bone, safety amber and signal red reserved for operational meaning. Solid tonal steps — never gray gradients.
- **Motion:** Mechanical and short, tied to engagement, mode change, and acknowledgement. No floating or looping decoration.
- **Avoidances:** Cartoon skeuomorphism, fake screws, glossy plastic, faux wear, novelty gauges, gray gradients.
- **Risk / cheap validation:** Density can blind rather than inform — validate against a genuinely complex state, not a tidy demo.

## P3 · Shared Atlas 共享数据地图

**Thesis.** Knowledge has geography: things sit near or far from each other, and you zoom to change the question. Relationships are the primary content.

- **Composition:** One central terrain plus edge rails for sources and collaborators. Focus and zoom are the main interactions.
- **Type:** Quiet UI face so labels never fight the terrain; small caps for place names; mono for coordinates and identifiers.
- **Material:** Layered translucent planes, contour lines, plotted paths. Depth signals containment and scale.
- **Color:** Cool gray-blue base, blue-black ink, one coral accent for the current focus.
- **Motion:** Pan, zoom, settle. Motion must preserve orientation — never teleport without a return path.
- **Avoidances:** Decorative globe imagery, gratuitous 3D, force-graph hairballs with no reading order.
- **Risk / cheap validation:** Spatial metaphor can obscure simple lists — test whether a linear task is harder here than in a table.

## P4 · On Roster 在册名册

**Thesis.** Not a brochure — a roster and an inspection form. Everything on the page is a registrable fact with a source, and the viewer's job is to recognise and verify.

- **Composition:** Tabular. Numbered rows, fixed columns, one row per entity. Header block carries register metadata (issue number, date, scope).
- **Type:** Small-caps Latin + heavy CJK display for the register mark; mono throughout the table; footnotes smaller and set apart.
- **Material:** Paper, ink, seal red. Zero gradients, zero glow.
- **Color:** Warm paper base, ink black, one seal-red accent used sparingly for the mark and for emphasis that maps to meaning.
- **Motion:** Almost none. Entries resolve; nothing floats.
- **Avoidances:** Hero imagery with overlay text, testimonial carousels, KPI counters, rounded cards.
- **Risk / cheap validation:** Can read as cold or bureaucratic — verify the first row makes the entity *likeable* in under three seconds.

## P5 · Lab Bench 实验台

**Thesis.** The interface is a record of method. Every claim shows the measurement, the instrument, and the uncertainty.

- **Composition:** Left method rail, central result surface, right annotation margin. Runs and comparisons are the organising unit.
- **Type:** Neutral text face, mono for units and values, generous line spacing for legibility.
- **Material:** Graph paper, ruled charts, precise ticks. Clean and unfussy.
- **Color:** Near-white base, graphite ink, one measured accent (teal or indigo) for the current series.
- **Motion:** Nothing decorative; sweep transitions that reveal a series in reading order.
- **Avoidances:** Fake precision, invented metrics, ornamental charts, drop shadows on data.
- **Risk / cheap validation:** Can expose how thin the real data is — confirm real evidence exists before committing.

## P6 · Contract 合同/勘验单

**Thesis.** The page is an instrument of record. Clauses, fields, and seals; the strength is in what is explicitly agreed and signed.

- **Composition:** Single column, numbered clauses, labelled fields, ruled signature area. Nothing floats outside the document.
- **Type:** Serif or robust text face for body; mono for identifiers, dates, and amounts; all caps for section marks.
- **Material:** Bond paper, carbon copy, stamp ink. Hard edges, no rounding.
- **Color:** Bone base, black, one deep stamp ink (vermilion or oxblood) for the seal and for mandatory markers.
- **Motion:** None. This is a document.
- **Avoidances:** Rounded corners, cards, playful illustration, gradient buttons.
- **Risk / cheap validation:** Can be uninviting for exploratory products — confirm the task really is transactional first.

## P7 · Atelier 工坊

**Thesis.** Made by hand, at human scale. The interface feels worked rather than generated; warmth comes from proportion and material, not from pastel haze.

- **Composition:** Asymmetric but calm; visible craft in spacing and alignment; one clear path with room to breathe.
- **Type:** A humanist serif or a warm sans for reading; hand-influenced display used sparingly; never script clichés.
- **Material:** Linen, uncoated paper, wood, clay. Soft depth from light direction, not gloss.
- **Color:** Ivory, oatmeal, warm clay, muted plant green, deep charcoal text. Low saturation, high warmth.
- **Motion:** Gentle and physical, like handling an object. Nothing bouncy.
- **Avoidances:** Pastel haze, inflated radii, craft-signalling stickers, "artisanal" clichés.
- **Risk / cheap validation:** Warmth can slide into mush — verify contrast and edge definition survive.

## P8 · Marquee 剧场场刊

**Thesis.** A programme for an event: the work is the star, the interface frames it and stays out of the way.

- **Composition:** Strong scale contrast; a poster-like opening, then a programme listing; generous margins.
- **Type:** High-contrast display face for titles, restrained text face for detail; dramatic size jumps are the hierarchy.
- **Material:** Coated stock, ink, stage light. Deep base with controlled highlights.
- **Color:** Near-black base, bone text, one saturated spot colour per production.
- **Motion:** Curtain-like reveals; content arrives, then holds still.
- **Avoidances:** Glossy gradients, gold accents by default, generic luxury clichés.
- **Risk / cheap validation:** Can become style over substance — confirm the actual content list is strong enough to carry it.

## P9 · Blueprint 工程图纸

**Thesis.** The interface is a drawing: precise, dimensioned, and annotated. Precision is the aesthetic.

- **Composition:** Orthogonal grid, measured gutters, dimension lines, callout annotations, title block.
- **Type:** Technical face and mono for labels; all-caps for drawing marks; consistent text height discipline.
- **Material:** Drafting paper, drafting pen, grid. No shadow, no gloss.
- **Color:** Blueprint blue or drafting white base with a single ink colour; accent only for the active dimension.
- **Motion:** Draw-on transitions that trace, measure, then settle.
- **Avoidances:** Decorative 3D renders, sketchy hand-drawn effects, glow.
- **Risk / cheap validation:** Can be cold for consumer products — validate against a real user who is not an engineer.

## P10 · Terminal Ledger 终端账本

**Thesis.** Money and events as a running record. Absolute legibility of value and change, with provenance always one step away.

- **Composition:** Ledger rows; debit/credit logic; running totals pinned; one filter surface.
- **Type:** Mono or tabular figures throughout for values; a plain face for prose; right-aligned numerics.
- **Material:** Thermal print, ledger paper, dot-matrix texture used with restraint.
- **Color:** Near-white or near-black base, graphite ink, one green/red pair **only** for signed meaning (never decorative).
- **Motion:** Row insertion and settlement only.
- **Avoidances:** Abstract "fintech gradient" purple/blue, glowing numbers, confetti-like decoration.
- **Risk / cheap validation:** Can feel austere — verify the primary value is instantly readable.

---

## Named combinations

Use when the brief is clear but the register is not.

| Combination | Composition | Type | Color | Fit |
| --- | --- | --- | --- | --- |
| `Decision Desk` × `Lab Bench` | Method rail + editorial desk | Editorial display + mono | Paper + indigo | Analytics with narrative |
| `Control Plane` × `Blueprint` | Dimensioned console | Grotesk + technical | Off-black + amber | Hardware, developer tooling |
| `On Roster` × `Contract` | Tabular record + seals | Small caps + mono | Paper + vermilion | Compliance registers, audit |
| `Atelier` × `Marquee` | Calm canvas + poster opening | Humanist + display | Ivory + one spot | Creative studios, portfolios |
| `Shared Atlas` × `Lab Bench` | Terrain + measurement rail | Quiet UI + mono | Gray-blue + teal | Research exploration tools |
| `Terminal Ledger` × `On Roster` | Ledger rows + roster columns | Tabular mono | Ledger paper + stamp | Finance registers, inventories |

---

## Universal checklist (applies to every preset)

Regardless of preset, every direction must state:

- **Thesis** in one sentence.
- **How it differs** from the three most likely category peers.
- **Largest risk** and the **cheapest way** to validate it.
- **Explicit avoidances** — what this direction refuses to do.

And every delivery must survive:

- Real content and long text; empty, error, and loading states.
- Keyboard navigation with visible focus; reduced-motion honoured.
- Sufficient contrast; mobile layouts; performance budget.
- No fabricated logos, metrics, integrations, or testimonials.

## Provenance

These presets are **production heuristics authored for this skill**, extending the method described in the source article. They are not quotations from, or claims by, the source author. Treat them as a starting vocabulary, not a canon — add project-specific presets as they prove themselves, and retire any preset that stops producing distinct work.
