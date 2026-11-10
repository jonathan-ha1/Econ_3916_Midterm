# Does the NBA Pay for Production and Efficiency?

## About this project
NBA teams spend millions of dollars on players every season, but it isn't always clear whether that money goes to the players who actually perform best. This project looks at whether a player's efficiency last season is connected to how much they get paid this season, after taking age and position into account, and how much of a player's pay is shaped by other factors like contract timing and league salary rules.

## Question
Among NBA players in the 2026-27 season, how is a player's efficiency last season (2025-26 Box Plus/Minus, BPM) related to their 2026-27 salary, taking into account their age and position?

## Data
Both files come from Basketball-Reference
- Salaries: https://www.basketball-reference.com/contracts/players.html (2026-27 salary column)
- Stats: https://www.basketball-reference.com/leagues/NBA_2026_advanced.html (2025-26 advanced stats)

The cleaned files used in the notebook are in the `data/` folder: `NBA_salaries.csv` and `NBA_Stats.csv`.

## How to run the notebook
1. Open the notebook in Google Colab: https://colab.research.google.com/drive/1WgTnEe_VhA7fbsRdGCxyFwMG8wZVwSqX?usp=sharing 
2. Click the folder icon on the left and upload `NBA_salaries.csv` and `NBA_Stats.csv` from the `data/` folder.
3. Click Runtime → Run all.
4. The last cell, “Numbers my report quotes,” prints every number used in the report, including 455 players in the salary file and a final sample of 345.

## Findings
Players who played better last season do get paid more, since a player with one more point of BPM makes about 17.0% more salary this season than a player of the same age and position. Age matters too, with pay going up early in a player’s career and peaking around age 31 before going down, which makes sense since young players are stuck on rookie deals and older players usually take smaller contracts. When minutes played is added in, the effect drops to 12.5%, which means part of the reason better players get paid more is that they also play more. Still, a lot of contracts were signed before last season even started, so this shows that performance and pay are connected, not that playing better directly causes a bigger salary.

## Files
- `midterm_starter_(1).ipynb`: the analysis notebook
- `NBA Players Salary and Efficiency.pdf`: the written report
- `data/NBA_salaries.csv` and `data/NBA_Stats.csv`: the cleaned data files
