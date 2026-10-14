# ✂️ Martin

Your landing page isn't a novel. Martin finds the one outcome a visitor came for, then edits your site so that shows up first.

```bash
git clone https://github.com/apwn/martin-skill ~/.claude/skills/martin
```

Codex: clone to `~/.agents/skills/martin`. Then open the site repo and run `/martin`.

## Origin

Martin Tale ([@MartinTale](https://x.com/MartinTale)) told me my landing pages had too much copy and would work better if I cut it roughly in half and got straight to the point.

![Martin Tale on cutting landing page copy](assets/martin-tweet.jpg)

This skill turns that advice into an automated coding workflow. A playful homage, not an official endorsement by Martin Tale.

## What it does

Martin inspects the page, names the primary customer outcome, and marks each section KEEP, COMPRESS, MERGE, MOVE or DELETE. Features get clustered under real benefits, not listed as a catalog. Then it edits the source. Pricing, genuine proof, legal copy, accessibility, SEO and working UI stay.

| Mode | Behavior |
|---|---|
| `fix` (default) | Edits the website code |
| `audit` | Recommendations only |
| `brutal` | Cuts harder at repetition, same safeguards |
| `copy` | Text only |
| `hero` | Hero clarity and size |
| `mobile` | Mobile hierarchy and clutter |

Ask in plain language: `Use Martin in brutal mode on my homepage`.

## Example: [level39.fun](https://level39.fun)

The page already knew what it was selling. It just said "beat level 39" four times before anyone learned a jump.

It was already lean. Martin made small targeted cuts, not a half-page rewrite.

<table>
  <tr>
    <td align="center"><img src="assets/level39-before.png" alt="level39.fun mobile before" width="300" /><br>Before</td>
    <td align="center"><img src="assets/level39-after.png" alt="level39.fun mobile after" width="300" /><br>After</td>
  </tr>
</table>

Desktop: 473 → 467 visible words. Mobile: 470 → 442 words, page height 4479 → 4273 px. Tests and build passed.

MIT. See [LICENSE](LICENSE).

Research, limits and the decision notes are in [references/](references/).
