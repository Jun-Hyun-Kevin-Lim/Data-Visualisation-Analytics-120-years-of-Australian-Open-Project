# Australian Open (120 Years) — Advanced Data Visualisation (Tableau)

## Overview
This project analyzes **120 years of Australian Open match records** to identify long-run trends, dominance patterns, and outliers across men’s and women’s champions. Using Tableau, I applied multiple advanced visualisation techniques (treemap, parallel coordinates, geographic map, scatter) with explicit **null-handling** and **normalization** to ensure transparent comparisons.

## Key Ideas
- **Dominance + diversity:** Nationality patterns and top-player dominance over time
- **Performance multi-metric view:** Games won/lost, win ratios, set-level win ratios
- **Transparency in data gaps:** Null values treated explicitly (e.g., unseeded champions, non-existent later sets)

## Dataset (Key Fields)
- Year, Gender, Champion, Champion Nationality
- Champion Seed, Runner-up Seed
- Score, Match Duration (mins)
- Games Won/Lost, Win Ratio, Set Win Ratios

## Visualisation Techniques
1) **Treemap**
- Hierarchical view of champions by **nationality → player**, with seed encoding
- Null seed handled as **“Unseeded”** (calculated field)

2) **Parallel Coordinates**
- Multi-metric comparison across normalized win/set ratios
- Later-set ratios nulls treated as match-ended indicators (set to 0 via calculated fields)

3) **Geographic Map**
- Champions’ nationality distribution with bubbles sized by games won
- Historical edge case: **Yugoslavia** manually corrected to **Serbia** for mapping

4) **Scatter Chart**
- Relationship between **games won vs games lost**, segmented by gender + seed
- Highlights outliers and the general link between seeding and success

## Key Findings (Highlights)
- Consistent dominance appears clearly for top champions (e.g., **Novak Djokovic**, **Margaret Court**, **Serena Williams**)
- Seeding generally correlates with higher success, but notable **low-seed/unseeded outliers** exist (e.g., Andre Agassi, Monica Seles)
- Geographic view reinforces long-run regional dominance patterns (Australia/Europe concentration)

## Files
- `docs/au-open-120y-visual-analytics-report.pdf` — full report (dataset, methods, charts, insights)

## Repo Structure
- `docs/` report PDF

## Notes
This repo is documentation-first (report + visuals). If needed, I can add dashboard screenshots/GIFs under `assets/` for faster recruiter review.
