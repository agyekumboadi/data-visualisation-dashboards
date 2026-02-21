# Tableau Dashboards

This folder contains Tableau dashboard exports (images) and is designed to demonstrate:
- KPI storytelling (what happened + what changed)
- segmentation (group comparison)
- trend analysis over time
- relationship analysis (how two measures move together)
- interactive filtering (for slicing the view)

> If you also have the packaged workbook file (`.twbx`), store it in `assets/docs/` for reproducibility.

---

## Dashboard: King Crab Population (2018–2019)

**File**
- `Tableau_KingCrab_Population_In_Alaska_DataStorytelling.png`

**Purpose**
This dashboard is structured as a compact data story for a two-year snapshot (2018–2019). It highlights:
1. **Relationship patterns** (how two measures change together)
2. **Group differences** (comparing populations by group)
3. **Year-over-year trend** (whether key measures increased or decreased)

---

## What the dashboard contains (by section)

### A) Relationship between Height and Whole Weight (Scatter + trend)
**What it shows**
- Each point represents the **average** observation at a given height level.
- The trend line shows the overall direction and strength of the relationship.

**How to interpret**
- The upward curve suggests **WholeWeight rises as Height increases**.
- A curved pattern typically indicates **non-linear growth** (weight increasing faster after a certain height).

**Why this is useful**
- Helps communicate growth patterns: whether weight scales gradually or accelerates at larger sizes.
- Useful for biological growth insight and size/weight modelling.

---

### B) 2018 Total Number of Spots (Bar chart)
**What it shows**
- A 2018 count comparison of total observations by group.

**How to interpret**
- Quickly identifies which group(s) dominate the sample in 2018.
- Helps validate if some groups might be under-represented.

**Why this matters**
- If one group has far more data, it can influence averages and trends.
- It also supports decisions on whether weighting or balancing is needed.

---

### C) Average Weights by Group (Stacked bars)
**What it shows**
- Group-level weight comparison, split visually (stacked) to highlight composition and contrast.

**How to interpret**
- Taller bars indicate higher group averages.
- Differences between groups can suggest biological or behavioural factors that warrant deeper analysis.

**Why this matters**
- Group comparisons are a core KPI analysis technique—useful for policy decisions, catch limits, and sustainability assessments.

---

### D) Average WholeWeight Trend (2018–2019) (Line chart)
**What it shows**
- A year-to-year movement of average WholeWeight by group.

**How to interpret**
- Flat lines indicate stability.
- Upward/downward movement indicates improvement or decline in average WholeWeight.

**Why this matters**
- Trend movement is a quick “health indicator” for the population proxy measures.
- Even small shifts can be meaningful if consistent across groups.

---

## Filters / Interactivity
The design uses filtering to allow targeted comparison:

### Filter: Sex
- Used to isolate group differences and avoid mixing distributions.
- Helps answer: “Does the pattern hold across each category?”

### Filter: Year of Year (2018–2019)
- Allows controlled comparison between 2018 and 2019.
- Helps answer: “Did the same relationships or averages persist year-over-year?”

---

## Design & Visual Choices (why it works)
- Dark theme improves contrast, especially for analytical storytelling.
- Charts are arranged in a logical flow:
  1) relationship → 2) group comparison → 3) trend
- Combination of scatter + bars + line supports both:
  - exploratory analysis (scatter)
  - executive summary (bars/lines)

---

## Suggested Enhancements (optional)
If you iterate on this dashboard later:
- Add a short “Insights” text block summarising 3 key takeaways.
- Add tooltips with:
  - group name
  - exact average values
  - year label
- Consider confidence intervals or distribution plots if raw-level detail is available.

---

## Files in this folder
- `Tableau_KingCrab_Population_In_Alaska_DataStorytelling.png`
