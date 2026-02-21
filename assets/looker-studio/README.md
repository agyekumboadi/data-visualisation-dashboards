# Looker Studio Dashboards

This folder contains exported Looker Studio dashboard visuals. The focus here is on:
- executive KPI cards (quick performance view)
- breakdown by category (models, sentiment, systems affected)
- time series monitoring (month-to-month changes)
- compact dashboard layout (sales + service)

These exports are designed for fast review and portfolio demonstration.

---

## Dashboard: Sales

**File**
- `looker-studio_sales_dashboard.jpeg`

**What it is**
A KPI-first dashboard summarising overall performance and key breakdowns.

**Key elements typically shown**
- High-level KPI totals (e.g., profit, quantity sold, average quantity sold)
- Breakdown chart(s) for performance by model
- Dealer-level comparison showing profit contribution

**Why it’s useful**
- It answers “How are we doing?” within seconds.
- It supports decision-making by identifying:
  - best performing product/model
  - best performing dealer ID (profit contributors)
  - whether performance is concentrated or diversified

**How to read it effectively**
1. Start with KPIs: confirm totals and averages.
2. Check “Quantity Sold by Model” to see demand leaders.
3. Compare “Profit by Dealer ID” to identify top value channels.

---

## Dashboard: Service

**File**
- `looker-studio_service_dashboard.jpeg`

**What it is**
A service-focused dashboard that highlights operational or support themes alongside sentiment insight.

**Key elements typically shown**
- Units by Model (volume indicator)
- Customer by Sentiment (positive/neutral/negative distribution)
- Quantity Sold and Profit by Month (trend monitoring)
- Model by Systems Affected (cross-tab / heatmap style analysis)

**Why it’s useful**
- Combines operational indicators and customer sentiment.
- Helps answer:
  - Which models generate the most activity?
  - Is customer feedback trending positive or negative?
  - What systems are most frequently involved?

**How to interpret the sentiment block**
- If Positive dominates: service experience is generally strong.
- If Neutral is large: opportunities exist to improve experience and move neutral to positive.
- If Negative grows: investigate root causes (system affected, model, location, time period).

---

## Dashboard: Quantity Sold vs Revenue

**File**
- `looker-studio_qty-sold_by_revenue.jpeg`

**What it is**
A performance comparison visual that lets viewers understand if:
- high volume aligns with high revenue, or
- revenue is driven by fewer high-value items.

**How to use it**
- Identify whether growth is:
  - volume-led (units drive revenue), or
  - value-led (pricing / premium segments drive revenue)

**What to look for**
- Large gaps between quantity and revenue patterns indicate pricing differences or mix changes.
- A stable relationship suggests consistent pricing and sales mix.

---

## Notes on Reproducibility
This repository stores exports. If you later want reproducibility, add:
- a short build note (data source fields used)
- a link to the Looker Studio report (optional)
- the calculated fields used (if any) inside `assets/docs/`

---

## Files in this folder
- `looker-studio_sales_dashboard.jpeg`
- `looker-studio_service_dashboard.jpeg`
- `looker-studio_qty-sold_by_revenue.jpeg`
