# NYC Subway Traffic Analysis

> **Metis Data Science Bootcamp project (2021).** This repository is preserved as an early portfolio project and reflects the exploratory analysis practices used at the time.

An exploratory analysis of NYC subway turnstile activity designed to identify stations and weekday time windows where a hypothetical employee-wellness organization could reach commuters with free yoga and meditation sessions.

## Business question

Which subway stations and weekday time periods showed the greatest recorded turnstile traffic from August through November 2021?

## Verified findings

The notebook ranks these as the five busiest station/line combinations in the analyzed period after its cleaning and aggregation steps:

| Rank | Station/lines | Recorded entries + exits |
|---|---|---:|
| 1 | 34 ST–HERALD SQ (BDFMNQRW) | 8,410,930 |
| 2 | GRD CNTRL–42 ST (4567S) | 8,315,535 |
| 3 | 42 ST–PORT AUTH (ACENQRS1237W) | 6,165,122 |
| 4 | 34 ST–PENN STA (ACE) | 5,694,110 |
| 5 | FLUSHING–MAIN (7) | 5,458,666 |

These are totals produced by the original notebook, not current ridership estimates.

## Data

The project uses public [MTA turnstile data](http://web.mta.info/developers/turnstile.html) covering approximately August–November 2021. Turnstile counters are cumulative, so interval traffic must be calculated from differences between observations.

## Approach

1. Combine weekly MTA files and standardize column names.
2. Build turnstile and station identifiers.
3. Remove duplicate recovery-audit records.
4. Calculate interval changes in cumulative entries and exits.
5. inspect negative, zero, and extreme differences caused by counter resets or irregular readings.
6. Aggregate cleaned interval traffic by station, day, weekday/weekend, and hour.
7. Rank candidate stations and time periods for outreach.

## Repository guide

- `EDA MTA Turnstile NY.ipynb` — detailed cleaning and exploratory work
- `MTA EDA Summary.ipynb` — streamlined final analysis
- `MTA slide presentation .pdf` — final presentation
- `Project Writeup.pdf` — written project summary
- Proposal and MVP PDFs — original project framing

## Tools

Python, pandas, NumPy, Matplotlib, and Seaborn.

## What this project demonstrates

- Converting cumulative operational counters into interval metrics
- Investigating duplicates, resets, negative differences, and outliers
- Aggregating high-volume records into decision-oriented rankings
- Connecting exploratory analysis to a practical location and scheduling recommendation

## Limitations

The period reflects pandemic-era travel patterns and should not be treated as representative of current subway traffic. Turnstile data measures station activity, not unique commuters or employment status. The original cleaning replaces or filters irregular counter changes; alternative rules could change the totals. The analysis is a historical learning project rather than a live site-selection model.
