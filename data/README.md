# Dataset

This project uses **Crime Data from 2020 to Present**, published by the Los Angeles Police Department through the City of Los Angeles Open Data portal.

**Official source:** https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-Present/2nrs-mtv8/about_data

The archived project snapshot supplied with this repository work contains:

- **1,005,199 records**
- **28 source columns** (the extra parsed date column used during this archival check is not part of the CSV)
- occurrence dates ranging from **2020-01-01** to **2025-04-01**
- LAPD area/division, crime type, date/time, victim demographics, status and geospatial fields

The raw CSV is approximately 255 MB and is intentionally **not committed to GitHub**. Download the current public dataset from the LAPD/Open Data source if you want to reproduce the analysis.

## Important snapshot limitation

The archived CSV is not a complete like-for-like annual series through 2025. Record counts in the supplied snapshot are:

| Year | Records |
|---|---:|
| 2020 | 199,847 |
| 2021 | 209,876 |
| 2022 | 235,258 |
| 2023 | 232,348 |
| 2024 | 127,572 |
| 2025 | 298 |

The sharp reduction in 2024 and the tiny 2025 count should therefore **not** be interpreted automatically as a real collapse in crime. They reflect the supplied extract/reporting snapshot and should be treated carefully in year-over-year analysis.
