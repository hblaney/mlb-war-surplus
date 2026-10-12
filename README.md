# 2026 WAR vs what teams paid

I built a 2026 position-player WAR from Statcast batting and OAA, priced a win off free agents, then compared that to what guys actually made.

The memo is [here](https://hblaney.github.io/mlb-war-surplus/report.html).

xBA fielding had Brandon Lowe at 8 WAR with +32 glove runs. That was the model, not him. With OAA, Crow-Armstrong is 10.1 WAR (26 OAA) and Lowe is 5.9 (15 OAA).

FAs: about $6.45M per WAR. Corr 0.41, R² 0.17. One year of WAR does not track one year of FA pay. Pre-arb surplus is about +$9M, arb +$6.8M, FA −$3.9M. Value WAR is WAR minus salary / 6.45.

## Run

This folder. `tidyverse`, `sabRmetrics`, `readr`.

Outputs are already in `data/`. To rebuild WAR, delete `data/player_war_2026.csv` and run `analysis.qmd`. The pitch `.rds` stays local.
