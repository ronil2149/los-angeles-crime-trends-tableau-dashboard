# Data-quality and interpretation notes

These checks were run against the archived **1,005,199-row** CSV snapshot supplied with the project.

## Victim age

- `269,375` records use `Vict Age = 0`.
- There are also a small number of negative / extreme ages.
- Age-based charts should therefore exclude invalid/nonpositive ages.

Among valid ages (1–100), the largest broad age band is **20–34** with **284,192 records**, which supports the original project's finding that young adults are heavily represented.

## Missing demographic fields

- Missing victim sex: **144,781**
- Missing victim descent: **144,793**

## Mapping

- **2,240** records have a zero latitude or longitude value and should not be treated as valid map points.

## Weapon description

- Missing weapon description: **677,917** records.

## Case-status interpretation

The archived data contains several status categories rather than one explicit boolean `Solved` field:

- **Invest Cont:** 803,835
- **Adult Other:** 109,325
- **Adult Arrest:** 86,916
- **Juv Arrest:** 3,249
- **Juv Other:** 1,867
- **UNK:** 7

The original Tableau presentation reported a solved/clearance KPI of roughly 25%. Because the packaged Tableau workbook and its calculated-field formula are no longer available, this repository preserves that figure as an **original dashboard finding** rather than presenting a newly inferred definition of “solved.”
