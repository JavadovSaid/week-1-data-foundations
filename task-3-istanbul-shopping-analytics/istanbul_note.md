# Multi-Dimensional Retail Analytics on Istanbul Shopping Data

## Methodology & Data Quality Assessment
- **Dataset Overview:** Processed 99,457 transaction records across 10 shopping malls in Istanbul with 0 missing values across all 10 feature columns.
- **Data Engineering & Feature Extraction:**
  - Converted `invoice_date` from string (`object`) to standard `datetime64` format (`%d/%m/%Y`).
  - Extracted temporal features (`year` and `month`) to analyze yearly revenue trajectories.
  - Engineered `total_revenue` per line item (`quantity` × `price`).

## Groupby & Cross-Tabulation Summary
- **Category Economics & Revenue Ranking:**
  - **Top Revenue Categories:** `Clothing` dominates total gross revenue at **$31.08M** (34,487 transactions), followed by `Shoes` (**$18.14M**) and `Technology` (**$15.77M**).
  - **Average Purchase Value:** `Technology` yields the highest average purchase value per transaction (**$3,156.94**), whereas `Food & Beverage` holds the lowest (**$15.67**).
- **Mall Performance Hierarchy:**
  - `Mall of Istanbul` ($6.25M in Clothing) and `Kanyon` ($6.16M in Clothing) emerge as the leading revenue hubs, followed closely by `Metrocity` ($4.72M in Clothing).
  - Smaller footprint centers like `Cevahir AVM`, `Emaar Square`, and `Forum Istanbul` maintain consistent lower-tier spending volumes (~$1.5M–$1.57M in Clothing).
- **Yearly Trend (2021–2023):**
  - Revenue generation remained stable through 2021 and 2022 across major categories, followed by a sharp dropoff in recorded 2023 values due to partial-year data collection.

## 5 Actionable Business Insights for AVM Management
1. **Mall Anchoring & Tenant Mix Strategy:** `Mall of Istanbul` and `Kanyon` drive significantly higher sales than all other locations. Management should allocate primary anchor spaces to high-ticket categories (`Clothing`, `Shoes`, `Technology`) to maintain foot-traffic conversion.
2. **Category-Specific Ticket Sizing:** While `Clothing` generates the highest overall volume (34.5k orders), `Technology` commands an average basket size of **$3,156.94**—more than 200 times higher than `Food & Beverage` ($15.67). Premium electronics retailers should be incentivized with flexible lease structures.
3. **Targeted Female Demographic Campaigns:** Female shoppers generate substantially higher aggregate spending across every category—most notably in `Clothing` ($18.7M vs $12.4M for males), `Shoes`, and `Technology`. Marketing budgets should prioritize female-oriented promotional programs and loyalty perks.
4. **Suburban Outlet Differentiation:** Malls such as `Viaport Outlet` and `Zorlu Center` show near-identical revenue profiles across categories ($1.53M vs $1.57M in Clothing). Management can differentiate these venues by curating exclusive luxury or outlet-only product lines.
5. **Seasonal & Yearly Revenue Planning:** Revenue peaked in 2021–2022 across `Clothing`, `Shoes`, and `Technology`. AVM management must align major promotional expos during Q3–Q4 peak operational windows to stabilize year-over-year revenue growth.