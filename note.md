# Data Foundations & First Exploration

## Data Overview & Cleaning Steps
- **Dataset Shape:** 2,823 rows and 25 columns.
- **Duplicates:** 0 duplicate rows were identified in the dataset.
- **Data Type Corrections:** Converted the `ORDERDATE` column from an `object` string type to `datetime64` format to enable time-series analysis.
- **Missing Value Handling:**
  - `ADDRESSLINE2` (~71% missing) filled with `"Unknown"`
  - `STATE` (~29% missing) filled with `"Unknown"`
  - `POSTALCODE` (~15% missing) filled with `"Unknown"`
  - `TERRITORY` filled with `"Unknown"`

## Key Statistics
- **SALES Metrics:**
  - Minimum Sale: $482.13
  - Maximum Sale: $14,082.80
  - Mean Sale: $3,553.89
  - Median Sale: $3,184.80
- **Order Status Breakdown:** 
  - `Shipped`: 92.7%
  - `Cancelled`: 2.1%
  - `Resolved`: 1.7%
  - `On Hold`: 1.6%
  - `In Process`: 1.5%
  - `Disputed`: 0.5%

## Initial Business Insights
1. **Yearly Order Trajectory:** Order volume grew by 34.5% from 2003 (1,000 orders) to 2004 (1,345 orders). The sharp drop in 2005 (~478 orders) reflects partial-year data collection rather than a business decline.
2. **Right-Skewed Sales Distribution:** Average order value ($3,553.89) is higher than the median ($3,184.80), with a long right tail showing individual orders peaking up to $14,082.80.
3. **High Fulfillment Reliability:** Over 92.7% of total orders reach `Shipped` status successfully, while lost revenue from `Cancelled` (2.1%) or `Disputed` (0.5%) orders remains minimal.
4. **Product Line Category Volume:** Product offerings span across distinct categories (including Classic Cars, Vintage Cars, Motorcycles, and Ships) that drive consistent order volume across global markets.