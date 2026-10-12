# 2026 WAR vs what teams paid

Custom 2026 position-player WAR (Statcast batting + OAA), then a free-agent price per win, then surplus / value WAR.

The memo is **[report.html](report.html)**. If GitHub Pages is on, that link is a normal webpage. Knit `report.Rmd` if you need to rebuild it.

- xBA fielding made Brandon Lowe 8 WAR on +32 glove runs. OAA fixes that: Crow-Armstrong 10.1 WAR (26 OAA), Lowe 5.9 WAR (15 OAA).
- FA price is about **$6.45M per WAR**. Correlation 0.41, R² 0.17. 2026 WAR does not explain 2026 FA pay.
- Pre-arb surplus about +$9.0M, arb +$6.8M, FA −$3.9M. Value WAR = WAR − salary / 6.45.

## Run

Working directory = this folder. Packages: `tidyverse`, `sabRmetrics`, `readr`.

`data/` already has OAA, salaries, and WAR outputs. Knit `report.Rmd` to rebuild the memo. `quarto render analysis.qmd` rebuilds WAR if you delete `data/player_war_2026.csv` first. Do not upload `statcast_2026.rds`.
