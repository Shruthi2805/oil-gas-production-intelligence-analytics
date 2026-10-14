# GULF HORIZON ENERGY | Oil & Gas Production Intelligence & Operational Performance Analytics

**Flagship UAE-focused synthetic portfolio case study.** This fictional company has no affiliation with ADNOC or other operators. No real-time connectivity, real operating results, or actual environmental measurements are claimed.

## Start here
1. Read `docs/00_Project_Charter.md`, `docs/01_Business_Requirements.md`, and `docs/02_Data_Dictionary_and_Model.md`.
2. Open `data/Gulf_Horizon_Energy_Data.xlsx` or import five CSVs. Production and costs are at date+well grain; events are at event grain.
3. Use `sql/02_SQL_Server_Setup.sql` to create SQL Server tables; load CSVs with Import Flat File / BULK INSERT after adapting file paths. Run `sql/01_production_analysis.sql` and `sql/03_Advanced_Analysis.sql`.
4. Follow `powerbi/Power_BI_Build_Guide.md`; paste measures from `powerbi/DAX_Measures.txt` and `powerbi/Advanced_DAX_Measures.txt`.
5. Match `design/APPROVED_Design_Specification.md` and the included visual reference. Use project heading, NOT the wording on the generated reference.
6. Complete Visio process maps, MicroStrategy dossier, Jira stories, Confluence pages, UAT and evidence before claiming skills or completion.

## What exists / what does not
Included: synthetic source workbook and CSVs; SQL scripts; DAX text; detailed BA docs; diagram blueprints; MicroStrategy build specification; Jira/Confluence import-ready text; UAT and presentation outline; approved visual reference. **Not included:** a functioning PBIX, Visio .vsdx, MicroStrategy dossier, live data, completed Jira tickets, or executed UAT evidence. Those require work in the respective apps.

## Data limitations
The starter has 6 fields, 48 wells and 90 days (2026-01-01 to 2026-03-31) of generated daily production. All production quantities are synthetic BOE, not separate measured oil/gas/water volumes. **Do not display water production, CO2e, revenue, or oil-only barrels as measured KPIs until additional source tables and defensible definitions are added.** `ProductionShortfallBOE` is a per-row nonnegative gap; sum is not equivalent to net target variance. Downtime `EstimatedLostBOE` is an illustrative scenario estimate, not independently measured production loss. `UptimeRatio` is simulated and not derived from downtime hours. Geographic map must use fictional approximate field centroids, never imply real well coordinates.
