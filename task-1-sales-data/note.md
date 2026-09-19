
Markdown
# Data Foundations & First Exploration

## Data Overview & Cleaning Steps
* **Dataset Shape:** 2,823 rows and 25 columns.
* **Duplicates:** `0` duplicate rows identified across the dataset.
* **Data Type Corrections:** Converted the `ORDERDATE` column from string (`object`) to `datetime64` format to enable time-series and seasonality analysis.
* **Missing Value Handling:**
  * `ADDRESSLINE2`: 2,521 missing values (~89.3%) filled with `"Unknown"`
  * `STATE`: 1,486 missing values (~52.6%) filled with `"Unknown"`
  * `TERRITORY`: 1,074 missing values (~38.0%) filled with `"Unknown"`
  * `POSTALCODE`: 76 missing values (~2.7%) filled with `"Unknown"`

---

## Key Statistics

### Financial Metrics (`SALES`)
| Metric | Value |
| :--- | :--- |
| **Minimum Sale** | $482.13 |
| **Maximum Sale** | $14,082.80 |
| **Mean Sale** | $3,553.89 |
| **Median Sale** | $3,184.80 |
| **Standard Deviation** | $1,841.87 |

### Order Status Breakdown
* **`Shipped`**: 92.70%
* **`Cancelled`**: 2.13%
* **`Resolved`**: 1.66%
* **`On Hold`**: 1.56%
* **`In Process`**: 1.45%
* **`Disputed`**: 0.50%

### Order Volume Trajectory
| Year | Total Orders | Notes |
| :---: | :---: | :--- |
| **2003** | 1,000 | Baseline performance |
| **2004** | 1,345 | Peak order volume (+34.5% YoY) |
| **2005** | 478 | Incomplete / partial-year data collection |
