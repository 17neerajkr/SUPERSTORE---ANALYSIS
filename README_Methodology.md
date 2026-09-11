# Superstore Data Analyst Assessment --- Final Submission

## Files

-   `Superstore_Assessment_GoogleSheet_Ready.xlsx` --- upload/open in
    Google Sheets. It contains all required worksheets.
-   `Superstore_Data_Analyst_Assessment.ipynb` --- complete
    Python/Jupyter notebook with Q1--Q10 analysis and reproducible code.
-   `Processed_Data.csv` --- analysis-ready processed dataset.
-   `Dashboard_Data.csv` --- compact data extract suitable for Looker
    Studio.
-   `dashboard_mockup.png` --- dashboard design reference.
-   `Management_Presentation.pptx` --- 7-slide senior-management
    presentation.
-   `README_Methodology.md` --- this methodology document.

## Dataset

**Sample - Superstore**, sourced from Tableau Public Sample Data:
https://public.tableau.com/app/resources/sample-data

The supplied dataset contains **9,994 rows and 21 source columns**.

## Business problem

How can management grow sales while protecting profit, especially by
reducing margin leakage from discounts and low-profit product areas?

## Methodology

1.  Loaded the supplied CSV with Pandas.
2.  Parsed Order Date and Ship Date.
3.  Checked missing values and exact duplicates.
4.  Validated date order, discount range, quantity and sales.
5.  Created Ship Days, Year, Month, Year-Month, Profit Margin, Profit
    per Unit, Profitability, Discount Band and Order Sales.
6.  Used unique Order IDs for order-level KPIs.
7.  Flagged statistical outliers using IQR without deleting them.
8.  Compared category, sub-category, region, segment, year and
    discount-band performance.
9.  Avoided causal claims where the dataset only supports association.
10. Prepared dashboard-ready data.

## Key findings

-   Total Sales: **\$2,297,201**

-   Total Profit: **\$286,397**

-   Overall Profit Margin: **12.5%**

-   Furniture contributes **32.3% of sales** but only **6.4% of
    profit**.

-   30% discount band has about **-48.2% margin**.

-   West is the strongest region by margin; Central is the weakest.

-   Home Office has the highest segment margin.

## Looker Studio

The assessment requires an actual interactive Looker Studio dashboard
and shareable link. This cannot be published from this environment
because it requires the submitter's Google account. Create it using
`Dashboard_Data.csv` or the Google Sheet, then paste the link into the
`Q8` worksheet.

## Important analytical caveat

The data is a historical/fictitious sample. The analysis identifies
patterns and opportunities, but high discounts cannot be stated to have
caused losses without further causal or cost-level analysis.
