📊 Superstore Data Analyst Assessment
Professional Data Analyst Assessment — Final Submission Package
This repository contains the complete analysis, processed datasets, dashboard-ready data, Jupyter Notebook, and management presentation developed for the Superstore Data Analyst Assessment.
The objective of this project is to analyze historical sales and profitability data, identify business performance drivers, uncover areas of margin leakage, and provide actionable recommendations for management.
📌 Table of Contents
Project Overview
Business Problem
Dataset
Objectives
Tools & Technologies
Project Methodology
Key KPIs
Key Findings
Business Recommendations
Dashboard
Project Deliverables
Data Quality & Limitations
Analytical Approach
Reproducibility
Conclusion
📊 Project Overview
The Sample Superstore dataset was analyzed to understand sales performance, profitability, discount behavior, customer segments, geographic performance, and product-level profitability.
The analysis focuses on answering a central management question:
How can management grow sales while protecting profit, particularly by reducing margin leakage from excessive discounts and low-profit product areas?
The project combines:
Data cleaning and validation
Exploratory Data Analysis
Descriptive analytics
Profitability analysis
Discount analysis
Product and category analysis
Regional and segment analysis
Outlier analysis
Business recommendations
Dashboard preparation
Management-level presentation
🎯 Business Problem
Although the business generates substantial sales, profitability is not distributed evenly across products, regions, segments, and discount levels.
The analysis therefore focuses on identifying:
Where sales are being generated.
Where profits are being generated.
Which product areas are underperforming.
How discounts relate to profitability.
Which regions and customer segments perform best.
Where management should prioritize corrective action.
How profitable opportunities can be scaled.
📂 Dataset
Source
Sample - Superstore
Source: Tableau Public Sample Data
The supplied dataset contains:
AttributeValueRecords9,994Source Columns21Dataset TypeHistorical / Sample Business Data
Important Fields
The analysis uses fields including:
Order ID
Order Date
Ship Date
Ship Mode
Customer ID
Customer Name
Segment
Country
City
State
Postal Code
Region
Product ID
Category
Sub-Category
Product Name
Sales
Quantity
Discount
Profit
🎯 Objectives
The project was designed to:
Understand overall business performance.
Calculate important sales and profitability KPIs.
Evaluate category and sub-category performance.
Analyze regional and customer-segment performance.
Understand the relationship between discounts and profit.
Identify potential sources of margin leakage.
Detect unusual observations and outliers.
Identify business opportunities.
Provide actionable management recommendations.
Prepare data for an interactive dashboard.
Communicate findings through a management presentation.
🛠 Tools & Technologies
Tool / TechnologyPurposePythonData processing and analysisPandasData manipulationNumPyNumerical analysisMatplotlib / VisualizationExploratory analysisJupyter NotebookReproducible analysisExcel / Google SheetsStructured analysis and submissionLooker StudioDashboard visualizationPowerPointManagement presentationMarkdownDocumentation🔎 Project Methodology
The analysis followed a structured data analytics workflow.
1. Data Loading
The supplied dataset was loaded into Python using Pandas.
2. Data Cleaning
The following checks were performed:
Missing-value assessment
Duplicate-record assessment
Data-type validation
Date parsing
Numeric-field validation
Discount validation
Quantity validation
Sales validation
3. Data Transformation
Additional analytical fields were created, including:
Ship Days
Year
Month
Year-Month
Profit Margin
Profit per Unit
Profitability
Discount Band
Order Sales
4. KPI Calculation
Order-level calculations use unique Order IDs where appropriate to avoid overstating order counts.
5. Exploratory Data Analysis
Performance was evaluated across:
Category
Sub-Category
Region
Segment
Year
Discount Band
6. Outlier Analysis
Statistical outliers were identified using the Interquartile Range (IQR) approach.
Outliers were flagged rather than automatically removed, because unusual transactions may contain legitimate business information.
7. Business Analysis
The analysis moved beyond descriptive statistics to identify:
Profitability gaps
Margin leakage
Discount-related patterns
Product opportunities
Regional opportunities
Segment opportunities
8. Recommendation Development
Findings were translated into practical management recommendations based on the evidence available in the dataset.
9. Dashboard Preparation
A compact dataset was prepared specifically for dashboard visualization in Looker Studio.
📈 Key KPIs
KPIResultTotal Sales$2,297,201Total Profit$286,397Overall Profit Margin12.5%Total Records9,994
These KPIs provide the high-level baseline for evaluating the business performance.
🔍 Key Findings
1. Furniture Has a Significant Profitability Gap
Furniture contributes approximately:
32.3% of total sales
Only 6.4% of total profit
This indicates a significant difference between revenue contribution and profit contribution.
Business implication
Furniture requires deeper profitability investigation, particularly at the sub-category and product level.
2. High Discounts Are Associated With Poor Margins
The 30% discount band shows approximately:
-48.2% margin
This represents a significant profitability concern.
Business implication
Discounting should be governed more carefully, particularly for products or segments where additional discounts do not generate sufficient incremental value.
3. Regional Profitability Is Uneven
The analysis indicates that:
West is the strongest region by margin.
Central is the weakest region by margin.
Business implication
Regional strategies should not be identical across the business.
The Central region requires additional investigation into:
Product mix
Discounting
Customer mix
Sales strategy
Operational factors
4. Home Office Shows Strong Profitability
The Home Office segment demonstrates the highest segment margin.
Business implication
Management should investigate opportunities to scale profitable Home Office customers and products while maintaining healthy margins.
💡 Business Recommendations
1. Tighten Discount Governance
Priority: High
Implement stronger discount controls for transactions involving high discount levels.
Recommended actions:
Establish discount approval thresholds.
Monitor margin impact before approving large discounts.
Evaluate discount performance by product and customer segment.
Identify products where discounts consistently generate negative margins.
Develop margin-based pricing guidelines.
Expected objective
Increase realized margin while maintaining commercially valuable sales.
2. Launch a Furniture Profitability Recovery Plan
Priority: High
Furniture generates a substantial share of sales but a disproportionately small share of profit.
Recommended actions:
Analyze Furniture at sub-category level.
Identify consistently loss-making products.
Review high-discount Furniture transactions.
Investigate product-level margin leakage.
Review pricing and discount strategies.
Prioritize profitable Furniture products for growth.
Expected objective
Improve Furniture profitability without unnecessarily sacrificing revenue.
3. Scale Profitable Opportunities and Improve Central
Priority: Medium
Use profitable segments and regions as benchmarks while investigating weaker areas.
Recommended actions:
Study the drivers behind strong West-region performance.
Analyze Central-region margin leakage.
Scale high-performing Home Office opportunities.
Compare product mix between high- and low-performing regions.
Replicate successful commercial practices where appropriate.
Expected objective
Improve overall profitability through targeted regional and segment strategies.
📊 Dashboard
The project includes a dashboard-ready data extract intended for Looker Studio.
Recommended Dashboard Sections
Executive KPI Section
Total Sales
Total Profit
Profit Margin
Orders
Quantity
Sales & Profit Trends
Sales by Year
Profit by Year
Monthly Sales Trend
Monthly Profit Trend
Product Performance
Category Sales
Category Profit
Sub-Category Profitability
Top / Bottom Products
Discount Analysis
Discount Band
Sales
Profit
Profit Margin
Geographic Analysis
Region Sales
Region Profit
Regional Margin
Customer Analysis
Segment Sales
Segment Profit
Segment Margin
Dashboard Data
Dashboard_Data.csv is provided as a compact dashboard-ready dataset.
Note: Publishing an interactive Looker Studio dashboard requires access to the submitter's Google account. The dashboard should be published using the provided dashboard-ready data and the final shareable link should be added to the assessment submission.
📁 Project Deliverables
FileDescriptionSuperstore_Assessment_GoogleSheet_Ready.xlsxExcel workbook containing the required worksheets and assessment outputsSuperstore_Data_Analyst_Assessment.ipynbComplete Python/Jupyter Notebook containing the analysisProcessed_Data.csvCleaned and analysis-ready datasetDashboard_Data.csvCompact dataset prepared for Looker Studiodashboard_mockup.pngDashboard design/reference mockupManagement_Presentation.pptxManagement-level presentation summarizing findings and recommendationsREADME_Methodology.mdProject documentation and methodology🧪 Data Quality & Limitations
Several validation and quality checks were performed before analysis.
Data Quality Checks
Missing values
Duplicate records
Date consistency
Ship-date validation
Discount-range validation
Quantity validation
Sales validation
Outlier identification
Analytical Limitations
The dataset represents historical/sample business data. Therefore:
Observed relationships should not automatically be interpreted as causal.
High discounts are associated with poor profitability, but the dataset alone does not prove that discounts caused losses.
Additional information such as cost structure, pricing strategy, customer acquisition costs, and operational costs could improve the analysis.
Historical performance may not necessarily predict future performance.
Important Analytical Principle
The analysis distinguishes between correlation/association and causation and avoids unsupported causal claims.
🧠 Analytical Approach
The project follows a structured analytical framework:
Raw Dataset
     │
     ▼
Data Loading
     │
     ▼
Data Quality Checks
     │
     ▼
Data Cleaning & Transformation
     │
     ▼
KPI Calculation
     │
     ▼
Exploratory Data Analysis
     │
     ├── Category Analysis
     ├── Product Analysis
     ├── Regional Analysis
     ├── Segment Analysis
     ├── Discount Analysis
     └── Time-Series Analysis
     │
     ▼
Business Insights
     │
     ▼
Actionable Recommendations
     │
     ├── Dashboard
     └── Management Presentation

🔄 Reproducibility
The primary analytical workflow is available in:
Superstore_Data_Analyst_Assessment.ipynb

The notebook contains the Python-based processing and analytical workflow required to reproduce the major analysis steps.
Recommended Execution Order
Open the Jupyter Notebook.
Load the source dataset.
Execute the data-quality checks.
Execute the transformation cells.
Run the KPI calculations.
Run the exploratory analysis.
Review the business findings.
Review the recommendations.
Use Dashboard_Data.csv for dashboard development.
📌 Final Conclusion
The analysis indicates that the business has a meaningful opportunity to improve profitability without relying solely on additional sales growth.
The strongest opportunities are concentrated around:
Better discount governance
Furniture profitability improvement
Scaling profitable customer segments
Improving weaker regional performance
Using margin-based decision-making alongside sales growth
The key management principle emerging from the analysis is:
Growth should be evaluated not only by how much revenue is generated, but by how much profitable revenue is generated.
👤 Project Type
Data Analyst Assessment / Placement Project
Core Skills Demonstrated
Python · Pandas · Data Cleaning · EDA · KPI Analysis · Business Analytics · Profitability Analysis · Dashboard Preparation · Data Visualization · Business Recommendations · Management Reporting
✅ Submission Status
DeliverableStatusDataset Processing✅ CompleteData Quality Checks✅ CompleteKPI Analysis✅ CompleteExploratory Analysis✅ CompleteBusiness Insights✅ CompleteRecommendations✅ CompleteDashboard Data✅ CompleteDashboard Mockup✅ CompleteManagement Presentation✅ CompleteMethodology Documentation✅ CompletePrepared for professional Data Analyst assessment and evaluation.
