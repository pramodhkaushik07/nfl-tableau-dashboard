# NFL Performance Dashboard (Tableau)

An interactive Tableau dashboard built to evaluate NFL team performance through scoring outcomes, offensive production, and efficiency-based KPIs. The dashboard supports rapid comparison across teams and seasons, enabling identification of outliers, performance gaps, and longitudinal performance trends.


<img width="1512" height="912" alt="NFL_Dashboard" src="https://github.com/user-attachments/assets/fe5c5214-4c42-4202-b14c-f7b27bac0f32" />


---

## Objective
Create a single, decision-oriented view that allows users to:
- Assess the relationship between offensive production (yards) and results (points)
- Understand how team performance evolves across seasons and conferences
- Compare teams dynamically under different performance definitions rather than relying on a single metric

The dashboard is designed for exploratory, insight-driven analysis rather than static reporting.

---
## Key Questions This Dashboard Answers

- How closely aligned are offensive production (yards) and scoring outcomes (points) across teams?
- Which teams outperform or underperform relative to their yardage, indicating potential efficiency gaps?
- How does team scoring performance evolve over time, and are trends consistent across conferences?
- Which teams demonstrate sustained performance versus volatility across seasons?
- How do team rankings change when performance is evaluated using different KPIs rather than a single metric?

---
## Key Insights (Illustrative)

The dashboard is designed to surface insights such as:

- Teams with comparable offensive yardage can exhibit materially different scoring outcomes, highlighting differences in efficiency rather than volume.
- Outlier teams appear in the Pts vs Yards view, prompting investigation into red-zone performance, turnovers, or situational execution.
- Scoring consistency over time varies significantly by team and conference, with some teams showing sustained performance while others demonstrate high volatility.
- Team rankings shift meaningfully depending on the selected KPI, reinforcing the risk of evaluating performance through a single metric lens.
 
---
## Dashboard Structure

### Pts vs Yards Scatterplot
Maps total points scored against total yards gained by team.  
This view functions as the primary interaction anchor—selecting a team filters all other views, enabling focused deep dives without additional navigation.

### Points Over Time (Area Chart)
Displays scoring trends across seasons, segmented by conference.  
Forecasting is applied to emphasize directional patterns and sustained performance behavior rather than short-term noise.

### KPI Ranking (Parameter-Driven Bar Chart)
Dynamically ranks teams based on a user-selected KPI.  
This approach avoids redundant views and highlights how perceived performance changes when evaluation criteria shift.

---

## Interaction & Design Rationale
- Team-level selection propagates across all views to maintain analytical context
- Global conference and season filters ensure consistent comparisons
- KPI parameter enables flexible performance evaluation without increasing dashboard complexity
- Team logos are implemented as custom Tableau shapes to improve recognition while preserving visual clarity

The design prioritizes speed of insight, interpretability, and low cognitive overhead.

---

## Repository Contents
- `tableau/NFL_Dashboard.twbx` — Packaged Tableau workbook containing all data sources, calculations, and visualizations
- `nfl_team_logos/` — Custom shape assets used to render team logos within Tableau

---

## Usage
1. Download the packaged Tableau workbook (`.twbx`)
2. Open in Tableau Desktop
3. Use interactive controls to explore team performance across metrics, seasons, and conferences

---

## Tools
- Tableau Desktop
