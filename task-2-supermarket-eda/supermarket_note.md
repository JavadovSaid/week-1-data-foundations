# Supermarket Sales — Exploratory Data Analysis (EDA)

## Methodology & Data Quality Assessment
- **Dataset Structure:** Verified 1,000 rows and 17 columns containing zero missing values across all features.
- **Data Transformations:** 
  - Converted `Date` to `datetime` format and extracted `Hour` from the `Time` column.
  - Calculated `Gross Margin %` (which evaluates consistently at **4.761905%** across all transactions).

## Groupby Aggregation Findings
- **Branch Performance:** 
  - **Branch C** generated the highest total revenue ($110,568.71 across 328 orders) with an average ticket size of $337.10.
  - **Branch A** ($106,200.37 across 340 orders) and **Branch B** ($106,197.67 across 332 orders) yielded nearly identical total sales.
- **Customer Segmentation:** **Members** generated $164,223.44 (50.1% / 501 orders) versus **Normal** customers at $158,743.31 (49.9% / 499 orders).
- **Product Line Revenue:** 
  - **Top Performer:** `Food and beverages` ($56,144.84 total sales / 174 orders).
  - **Lowest Performer:** `Health and beauty` ($49,193.74 total sales / 152 orders).

## 4 Core Business Insights
1. **Branch C Cross-Selling Advantage:** Branch C outperforms A and B in overall sales ($110.5k) despite having fewer orders (328), driven by a significantly higher mean purchase amount (~$337 vs ~$312 in Branch A).
2. **Evening Rush Peak at 19:00:** Hourly trend analysis reveals a sharp surge in total sales peaking at **19:00 (7 PM)** (~$39.7k), followed by a mid-day secondary spike at **13:00 (1 PM)** (~$34.7k).
3. **Category-Branch Synergy:** The cross-tabulation heatmap shows distinct localized preferences: Branch C dominates `Food and beverages` ($23,767) and `Fashion accessories` ($21,560), while Branch A leads in `Home and lifestyle` ($22,417).
4. **Loyalty Program Parity:** Member and non-member revenue generation is nearly a 50/50 split, indicating that the current membership tier is driving high enrollment but lacks exclusive incentives to boost basket size over guest shoppers.