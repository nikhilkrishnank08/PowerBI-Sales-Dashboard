# 📊 Sales Performance Dashboard

## Business Question
How is our retail business performing across regions, categories, and time periods? Where are the opportunities to grow revenue and improve profitability?

## Dashboard Preview
![Sales Performance Dashboard]
![My Image](images/dashboard_screenshot.png)

## Dataset
- **Source:** [Kaggle - Sample Superstore](https://www.kaggle.com/datasets/naveenkumar20bps1137/sample-superstore)
- **Records:** 9,994 orders
- **Time Period:** 2014–2017
- **Fields:** Sales, Profit, Quantity, Discount, Region, Category, Customer Segment, Ship Mode

## Tools Used
- **Power BI Desktop** - Dashboard design, DAX measures, interactive visuals
- **Power Query** - Data cleaning, date format standardisation, column transformations
- **DAX** - Calculated measures (Revenue, Profit, AOV, Profit Margin %, YoY Growth)
- **GitHub** - Version control and portfolio hosting

## Data Cleaning Steps
The raw dataset had inconsistent date formats - some dates used dashes (`11-08-2016`) and others used slashes (`6/16/2016`). This was resolved in Power Query by:
1. Replacing all dashes with slashes using `Table.ReplaceValue()`
2. Converting to Date type with US locale (`en-US`)
3. Extracting Year and Month Name columns for easier filtering and grouping

## Key Features
- **5 KPI Cards** - Total Revenue ($2M), Total Profit ($286K), Total Orders (10K), Average Order Value ($229.86), Profit Margin (12.5%)
- **Monthly Revenue Trend** - Line chart showing seasonality and peaks across the year
- **Regional Performance** - Clustered Bar chart comparing revenue across West, East, Central, and South regions
- **Top Products by Revenue** - Clustered bar chart highlighting the highest-grossing products
- **Profit by Category** — Donut chart showing profit distribution across Technology, Office Supplies, and Furniture
- **Interactive Slicers** — Filter the entire dashboard by Year (2014–2017), Region, and Category

## Key Insights

### 1. Technology Drives Revenue but Furniture Destroys Profit
Technology and Office Supplies together generate over 93% of total profit ($145.45K + $122.49K), while Furniture contributes only 6.4% ($18.45K) despite having significant sales volume. This suggests Furniture has high costs or heavy discounting that erodes margins.

**Recommendation:** Investigate Furniture category discounts and supplier costs. Reducing Furniture discounts by even a small amount could meaningfully improve overall profitability.

### 2. West Region Leads, South Region Underperforms
The West region generates the highest revenue (~$0.8M), followed by East, Central, and South. The South region lags significantly behind other regions.

**Recommendation:** Analyse what's different about the South — is it fewer customers, lower order values, or limited product availability? This could reveal a growth opportunity.

### 3. Strong Seasonal Pattern — Revenue Peaks in Nov–Dec
The monthly trend line shows a clear pattern: revenue dips in January–February, stays moderate through mid-year, and spikes sharply in September through December (likely driven by back-to-school and holiday shopping).

**Recommendation:** Align marketing spend and inventory planning with this seasonality — increase investment in Q4 and reduce in Q1 to optimise ROI.

### 4. Average Order Value of $229.86 with 12.5% Margin
With 10K orders generating $2M in revenue, the average order is ~$230. The overall profit margin of 12.5% is moderate for retail, suggesting there is room to improve through pricing optimisation or discount reduction.

## How to Use
1. Download the `Sales_Performance_Dashboard.pbix` file
2. Open it in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
3. Use the **Year**, **Region**, and **Category** slicers in the top-right corner to filter the entire dashboard
4. Click on any bar or chart element to cross-filter other visuals

## Project Structure
```
PowerBI-Sales-Dashboard/
├── Sales_Performance_Dashboard.pbix    # Power BI dashboard file
├── Sales_Performance_Dashboard.pdf     # PDF export for quick viewing
├── Sample_ Superstore.csv             # Source dataset
├── dashboard_screenshot.png            # Dashboard preview image
└── README.md                          # This file
```

## Skills Demonstrated
- Data cleaning and transformation (Power Query, M code)
- DAX measures (SUM, COUNTROWS, DIVIDE, time intelligence)
- KPI dashboard design with interactive slicers
- Business insight generation and data storytelling
- Version control with Git and GitHub

## Author
**Nikhil Krishnan Karthikeyan Nair**
- 🔗 [LinkedIn](https://www.linkedin.com/in/nikhil-kkn)