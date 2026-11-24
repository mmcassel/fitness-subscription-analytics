# Fitness Subscription Analysis: Customer Lifecycle & Growth Sustainability

## Executive Summary

This analysis of fitness subscriptions evaluates customer retention, future subscription revenue, and the payback period on customer acquisition costs (CAC) to assess whether the company's growth strategy is sustainable. The data covers 9,300 customers and about 65,000 transactions from January 2024 to January 2026.

### 1. After how many months do customers typically cancel?

**Customers most often cancel after their third month.** Retention is consistent across every monthly cohort: 85% of customers remain after month 1 and 78% after month 2, then retention drops sharply to **50% at month 3**. Half of all customers are gone at this point, likely when an introductory offer or trial period ends. After month 3, churn slows to about 1–2 percentage points per month, and **about 36% of customers are still subscribed after one year.**

### 2. What is the expected subscription revenue over the next 12 months?

**Subscription revenue is forecast at approximately \$2.52 million for February 2026 – January 2027**, rising from about \$181,500 in February 2026 to about \$239,600 by January 2027. The forecast was generated with a 95% prediction interval: for February 2026, the expected range is about \$171,000 – \$192,000, and the range widens in later months as uncertainty grows. The forecast is driven almost entirely by the growth trend (98.1%), with only a minor seasonal effect (1.9%) peaking in December. Model quality is rated Good using "Describe Forecast" in Tableau.

**Key caveat:** the forecast assumes customer acquisition continues at its recent pace. Growth has come from steadily rising new-customer numbers (from 156 per month in January 2024 to 769 in December 2025), but **January 2026 recorded no new customers**. If acquisition has slowed, actual revenue will fall short of this projection.

### 3. How long does it take the 2024 and 2025 cohorts to reach CAC break-even?

**Both cohorts reached break-even in about 12 months**, by December of their acquisition year:

| Cohort | Customers | Total CAC | Break-even | Cumulative revenue (Jan 2026) | Return on CAC |
|---|---|---|---|---|---|
| 2024 | 2,816 | \$501,537 | December 2024 | \$1.21 million | 2.4× |
| 2025 | 6,484 | \$1,162,459 | December 2025 | \$1.38 million | 1.2× |

The 2025 cohort was more than twice the size of 2024 yet reached break-even in the same timeframe, showing that the business's unit economics have held steady as it scaled.

## Is Growth Sustainable?

**Yes, with an important risk.** Each annual cohort recovers its acquisition cost within about a year, and the 2024 cohort has since returned 2.4 times its CAC, so acquiring customers is profitable over time. However, the business depends heavily on continuous new-customer acquisition: half of each cohort cancels by month 3, and the revenue forecast assumes acquisition keeps growing. The lack of new customers in January 2026 should be investigated immediately.

## Recommendations

1. **Target the month-3 drop-off.** Retention falls from 78% to 50% between months 2 and 3. Retention efforts at this point (renewal incentives, discounted continuation offers, or engagement campaigns before the introductory period ends) offer the biggest opportunity to increase customer lifetime value and shorten the break-even period.
2. **Investigate the January 2026 acquisition gap.** Determine whether the absence of new customers reflects a real slowdown, a marketing pause, or a data issue, since the revenue forecast depends on continued growth.
3. **Monitor the forecast against actual results** monthly, and update it as new data arrives.
4. **Review acquisition costs by channel.** CAC varies widely across acquisition channels; shifting spend toward lower-cost channels would shorten the payback period further.

## Report Pages (Tableau)

- **Customer Cohort:** Retention heatmap by monthly cohort and months since first purchase. Each cell shows the percentage of the cohort's original         customers still subscribed in that month.
- **Revenue Forecast:** Monthly subscription revenue with a 12-month forecast (95% prediction interval).
- **CAC vs. LTV:** Cumulative revenue against total CAC, with a cohort filter for 2024 and 2025 and a dynamic break-even label.

## Repository Contents

- `README.md`: executive summary (this file)
- `MitchCassel_Subscription_Analytics_project.twbx`: Tableau packaged workbook with all three report pages
- `data/Fitness_Subscriptions_Dataset.xlsx`: source data
- `screenshots/`: images of each report page and the data model
  - `customer_cohort.png`
  - `revenue_forecast.png`
  - `cac_vs_ltv.png`
  - `data_model.png`