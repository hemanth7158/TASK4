# NYC Property Sales Dashboard - Power BI (Task 4)

##  Objective
Create an interactive dashboard using Power BI to analyze NYC real estate transactions and enable business stakeholders to:
- Monitor sales trends
- Understand neighborhood-level activity
- Evaluate performance by borough/building type

---

##  Dataset
**Source**: [Kaggle - NYC Rolling Sales](https://www.kaggle.com/datasets/new-york-city/nyc-property-sales)  
**File**: `nyc-rolling-sales.csv`

### Key Columns Used:
- `BOROUGH`, `NEIGHBORHOOD`, `ZIP CODE`
- `BUILDING CLASS CATEGORY`
- `SALE PRICE`, `SALE DATE`
- `GROSS SQUARE FEET`, `YEAR BUILT`

---

##  Tools Used
- **Power BI Desktop**
- Power Query (for data cleaning and transformation)
- DAX (for KPI calculations and time-series measures)

---

## Data Cleaning Steps
1. Converted `SALE DATE` to proper Date format.
2. Removed transactions with `SALE PRICE = 0` (invalid or placeholder entries).
3. Extracted `YEAR` and `MONTH` from `SALE DATE` for trend analysis.
4. Calculated `Price per Sq. Ft = SALE PRICE / GROSS SQUARE FEET`.
5. Filtered extreme outliers for more realistic insights.

---

##  Dashboard Features

| Section           | Visual Type         | Description |
|------------------|---------------------|-------------|
| **KPI Summary**  | Card Visuals        | - Total Sales<br>- Average Sale Price<br>- Transaction Count |
| **Sales Trend**  | Line Chart          | Monthly/Yearly trend of total sales |
| **Borough Breakdown** | Bar Chart     | Total or average sale price per borough |
| **Building Class Analysis** | Donut Chart | Share of transactions by building category |
| **Detailed View** | Table               | Drill-down by ZIP Code and Neighborhood |
| **Filters**      | Slicers             | Interact by Borough, Year, and Building Class |

---

##  Dashboard Layout

```
+------------------------------+
| KPI CARDS (Top Summary)     |
+------------------------------+
| Line Chart      | Bar Chart |
| (Sales Trend)   | (Borough) |
+------------------------------+
| Pie Chart | Filters | Table |
+------------------------------+
```

---

##  Key Insights
- Boroughs with highest average sale prices
- Sales spikes in specific months/years
- Building class categories contributing most to sales
- Neighborhoods with growing or declining activity

---
