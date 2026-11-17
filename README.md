# MLB Payroll-Adjusted Standings Simulator

**Live:** https://woyakn77-create.github.io/mlb-payroll-simulator/ · [Back to portfolio](https://woyakn77-create.github.io/portfolio/)

What would the standings look like if every team's runs were scaled by how much it spends? Every regular-season game (2,429 in 2026, 2,106 in 1982) is replayed with each team's runs multiplied by a payroll factor, and the winner is re-decided.

## Two models
- **League average:** run multiplier = (league-average payroll / team payroll) ^ k, with separate penalty and bonus strengths and limits.
- **Salary cap and floor:** only teams outside the band are adjusted. Defaults: MLB's 2026 luxury-tax threshold ($244M) as the cap and the players' union's proposed $150M minimum as the floor.

Standings show by league and division, with adjusted games behind and wins gained or lost. Reference cards show what the current settings do to the top and lowest spenders.

## Validation
Every team's record rebuilt from the game logs matches the official standings for both seasons.

## Files
| File | What it is |
|---|---|
| `index.html` | Web simulator, one self-contained file with all game data |
| `MLB_Payroll_1982_vs_2026.xlsx` | Excel model with live formulas: User Guide, Standings Simulator (inputs and auto-sorted standings), payroll statistics for both eras, and every game |

## Sources
2026 payroll: MLB Labor Relations figures via USA TODAY. 2026 scores: MLB Stats API. 1982 payroll: Doug Pappas, Baseball Prospectus (average salary x 25). 1982 scores: Retrosheet game logs. The information used here was obtained free of charge from and is copyrighted by Retrosheet. Interested parties may contact Retrosheet at www.retrosheet.org.

A thought experiment comparing results to spending, not a talent rating.
