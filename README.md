
## Dataset Source

The dataset used in this project is publicly available from the UCI Machine Learning Repository.

**Dataset:** [Online Retail Dataset – UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail)

The dataset contains 541,909 transaction records from a UK-based online retailer, covering December 2010 to December 2011.

# Retail Sales & Customer Analysis | Python & Pandas

## Project Overview

This project analyzes the UCI Online Retail transaction dataset to understand sales performance, merchandise demand, geographic markets, and customer purchasing behavior.

The analysis uses **Python and Pandas** for data preparation and aggregation, and **Matplotlib** for visualizations. The accompanying business report translates the findings into practical business recommendations.

**Period covered:** December 2010–9 December 2011  
**Original dataset:** 541,909 transaction-line records  
**Tools:** Python, Pandas, NumPy, Matplotlib, Jupyter Notebook

## Business Questions

- How did net transaction revenue change over time?
- Which merchandise products and markets generated the most revenue?
- How concentrated was revenue among the highest-value customers?
- What do average order value, purchase frequency, and repeat purchasing reveal about customer behavior?
- How did the number of unique purchasing customers change month by month?

## Data Preparation

- Classified transactions into candidate sales, cancellations, zero-price transactions, nonstandard adjustments, and bad-debt adjustments.
- Retained eligible sales and cancellations to calculate **net transaction revenue** rather than treating all positive sales as final revenue.
- Identified and separated special non-merchandise codes, such as shipping, financial charges, discounts, samples, manual entries, and gift vouchers, for merchandise-focused analysis.
- Standardized relevant stock codes and derived revenue and date fields.
- Retained transactions without a CustomerID for overall revenue and product analysis, but excluded them from customer-level metrics.
- Retained exact duplicate-looking rows because the dataset does not establish that they are erroneous duplicates.

## Key Findings

| Area | Finding |
| --- | --- |
| Net transaction revenue | Approximately **£9.76 million** across eligible sales and cancellations |
| Highest-revenue month | **November 2011:** approximately **£1.46 million** in net transaction revenue |
| Leading merchandise product | **REGENCY CAKESTAND 3 TIER:** approximately **£164,762** in net merchandise revenue |
| Leading international merchandise market | **Netherlands:** approximately **£283,480** (excluding the United Kingdom) |
| Top 10 identified customers | Generated approximately **16.54%** of identifiable-customer merchandise revenue |
| Average order value | Approximately **£476.09** per identified-customer merchandise sales invoice |
| Purchase frequency | Approximately **4.25** sales invoices per identified customer |
| Observed repeat customer rate | Approximately **65.27%** of identified customers placed more than one sales invoice |
| Peak unique purchasing customers | **November 2011:** **1,660** identified purchasing customers |

## Business Recommendations

- Prepare inventory and fulfillment capacity ahead of periods with stronger demand, while validating seasonality against additional years of data.
- Prioritize availability and merchandising of high-revenue products without overlooking profitability and returns.
- Investigate expansion opportunities in established international markets, accounting for delivery costs and local demand.
- Develop targeted retention and customer-service strategies for repeat and high-value purchasers.
- Improve CustomerID capture and transaction classification to strengthen future customer and revenue reporting.

## Project Files

- **[Jupyter Notebook](Untitled168%20%282%29.ipynb)** — data cleaning, calculations, and visualizations.
- **[Business Analysis Report](Retail_Sales_Customer_Analysis_Report.pdf)** — detailed findings, charts, recommendations, and limitations.

## Limitations

- **December 2011 is incomplete:** The dataset ends on 9 December, so December totals are not comparable with complete months.
- Some transactions have missing CustomerIDs; customer metrics cover **identified customers only**.
- Repeat purchasing is measured within the observed dataset; it is **not a cohort retention rate**.
- Merchandise revenue excludes selected special transaction codes, including discounts and manual entries, and should not be interpreted as a fully discount-adjusted product profitability measure.
- Potential duplicate-looking records were retained; the source data does not definitively establish whether they are duplicates.
- Results describe historical transactions and do not, by themselves, establish future demand or recurring seasonality.

## Dataset Source

UCI Machine Learning Repository — **Online Retail** dataset.

The source data is not included in this repository unless redistribution terms and file size are checked.

---

*Portfolio project: Retail Sales & Customer Analysis*

