# Credit Card Customer & Transaction Analysis | Power BI

An interactive Power BI report for exploring credit card revenue, transaction activity, and customer segments across two report pages.

## Project Overview

This project brings together transaction and customer information to help users examine business performance from both financial and demographic perspectives. It supports comparisons across card categories, spending categories, payment methods, and customer groups.

**Report file:** `Credit Card Customer Report.pbix`

## Business Questions

- How do revenue and transaction volume vary by quarter?
- Which card categories and expenditure types contribute to revenue?
- How does revenue differ across payment methods?
- How are revenue and acquisition costs distributed across card categories?
- How does revenue vary by occupation, income group, age group, and education?
- What differences appear across gender, marital status, dependents, and state?

## Report Pages

### 1. Credit Card Transaction Report

An overview of credit card financial performance and transaction activity.

**KPI cards**
- Total revenue
- Total interest earned
- Total transaction amount
- Total transaction volume

**Visual analysis**
- Quarterly revenue and transaction volume
- Revenue by expenditure type, education level, and customer occupation
- Revenue by payment method (`Use Chip`)
- Customer acquisition cost by card category
- Card-category summary of revenue, interest earned, and transaction amount
- Client-record counts by quarter, gender, income group, and card category

### 2. Credit Card Customer Report

A customer-focused view of revenue distribution and demographic segments.

**KPI cards**
- Total revenue
- Total interest earned
- Total customer income
- Sum of customer satisfaction scores

**Visual analysis**
- Revenue trends over time, segmented by gender
- Revenue distribution by gender
- Revenue by income group, state, age group, marital status, education, and dependent count, segmented by gender
- Occupation-level comparison of revenue, transaction amount, and income
- Client-record counts by quarter

> **Metric interpretation:** The customer satisfaction card currently uses a sum, not an average. Client-count visuals use nonblank counts of `Client_Num`, not distinct customer counts. Interpret these metrics accordingly.

## Interactive Exploration

Both pages include a **week-start-date slicer**. Use the available report selections to focus on a period or customer segment and explore the associated visuals.

## Data Structure

The report visuals reference two main tables:

| Table | Fields used in the report |
| --- | --- |
| `credit_card` | Client number, week start date, quarter, card category, expenditure type, payment method, revenue, interest earned, transaction amount, transaction volume, and acquisition cost |
| `customer` | Gender, age group, education level, marital status, dependent count, occupation, income, income group, state, and satisfaction score |

`Client_Num` is referenced in client-count visuals. Review the model in Power BI Desktop to confirm relationship keys, cardinality, and filter direction before extending the analysis.

## Tools & Skills Demonstrated

- **Microsoft Power BI** — report authoring and interactive analysis
- **Data visualization** — KPI cards, bar charts, line charts, combo charts, treemaps, and tables
- **Customer segmentation** — demographic and income-based comparisons
- **Business analysis** — revenue, transaction, interest, and acquisition-cost analysis

## Repository Structure

```text
.
├── README.md
└── Credit Card Customer Report.pbix
```


