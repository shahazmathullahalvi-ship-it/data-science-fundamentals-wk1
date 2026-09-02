
# Data Science Fundamentals — Week 1

## Project Overview

This repository contains my Week 1 Data Science Fundamentals project — a first
exploratory analysis of a real, open e-commerce transactions dataset. The goal
was to get comfortable profiling a dataset, spotting data quality issues, and
pulling out a few meaningful business insights before writing any Python.

## Dataset

The dataset captures individual e-commerce orders, with the following fields:

| Field         | What It Captures                        |
|---------------|------------------------------------------|
| Order ID      | Unique identifier for each transaction    |
| Date          | When the order was placed                 |
| Amount        | Transaction value                         |
| Category      | Product category purchased                |
| Region        | Where the customer is located             |
| Customer Type | New vs returning customer                 |

## Analysis

I started by checking the size and shape of the dataset (row/column count),
confirmed the data types for each field (dates as dates, amounts as numbers,
categories/region/customer type as text), and scanned for obvious quality
issues such as missing values, duplicate Order IDs, and impossible values
(e.g. negative or zero Amount). From there, I looked at basic patterns —
order volume by Region, average order value by Category, and the split
between new and returning customers.

## Key Insights

### 1. Order volume is concentrated in a handful of regions
The West region accounted for roughly 34% of all orders, nearly double the
next-highest region (East, 19%). This suggests marketing spend and
inventory planning may be disproportionately weighted toward one part of
the customer base.

### 2. The highest-value category isn't the highest-volume one
Electronics had the highest average order value ($142), but Apparel had
the highest order count by a wide margin. High ticket size and high
purchase frequency are coming from two different parts of the catalog,
which matters for how each category should be promoted.

### 3. Returning customers spend more per order than new customers
Returning customers made up about 41% of total orders but drove 53% of
total revenue — an average order value roughly 25% higher than new
customers. Retention appears to be a stronger revenue lever here than
acquisition alone.

## Conclusion

Together, these patterns point to a business that is regionally
concentrated, has a clear split between "high value" and "high volume"
categories, and gets outsized value from repeat customers. With more time,
I'd want to check whether the regional concentration is due to market size
or marketing spend, and whether the returning-customer premium holds
across categories or is driven by one or two of them.

## Skills Demonstrated

- Data profiling and quality checks
- Data interpretation
- Critical thinking
- Insight generation
- Data storytelling
