# Hero budget, no-regression, self-review

Measure at 1440x900 (desktop) and 390x844 (mobile) when a browser is available. A screen is one viewport height at that size.

## No-regression
A merge, collapse or reorder must not make any single section taller than it was, especially the hero. If pouring section B into A would grow A, keep B below A, collapse B into a closed disclosure, or delete B if it adds no new job. Growing the hero to "finish the merge" is a fail. That is the birthday-page lesson: the prize block joined the hero and the fold got worse.

## Hero budget
- Desktop: hero fits in about 0.75 of a 1440x900 viewport (about 675px), including padding.
- Mobile: hero fits in one 390x844 viewport.
- Above the fold: headline, the core offer, and the primary CTA. A product visual helps if it fits without blowing the budget.
- Details, catalogs, prize lists, extra invites and secondary proof go below the fold or into a closed disclosure.
- If the starting hero is already over budget, shrink it. Do not grow it.

NN/g: the fold still matters. Users scroll when the first screen is promising, not when it is a stuffed full-bleed wall. A hero that fills the viewport with no peek of the next section is a false floor. Do not add a "scroll down" arrow as a substitute for a shorter hero.

Julian Shapiro / Demand Curve: if a stranger reads only the headline, they should know what you sell. Slogan headers fail. The subhead is one or two sentences that make the claim believable. The primary CTA is the next step of that claim, not a vague "Learn more". Do not bloat the header with every objection. That is how heroes grow.

## 5-second test
Look at the above-the-fold screenshot for five seconds, then answer as a stranger:
1. What is this?
2. Who is it for?
3. What should I do next?

NN/g's 5-second test is a first-impression method. Martin's version also uses Shapiro's headline litmus and the Demand Curve ATF questions (what you do, whether you are a fit). If any answer is fuzzy, fix the fold before you report. Do not invent a category, audience or proof to pass the test.

## Visual hierarchy
- One primary CTA style. Repeat the same action later if needed. Do not run two equally loud buttons that ask for different things.
- Clear type scale: one display headline, a smaller subhead, body, quiet captions. Headings should be specific enough to scan (NN/g).
- Scannable chunks. No walls of text. Short paragraphs, lists, real product visuals.
- Mobile tap targets: at least 24x24 CSS px (WCAG 2.2 SC 2.5.8). Primary CTAs should aim for 44x44 (SC 2.5.5). Disclose when you could not measure.
- Collapsed details need a descriptive trigger (NN/g accordions, Baymard trigger indicators). Do not hide the offer, price, legal warning or primary CTA inside a closed panel.

## Self-review loop
After edits, before the report, up to 2 rounds:
1. Screenshot the full page and the fold at 1440x900 and 390x844. If there is no browser, critique from the layout and say estimated.
2. Critique as a skeptical designer, not the author. Check the hero budget, above-the-fold contents, false floor, 5-second answers, one primary CTA, type scale, walls of text, tap targets, and the per-section height table.
3. If anything fails, fix it. A section that grew is an automatic fail.
4. Screenshot again. Stop after 2 fix rounds. If a gate still fails, say so in the report. Do not ship a taller hero and call the loop done.
