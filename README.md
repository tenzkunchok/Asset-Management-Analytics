# Enterprise Asset Management (EAM) Analytics

This project analyzes maintenance performance data for an Enterprise Asset Management (EAM) system using SQL and Tableau.

## Objectives
- Assess asset backlog exposure and maintenance risk
- Identify downtime and failure patterns across locations and asset types
- Support maintenance prioritization and operational decision-making

## Data

The project uses structured operational datasets representing a simplified EAM environment:

Assets – asset type, criticality, condition, and replacement cost
Work Orders – status, priority, timing, and cost information
Failures & Defects – reliability and downtime indicators
Locations – facility and borough-level context

All datasets were cleaned and prepared in MySQL before analysis.
All raw datasets are stored in the `data/` folder.


## Tools
- SQL (MySQL) for data preparation and analysis
- Tableau for interactive dashboards and KPIs

## SQL
- `SQL/views.sql` – creates analysis-ready views used for dashboards
- `SQL/analysis_queries.sql` – analytical queries for risk, backlog, and cost analysis

## Results

- A small subset of assets accounts for a disproportionate share of downtime and failures
- Maintenance backlog is concentrated in specific priority levels and locations
- Certain asset types show persistent reliability and cost challenges
- Downtime impact varies significantly by borough
- Work order delays are primarily driven by pre-completion bottlenecks

## Recommendations

- Prioritize preventive maintenance for high-downtime assets
- Address backlog at hotspot locations through targeted resource allocation
- Improve throughput for medium-priority maintenance tasks
- Review maintenance strategies for high-failure asset types
- Use regional downtime insights to guide staffing and planning
- Streamline work order workflows to reduce cycle time
