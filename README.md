# Limpopo-Poultry-Hatchery-Production-Analysis-Using-Excel

# Limpopo Poultry Hatchery — Production Data

Weekly hatchery production data for 6 poultry flocks/farms across Limpopo province (Waterberg, Capricorn, and Mopani districts), covering **7 January – 27 May 2022**. Includes raw data, a documented cleaning process, pivot summaries, a dashboard, and analysis with recommendations.

## Repository / Workbook Structure

```
Limpopo_Poultry_Hatchery.xlsx
├── Limpopo poultry hatchery messy    # Raw data (127 records, 23 cols)
├── Data_Quality_Report              # Log of cleaning issues & fixes
├── Limpopo poultry hatchery clean   # Cleaned data (118 records, 29 cols)
├── Data dictionary #definations
├── Pivot Tables    # Hatchability % / Fertility % by farm & quarter
├── Dashboard    # Visual production summary
└── Analysis # KPIs, farm summary, key insights
```

## Farms Covered

| Flock ID | Farm | Type | District |
|---|---|---|---|
| FL-001 | Lephalale Poultry Farm | Broiler | Waterberg |
| FL-002 | Bela-Bela Agri | Broiler | Waterberg |
| FL-003 | Mokopane Layers | Layer | Waterberg |
| FL-004 | Polokwane Hatchery Hub | Broiler | Capricorn |
| FL-005 | Tzaneen Breeder Farm | Breeder | Mopani |
| FL-006 | Giyani Poultry | Broiler | Mopani |

## Contents

- **Raw data** — as originally logged, unedited.
- **Cleaned data** — deduplicated, standardised, outliers handled, QC-flagged. See `Data_Quality_Report` tab for the full list of fixes applied.
- **Pivots & Dashboard** — summary views for quick reporting.
- **Analysis** — KPI rollups and written recommendations per farm.

## Key Findings & Recommendations

From the `Analysis` tab:

1. **Best performer** — Tzaneen Breeder Farm, highest avg hatchability (91.86%).
2. **Watch list** — Mokopane Layers, lowest avg hatchability (90.50%); investigate incubation temperature variance and egg handling procedures.
3. **Biosecurity** — 3 check failures recorded; Bela-Bela Agri (Feb 4) and Giyani Poultry (Apr 15) were repeat concerns — enforce staff entry protocols.
4. **Production gaps** — Easter shutdown (Apr 1) caused 100% production loss across all 6 farms; plan ahead to minimise restart delays.
5. **Data quality** — 30 weekly records fell below the 91% hatchability threshold; cross-check against environmental log data for temperature/humidity correlations.
6. **Feed efficiency** — Waterberg district farms consumed more feed per hatched chick; recommend a feed conversion ratio analysis in the next phase.
7. **Highest cull rate** — Giyani Poultry (0.67%), also the lowest fertility % among broilers — worth investigating for a shared root cause.
8. **Best mortality profile** — Tzaneen Breeder Farm (0.40% cull rate, 86 mortalities on 240,000 set), consistent with its top fertility and hatch rates.

## Documentation

- [`Limpopo Poultry Hatchery.xlsx`]-- Includes raw data, a documented cleaning process, pivot summaries, a dashboard, and analysis with recommendations.
- [`Limpopo Poultry Hatchery Analysis Report.pdf`]—summary report on the analysis.

## Notes

- All hatchability, cull rate, and QC flag fields are live formulas, not hardcoded values — recalculating the workbook updates them.
- The clean sheet excludes the Easter shutdown week (2022-04-01, zero production across all farms); it remains in the raw sheet.
