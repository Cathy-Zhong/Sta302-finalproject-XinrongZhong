# STA302 hotel ADR project

This repository contains the reproducible R Markdown analysis for the modelling and diagnostics portion of the STA302 Part 1 proposal.

## Research question

Among non-cancelled bookings with a positive ADR at the Lisbon city-hotel property and the Algarve resort-hotel property, how is booking lead time associated with average daily rate (ADR), and does that association differ between the two properties after adjustment for arrival timing, length of stay, party composition, meal plan, reserved room type, market segment, and customer type?

The `hotel` variable distinguishes two specific properties, not representative samples of all city and resort hotels. Accordingly, conclusions are limited to bookings in these data.

## Novelty relative to the source article

Antonio, de Almeida, and Nunes (2019) introduced the datasets and discussed their use for cancellation-prediction research. This project instead uses an explanatory multiple linear regression with continuous ADR as the response and a `lead_time × hotel` interaction. It does not reproduce the source article's cancellation-classification task.

## Files

- `STA302_Part1_analysis.Rmd`: imports the original data, reproduces the cleaning pipeline, removes 31 zero-recorded-guest records, fits the preliminary model on 72,973 observations, reports estimates and 95% confidence intervals, and performs residual diagnostics.
- `data/hotels_clean_no_zero_guests.csv`: the 72,973-row, 24-variable analysis dataset after the zero-recorded-guest exclusion.
- `data/README.md`: explains where to place the original CSV.
- `.gitignore`: prevents large or generated files from being committed accidentally.

## Reproduce the analysis

1. Put the original `hotels.csv` in `data/hotels.csv`.
2. Open `STA302_Part1_analysis.Rmd` in RStudio.
3. Knit the file from the repository root.

The Rmd uses base R and `knitr`. It explicitly removes the 31 zero-recorded-guest bookings under the updated group decision. It does not silently delete exact duplicate-looking records or low ADR observations. If the Data Lead changes another cleaning decision, update the cleaning code, the row-count table, the committed analysis CSV, and all reported model results together.

## Source

Antonio, N., de Almeida, A., & Nunes, L. (2019). Hotel booking demand datasets. *Data in Brief, 22*, 41–49. https://doi.org/10.1016/j.dib.2018.11.126

