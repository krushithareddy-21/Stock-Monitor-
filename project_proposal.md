# Stock Monitor – Stock-Out Risk and Demand Analytics

## 1. Project Title

**Stock Monitor – Stock-Out Risk and Demand Analytics**

## 2. Team Members

| Member   | Name              | Roll number |
|--------  |-------------------|-------------|
| Member 1 | G.Krushitha Reddy | 2503A52619  |
| Member 2 | Sk. Yasmeen Shaik |  2503A52603 |
| Member 3 | G.Bhuvana Kruthi  |  2503A52630 |

## 3. Introduction

Retail stores and warehouses need to keep enough products available to meet customer demand. Too little stock can lead to products running out, while ordering more than needed can leave excess inventory. Reviewing these conditions across many products, stores, and dates can be difficult when working directly with raw data.

This project uses a retail inventory dataset to examine inventory levels, units sold, units ordered, and demand forecasts. It will present the analysis in an interactive Power BI dashboard so that users can view inventory status and demand-related risks in a clear way.

## 4. Problem Statement

Managers may find it difficult to identify products with low stock, compare sales with available inventory, or notice when actual sales differ from the demand forecast. Without a clear summary of this information, products that need attention may be overlooked and ordering decisions may not be well informed.

The project addresses this problem by cleaning and analyzing the available inventory data, identifying products in low, medium, and high stock-out risk groups, and displaying the results through charts and dashboard filters.

## 5. Motivation

Inventory decisions affect the availability of products and the amount of stock held by a store or warehouse. The team is motivated to use data analysis and visualization to make inventory information easier to understand. A dashboard can help users review products and compare patterns across stores, categories, regions, and dates without manually scanning the full dataset.

## 6. Objectives

- Prepare the retail inventory data for analysis.
- Review inventory levels alongside units sold and units ordered.
- Compare the dataset's demand forecast with actual units sold.
- Identify products labelled with low, medium, or high stock-out risk.
- Highlight products that may need monitoring or a reorder review.
- Examine inventory patterns across stores, product categories, and regions.
- Present the results in an interactive Power BI dashboard.

## 7. Dataset Description

The project uses a retail store inventory dataset. The workspace includes a raw CSV file and a cleaned CSV file. The cleaned file contains 73,100 records and includes the original fields along with derived analysis fields.

| Field                  | Description                                                                |
|------------------------|----------------------------------------------------------------------------|
| Date                   | Date associated with the inventory and sales record                        |
| Store ID               | Identifier for the store                                                   |
| Product ID             | Identifier for the product                                                 |
| Category               | Product category                                                           |
| Region                 | Region associated with the record                                          |
| Inventory Level        | Inventory quantity recorded                                                |
| Units Sold             | Number of units sold                                                       |
| Units Ordered          | Number of units ordered                                                    |
| Demand Forecast        | Forecast value provided in the dataset                                     |
| Price                  | Recorded product price                                                     |
| Demand Difference      | Derived value comparing demand forecast and units sold                     |
| Stock Coverage         | Derived field included in the cleaned dataset to support inventory analysis|
| Stock-Out Risk         | Risk category included in the cleaned dataset                              |
| Reorder Recommendation | Suggested action included in the cleaned dataset                           |

The demand forecast is treated as an existing dataset field. This project does not claim to train a machine-learning model or create a new demand forecast.

## 8. Data Preprocessing

The raw dataset is reviewed and prepared before analysis. The preprocessing work includes:

1. Loading the inventory data from the available file.
2. Checking field names, data types, and values.
3. Checking for missing values and duplicate records.
4. Cleaning and preparing the data for analysis.
5. Creating useful derived fields, including Demand Difference and Stock Coverage.
6. Using the prepared data, which also includes stock-out risk and reorder recommendation fields, for analysis and visualization.

Demand Difference compares the provided forecast with actual units sold. The exact calculation and the rules used for Stock Coverage and risk categories should be stated in the final report based on the team's implemented preprocessing. The project will not assume or present thresholds that have not been verified.

## 9. Methodology / Project Workflow

The project follows these stages:

1. **Data Collection:** Use the available retail inventory dataset.
2. **Data Cleaning:** Check data quality, including missing values and duplicate records.
3. **Data Preprocessing:** Prepare fields and derive Demand Difference and Stock Coverage.
4. **Data Analysis:** Compare inventory, sales, orders, forecast values, and risk categories.
5. **Data Visualization:** Choose charts that make the main comparisons and patterns easy to understand.
6. **Interactive Dashboard:** Build a Power BI dashboard with summary indicators, charts, and slicers.
7. **Final Report:** Document the dataset, preparation, analysis, visuals, findings, and limitations.

## 10. Data Analysis

The analysis will focus on descriptive comparisons in the available data:

- Group products by the low, medium, and high stock-out risk labels.
- Compare inventory levels with units sold to find records that may need attention.
- Compare demand forecast values with actual units sold and review Demand Difference.
- Review inventory and sales across stores, categories, and regions.
- Use units ordered and the available reorder recommendation field as additional context when reviewing products for monitoring or a reorder decision.

These results support review by a manager; they do not guarantee that a product will run out or replace the manager's ordering judgment.

## 11. Data Visualization

The project will use visualizations to summarize the analysis. Possible visuals include:

- **KPI cards** for selected inventory, sales, order, and risk totals.
- **Bar charts** to compare inventory or units sold by category, store, or region.
- **Pie or donut chart** to show the distribution of stock-out risk categories.
- **Treemap** to show the relative contribution of categories or products to a selected measure.
- **Map**, if the dataset contains usable geographic information at a suitable level.
- **Comparison chart** for demand forecast and units sold.

The final visuals will be selected based on the fields available and the clarity of the result. A map will only be included if the region values can be represented meaningfully.

## 12. Interactive Dashboard

The planned dashboard will be built in Power BI. It will provide a summary view of inventory and sales, along with charts for demand comparisons and stock-out risk. Slicers will allow users to focus on available dimensions such as date, store, category, or region.

The dashboard is intended to help a store or warehouse manager quickly review overall status and then explore the products or groups that may need closer attention. Its results will reflect the available dataset and the team's documented analysis rules.

## 13. Expected Results

The expected deliverables are:

- A cleaned dataset prepared for analysis.
- A summary of inventory, sales, orders, and demand forecast comparisons.
- Identification of products in the available low, medium, and high stock-out risk groups.
- Visual comparisons across stores, categories, and regions.
- An interactive Power BI dashboard that helps users explore the results.
- A final report explaining the process, observations, and limitations.

The project is expected to make relevant patterns easier to review. It does not promise to prevent stock-outs or eliminate excess ordering.

## 14. Target Users

- Store managers
- Warehouse managers
- Inventory management teams

## 15. Tools and Technologies

| Tool or technology  | Use in the project                                    |
|---------------------|-------------------------------------------------------|
| CSV and Excel files | Store and review the raw and prepared inventory data  |
| Python and Pandas   | Data preparation and analysis, where used by the team |
| Microsoft Power BI  | Planned interactive dashboard and visualizations      |

The final report will identify the tools actually used during implementation.

## 16. Team Member Responsibilities

The following is a suggested division of work. The team can confirm or adjust the allocation during the project; it does not describe completed individual contributions.

| Team member                      | Suggested responsibility                                                    |
|----------------------------------|-----------------------------------------------------------------------------|
| Member 1:G.Krushitha 2503A52619  | Review the dataset, check data quality, and document preprocessing          |
| Member 2:Sk.Yasmeen 2503A52603   | Perform the inventory and demand analysis and summarize findings            |
| Member 3:G.Bhuvana 2503A52630    | Build the Power BI visuals and dashboard, and help prepare the final report |

All three members will review the results and contribute to the final submission.

## 17. Future Scope

If the project is extended, it could include more historical data or additional business context, such as lead times or product availability targets, if those data become available. The analysis and dashboard could then be updated to reflect that information. Any future forecasting or automated recommendations would require separate design, implementation, and validation; they are not part of the current proposal.

## 18. Conclusion

Stock Monitor will use a retail inventory dataset to examine stock levels, sales, orders, demand forecasts, and stock-out risk categories. By preparing the data and presenting useful comparisons in Power BI, the project aims to make inventory patterns easier for store and warehouse managers to review. The dashboard will support informed decisions while keeping the analysis within the limits of the fields and rules actually available.

## 19. References

1. Project raw dataset: [`RAW_DATASET.csv`](../RAW_DATASET.csv).
2. Project cleaned dataset: [`stock_monitor_clean_dataset_final.csv`](../stock_monitor_clean_dataset_final.csv).
3. Project workbook: [`Stock_Monitor_Preprocessed_Krushitha.xlsx`](../Stock_Monitor_Preprocessed_Krushitha.xlsx).
4. Project overview and existing dataset notes: [`README.md`](../README.md).
5. Microsoft Power BI documentation: [https://learn.microsoft.com/power-bi/](https://learn.microsoft.com/power-bi/).
