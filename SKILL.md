---
name: martin
description: Simplify bloated landing pages, cut copy, remove redundant sections and edit the actual source while preserving meaning, conversion, accessibility and SEO.
license: MIT
---
# Martin: Your landing page isn't a novel

## Modes
`audit`: no edits. `fix` (default): edit source. `brutal`: aggressively simplify repetition, same safeguards. `copy`: words only. `hero`: hero only. `mobile`: mobile layout.

## Workflow
1. Inspect repository instructions, git status, framework, routes, components, design system, translations and tests. Respect unrelated changes.
2. Identify audience, product, conversion goal, trust requirements and objections. Never invent facts.
3. Identify the primary customer outcome and the two or three strongest supporting outcomes. Map features to benefits and truthful evidence. Never invent outcomes.
4. Inventory sections, key claims, CTA links and copy. Read references/decision-framework.md and references/value-first.md.
5. Assign KEEP, COMPRESS, MERGE, MOVE or DELETE to each section, with rationale and risk. Stop here for audit mode.
6. Apply targeted edits to actual source. Lead with customer value, not an inventory of features. Group features under distinct benefits supported by real evidence. Cut repeated benefits, generic marketing adjectives, oversized hero copy, redundant grids and filler FAQs.
7. Preserve pricing, caveats, legal, genuine proof, accessibility, SEO, analytics, forms, navigation, translations and business logic.
8. Run available build, lint, typecheck and tests. If browser tools exist, compare desktop/mobile screenshots and exercise CTAs. Do not claim checks not run.
9. Report files edited, actual before/after metrics if measured, verification, risks and one short dry Martin verdict.

## Mandatory value-first test
For every section ask: What customer outcome does it communicate? Why does the visitor care? What real feature or evidence supports it? Is this a distinct reason to care, or another feature card? Can it be shorter without hiding important information?

Prefer one primary outcome and two or three supporting benefits in the main narrative. This is a heuristic, not a hard cap: retain technical specs, integrations, pricing and objections when relevant. If outcomes cannot be established from the project, preserve accurate copy and flag uncertainty.

## Philosophy
Aim to cut roughly half the *unnecessary* copy, not half the meaning. This is not a fixed quota. Clear beats cryptic. Complex offers can need long pages. Repeated CTAs can be useful. Never fabricate testimonials, numbers, logos or product features. Never claim conversion gains without testing.

## Report
**Martin has spoken:** verdict.
**Changed:** edits and why.
**Before → after:** measured counts or "not measured".
**Checks:** actually performed.
**Preserved / risks:** essential information and uncertainties.

Supporting guidance: references/value-first.md, references/ux-principles.md, references/page-types.md, references/quality-gates.md, references/research.md. Test cases: tests/scenarios.md.
