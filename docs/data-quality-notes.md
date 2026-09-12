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

The earlier course presentation summarized the clearance rate as roughly 25%, but the surviving final Tableau Public dashboard reports a **clearance rate of 8.97%**, based on **90,171 solved** and **915,028 unsolved** incidents. Because the packaged .twbx workbook and its calculated-field formula are no longer available, this repository preserves the value displayed by the final live dashboard..
