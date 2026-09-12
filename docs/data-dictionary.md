# Data dictionary — fields used in the dashboard

| Field | Meaning / use |
|---|---|
| `DATE OCC` | Date when the incident occurred; used for year/month trends |
| `TIME OCC` | Incident time stored in HHMM-style numeric form; used for time-of-day analysis |
| `Crm Cd Desc` | Crime description/category |
| `AREA NAME` | LAPD geographic area/division |
| `Vict Age` | Victim age; requires cleaning because many records use `0` |
| `Vict Sex` | Victim sex code |
| `Vict Descent` | Victim descent code |
| `Weapon Desc` | Weapon description where available |
| `Status` / `Status Desc` | Case status used for status/clearance analysis |
| `LAT` / `LON` | Coordinates used for the Tableau crime map/heatmap |

The source file contains additional administrative and coding fields. The dashboard emphasizes the fields above because they directly support the project's spatial, temporal, demographic and case-status questions.
