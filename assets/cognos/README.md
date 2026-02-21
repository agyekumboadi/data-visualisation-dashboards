# IBM Cognos Analytics Dashboards

This folder contains exported IBM Cognos dashboard visuals built to demonstrate:
- KPI summary design (headline metrics)
- breakdown analysis (model, dealer, system affected)
- dashboard composition (multiple views on one canvas)
- heatmap/crosstab interpretation for operational insights

---

## Dashboard: Product Sales

**File**
- `cognos_product-sales_dashboard.jpeg`

**What it shows**
A product performance dashboard that typically includes:
- KPI tiles (Quantity Sold, Revenue)
- A multi-line trend chart: Product Line Performance by Year

**How to interpret**
- KPI tiles provide “current state” totals.
- The line chart shows:
  - which product line is increasing or declining over time
  - changes in ranking between product lines across years

**Why it’s valuable**
- Supports product strategy decisions (invest, maintain, or discontinue)
- Helps detect shifting demand patterns

---

## Dashboard: Automotive Sales — Quantity Sold & Profit

**File**
- `Cognos_AutomotiveSales_Dashboard_QuatitySold_&_Profit.jpeg`

**What it shows**
A sales dashboard combining:
- sales volume and profitability signals
- model comparisons
- high-level KPI summary

**Common dashboard logic**
- “Quantity Sold” indicates demand strength.
- “Profit” indicates value generation.
- A model can be high-volume but low-profit (or the opposite).

**How to read it**
1. Check KPIs first (overall baseline).
2. Use model breakdown to identify best sellers.
3. Compare with profit view to confirm whether best sellers also drive profit.

---

## Dashboard: Automotive Sales — Dealer ID

**File**
- `Cognos_AutomotiveSales_Dashboard_DealerID.jpeg`

**What it shows**
Dealer-level contribution analysis, usually used for:
- ranking dealers by profit
- understanding distribution of performance across channels

**How to interpret**
- Top dealer(s) represent the largest value contribution.
- If a small number of dealers dominate:
  - performance is concentrated
  - risk is higher if one dealer underperforms

**Suggested follow-up analysis**
- Compare dealer performance over time
- Segment by model or region (if available)

---

## Dashboard: Automotive Service

**File**
- `Cognos_AutomotiveService_Dashboard.jpeg`

**What it shows**
A service dashboard combining:
- recall counts by model
- monthly pattern in quantity/profit
- customer sentiment distribution
- affected system cross-analysis (heatmap style)

**How to interpret the “Affected System” view**
- Darker / stronger values indicate higher recall volume for that model-system combination.
- Useful for:
  - spotting repeated issues (e.g., recurring system impact)
  - prioritising investigation and QA focus

**Why it’s valuable**
- Supports operational risk management and quality assurance
- Links service issues to customer feedback and model performance

---

## Files in this folder
- `cognos_product-sales_dashboard.jpeg`
- `Cognos_AutomotiveSales_Dashboard_QuatitySold_&_Profit.jpeg`
- `Cognos_AutomotiveSales_Dashboard_DealerID.jpeg`
- `Cognos_AutomotiveService_Dashboard.jpeg`
