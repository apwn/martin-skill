---
name: martin
description: Simplify bloated landing pages. Judge structure first, cap the hero, then cut copy. Edit the actual source while preserving meaning, conversion, accessibility and SEO.
license: MIT
---
# Martin: Your landing page isn't a novel

## Modes
`audit`: no edits. `fix` (default): edit source. `brutal`: aggressively simplify repetition, same safeguards. `copy`: words only; still run the structural pass and report the outline. `hero`: hero only. `mobile`: mobile layout.

## Workflow
1. Inspect repository instructions, git status, framework, routes, components, design system, translations and tests. Respect unrelated changes.
2. Identify audience, product, conversion goal, trust requirements and objections. Never invent facts.
3. Identify the primary customer outcome and the two or three strongest supporting outcomes. Map features to benefits and truthful evidence. Never invent outcomes.
4. Structural pass, before any copy edits. Map the page as a list of sections with job, height in screens, and visual weight. Mark sections doing the same job, wrong order (proof before the offer, CTA buried), oversized heroes, decorative blocks, repeated CTAs or banners, and dead scroll. Propose a target outline with fewer sections and a clear order: hook, outcome, proof, action. Read references/decision-framework.md, references/page-types.md, references/value-first.md and references/hero-and-review.md.
5. Assign KEEP, COMPRESS, MERGE, MOVE or DELETE to each section, plus collapse into tabs or accordions or move to a subpage when that is cleaner. Include rationale and risk. Stop here for audit mode.
6. Restructure to the target outline first: merge, reorder, delete, collapse, or move. A merge must not make any section taller, especially the hero. Details go below the fold or into disclosure. Then, only if needed, edit copy. Lead with customer value. Group features under distinct benefits supported by real evidence.
7. Preserve pricing, caveats, legal, genuine proof, accessibility, SEO, analytics, forms, navigation, translations and business logic.
8. Self-review loop, up to 2 rounds, before you report. Screenshot desktop 1440x900 and mobile 390x844 if a browser is available. Critique as a skeptical designer against the gates in references/hero-and-review.md (above-the-fold test, 5-second test, hierarchy, per-section heights). Fix failures and repeat. Then run available build, lint, typecheck and tests. Do not claim checks not run.
9. Report files edited, before/after outline, per-section heights, structural metrics, self-review rounds, verification, risks and one short dry Martin verdict.

## No-regression and hero
A merge that grows the hero, or any other section, is a fail. Hero budget: about 0.75 of a 1440x900 desktop viewport, and one 390x844 mobile viewport, with headline, the core offer and the primary CTA above the fold. If the starting hero is already over budget, shrink it. Do not grow it.

## Structural metrics
Success is structural first. Word count is secondary.
- Section count
- Page height in screens, desktop and mobile
- Per-section height before and after (flag any section that grew)
- Screens until first CTA
- Screens until first product visual
- Number of distinct messages
- CTA count
- Word count last

A screen is one viewport height at 1440x900 (desktop) or 390x844 (mobile). Measure if a browser is available. Otherwise estimate from the layout and say estimated.

If section count or page height moved less than about 15% and the structural pass found leftover issues, do not ship a few deleted words. Either restructure, or say the page is already lean and name what you left on purpose. In `brutal` mode, push the structure further instead of stopping at a small word trim.

## Mandatory value-first test
For every section ask: What customer outcome does it communicate? Why does the visitor care? What real feature or evidence supports it? Is this a distinct reason to care, or another feature card? Can it be shorter without hiding important information?

Prefer one primary outcome and two or three supporting benefits in the main narrative. This is a heuristic, not a hard cap. If outcomes cannot be established from the project, preserve accurate copy and flag uncertainty.

## Philosophy
Judge structure first, then copy. A short page can still be a tall, repetitive scroll. Aim to cut unnecessary sections and dead height, not half the meaning. Clear beats cryptic. Never fabricate testimonials, numbers, logos or product features. Never claim conversion gains without testing.

## Report
**Martin has spoken:** verdict.
**Outline:** before list and after list (section + job).
**Heights:** per-section before/after table. Flag any section that grew.
**Changed:** structural moves first, then copy, and why.
**Before → after:** section count, height in screens (desktop/mobile), screens to first CTA, screens to first product visual, distinct messages, CTA count. Word count last, or "not measured".
**Self-review:** rounds run, what failed, what you fixed. If a browser was missing, say so.
**Checks:** actually performed.
**Preserved / risks:** essential information and uncertainties.

If the page was already lean, say so. Do not dress a 1% word trim as a win.

Supporting guidance: references/hero-and-review.md, references/value-first.md, references/ux-principles.md, references/page-types.md, references/quality-gates.md, references/research.md. Test cases: tests/scenarios.md.
