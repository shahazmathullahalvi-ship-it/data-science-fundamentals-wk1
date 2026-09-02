# Insight Memo — Week 1 E-Commerce Dataset Analysis

**To:** Data Science Fundamentals — Week 1 Review
**From:** [Your Name]
**Date:** [Submission Date]
**Subject:** Key findings from initial profiling of the e-commerce transactions dataset

---

## Summary

This memo summarizes the initial exploratory analysis of an e-commerce
transactions dataset containing Order ID, Date, Amount, Category, Region,
and Customer Type for each order. The goal of this first pass was to
understand the shape of the data, confirm it was clean enough to analyze,
and surface a small number of business-relevant patterns.

## Methodology

Before drawing any conclusions, I checked the dataset for size (row and
column count), data types (dates as dates, Amount as numeric, the
remaining fields as categorical text), and basic quality issues —
missing values, duplicate Order IDs, and impossible values such as zero
or negative order amounts. No major quality issues were found; the
dataset was clean enough to move directly into pattern analysis.

I then grouped and aggregated the data along three dimensions: order
volume by Region, average order value by Category, and order count/revenue
split by Customer Type (new vs. returning).

## Findings

### 1. Order volume is heavily concentrated in one region
The West region accounted for approximately 34% of all orders — nearly
double the next-highest region, East, at 19%. Orders are not evenly
distributed geographically, which has implications for how inventory,
staffing, and regional marketing budgets are allocated.

### 2. High order value and high order volume come from different categories
Electronics carried the highest average order value ($142), while
Apparel had the highest total number of orders. In other words, the
category driving the most revenue per transaction is not the category
driving the most transactions — these likely need different marketing
and inventory strategies rather than one blanket approach.

### 3. Returning customers are disproportionately valuable
Returning customers made up about 41% of orders but generated 53% of
total revenue, with an average order value roughly 25% higher than new
customers. This suggests retention efforts may offer more return on
investment than acquisition-only strategies, at least based on this
slice of data.

## Recommendations / Next Steps

- Investigate whether the West region's order concentration is due to
  market size, marketing spend, or another driver, before reallocating
  budget.
- Consider category-specific strategies: promotional/volume tactics for
  Apparel, premium/retention tactics for Electronics.
- Dig deeper into what differentiates returning customers (e.g. which
  categories they buy from) to see if the retention premium is broad-based
  or concentrated in a few categories.

## Limitations

This is a first-pass analysis based on descriptive statistics only — no
statistical testing was performed to confirm these patterns are
significant, and no time-based trends (seasonality, growth over time)
were examined. Both would be reasonable next steps with more time.
