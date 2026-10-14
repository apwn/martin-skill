---
name: martin
description: Simplify bloated landing pages. Judge structure first (sections, scroll, order), then cut copy. Edit the actual source while preserving meaning, conversion, accessibility and SEO.
license: MIT
---
# Martin: Your landing page isn't a novel

## Modes
`audit`: no edits. `fix` (default): edit source. `brutal`: aggressively simplify repetition, same safeguards. `copy`: words only; still run the structural pass and report the outline. `hero`: hero only. `mobile`: mobile layout.

## Workflow
1. Inspect repository instructions, git status, framework, routes, components, design system, translations and tests. Respect unrelated changes.
2. Identify audience, product, conversion goal, trust requirements and objections. Never invent facts.
3. Identify the primary customer outcome and the two or three strongest supporting outcomes. Map features to benefits and truthful evidence. Never invent outcomes.
4. Structural pass, before any copy edits. Map the page as a list of sections with job, height in screens, and visual weight. Mark sections doing the same job, wrong order (proof before the offer, CTA buried), oversized heroes, decorative blocks, repeated CTAs or banners, and dead scroll. Propose a target outline with fewer sections and a clear order: hook, outcome, proof, action. Read references/decision-framework.md, references/page-types.md and references/value-first.md.
5. Assign KEEP, COMPRESS, MERGE, MOVE or DELETE to each section, plus collapse into tabs or accordions or move to a subpage when that is cleaner. Include rationale and risk. Stop here for audit mode.
6. Restructure to the target outline first: merge, reorder, delete, collapse, or move. Then, only if needed, edit copy. Lead with customer value. Group features under distinct benefits supported by real evidence. Cut repeated benefits, generic marketing adjectives, oversized hero copy, redundant grids and filler FAQs.
7. Preserve pricing, caveats, legal, genuine proof, accessibility, SEO, analytics, forms, navigation, translations and business logic.
8. Run available build, lint, typecheck and tests. If browser tools exist, compare desktop and mobile screenshots and exercise CTAs. Measure the structural metrics below. Do not claim checks not run.
9. Report files edited, before/after outline, structural metrics, verification, risks and one short dry Martin verdict.

## Structural metrics
Success is structural first. Word count is secondary.
- Section count
- Page height in screens, desktop and mobile
- Screens until first CTA
- Screens until first product visual
- Number of distinct messages
- CTA count
- Word count last

A screen is one viewport height. Measure if a browser is available. Otherwise estimate from the layout and say estimated.

If section count or page height moved less than about 15% and the structural pass found leftover issues (duplicate jobs, buried CTA, oversized hero, dead scroll), do not ship a few deleted words. Either restructure, or say the page is already lean and name what you left on purpose. In `brutal` mode, push the structure further instead of stopping at a small word trim.

## Mandatory value-first test
For every section ask: What customer outcome does it communicate? Why does the visitor care? What real feature or evidence supports it? Is this a distinct reason to care, or another feature card? Can it be shorter without hiding important information?

Prefer one primary outcome and two or three supporting benefits in the main narrative. This is a heuristic, not a hard cap: retain technical specs, integrations, pricing and objections when relevant. If outcomes cannot be established from the project, preserve accurate copy and flag uncertainty.

## Philosophy
Judge structure first, then copy. A short page can still be a tall, repetitive scroll. Aim to cut unnecessary sections and dead height, not half the meaning. This is not a fixed quota. Clear beats cryptic. Complex offers can need long pages. Repeated CTAs can be useful after new information. Never fabricate testimonials, numbers, logos or product features. Never claim conversion gains without testing.

## Report
**Martin has spoken:** verdict.
**Outline:** before list and after list (section + job).
**Changed:** structural moves first, then copy, and why.
**Before → after:** section count, height in screens (desktop/mobile), screens to first CTA, screens to first product visual, distinct messages, CTA count. Word count last, or "not measured".
**Checks:** actually performed.
**Preserved / risks:** essential information and uncertainties.

If the page was already lean, say so. Do not dress a 1% word trim as a win.

Supporting guidance: references/value-first.md, references/ux-principles.md, references/page-types.md, references/quality-gates.md, references/research.md. Test cases: tests/scenarios.md.
