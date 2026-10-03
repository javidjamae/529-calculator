# The 529 Question

Should that money go in a 529? This calculator compares a 529 plan against an ordinary taxable brokerage account and shows which one leaves you with more after tax.

**Use it:** https://javidjamae.github.io/529-calculator/

Built for [Money Well Studio](https://moneywellstudio.com), the podcast where Jennifer and Julie talk money, for College Series Part 2.

## What it models

- **A real age-based glide path.** The 529 follows Vanguard's published Target Enrollment allocations (1 July 2026), stepping down from about 95% stocks to about 12% by enrollment. The taxable account holds one flat rate.
- **When you fund it.** From years before birth to senior year. Time to compound is most of the story.
- **Certainty.** What share of the money gets spent on qualified expenses. Earnings on the rest are taxed as ordinary income plus the 10% additional tax.
- **Federal tax.** Long-term capital gains rate, the 3.8% net investment income tax, and an optional tax-loss harvesting offset for the taxable account.
- **State benefit.** Your state income tax rate and the deductible cap.

It also shows the breakeven return the taxable account needs to tie, the cost of walking away from the 529 today, and a year-by-year table.

This calculator is an educational model and does not give tax advice.

## Running and editing the calculator

The whole calculator is one file, `index.html`, with plain JavaScript and no dependencies or build step.

- Open the link above to use it, or download `index.html` and open it in any browser.
- Press `.` on this repo to edit the code in GitHub's web editor.
- To host your own copy, fork the repo, then turn on GitHub Pages under Settings, Pages, deploying from the `main` branch.

## Updating the numbers each year

Some figures change every tax year:

- `GIFT_EXCLUSION` and `STATE_CAP_RANGE` near the top of the script drive the notes under the amount slider.
- The `GLIDE` table holds the Vanguard allocations. Replace it when Vanguard publishes a new schedule.
- The explanation sections at the bottom quote the 2026 gift figures ($19,000, $95,000, $190,000) and the glide path date in prose. Update them to match.

## Sources

IRS Publication 970 (qualified expenses, earnings versus basis, the additional tax), IRS *529 Plans: Questions and Answers*, IRS Topic 559 (NIIT thresholds), SECURE 2.0 section 126 (Roth rollover), and Vanguard's Target Enrollment Portfolio allocations.

## License

MIT. Use it, change it, share it.
