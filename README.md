# digital-wallet-analytics

Simulating a Fintech Rewards Platform
 
Project Overview

  This project analyzes user transaction data from a digital wallet platform to understand spending behavior, cashback efficiency, and engagement patterns.
  
  The analysis simulates how a fintech rewards platform like Super.com can use data to optimize cashback incentives, improve retention, and manage incentive costs.

Business Objectives

  Understand how users spend across categories and time

  Evaluate the efficiency of cashback incentives

  Identify high-value and incentive-sensitive user segments

  Derive actionable insights for incentive optimization and retention

Dataset Overview

  Source: Kaggle (Digital Wallet Transactions dataset)

  Scope: 4,755 successful transactions across 3,783 users

Key Fields:

  User & transaction identifiers

  Transaction amount, fees, cashback, loyalty points

  Product categories, merchants, payment methods

  Device type, location, timestamp

Only successful transactions were analyzed to ensure insights reflect realized user spending and rewards activity.

Data Cleaning & Feature Engineering

  Filtered dataset to include only successful transactions

  Removed non-informative identifiers and overly granular fields

  Converted transaction timestamps to datetime format

Engineered key features:

  net_spend = product amount + transaction fee

  cashback_rate = cashback ÷ product amount

  Created time dimensions (month, day of week) to support temporal analysis

Key Analyses & Insights
  1️) Platform-Level Performance

  2) Total gross transaction value: ~$23.6M

  3) Total cashback distributed: ~$241K

  4) Effective cashback rate (weighted): ~1.02%

Cashback incentives are meaningful but controlled, indicating efficient incentive deployment relative to platform spend.


Category-Level Performance

  Spending is well-distributed across essential and discretionary categories.

  Utilities, subscriptions, and recurring payments drive consistent volume.

  Cashback efficiency varies slightly across categories, becoming meaningful at scale.

  High-volume, low-efficiency categories represent strong margin-efficient segments, while higher-efficiency categories warrant periodic incentive review.

Cashback Efficiency Analysis

  A category-level comparison of cashback per dollar spent shows:

  Cashback efficiency is tightly clustered around ~1%

  Some categories receive higher incentives without proportional spend increases
  
  Uniform cashback increases are unlikely to yield proportional revenue gains.

User-Level Behavior

  Median user spend: ~$6.0K

  Spending distribution is right-skewed, with a small group of high-value users

  75% of users complete only one transaction

  The platform is primarily used for situational or scheduled payments, highlighting retention and repeat-usage as the largest growth opportunity.

Cashback Sensitivity

  No strong positive relationship between higher cashback rates and total user spend

  High-spend users cluster at low-to-moderate cashback levels

  Extremely high cashback rates are driven by small transaction sizes, not high value

  Cashback functions better as a retention and activation tool than as a driver of high-value spending.

Time-Based Insights

  Monthly spend remains stable with moderate seasonal peaks

  Spending patterns are consistent across weekdays and weekends

  Engagement is driven by recurring financial needs rather than impulse timing, reducing the need for aggressive day-of-week targeting.


Key Recommendations

  Focus cashback incentives on second and third transactions to improve repeat engagement among low- and mid-frequency users.

  Protect high-margin categories with stable spend and low incentive costs.

  Use seasonal peaks for targeted promotional campaigns rather than uniform incentive increases.

  Prioritize loyalty-based benefits for high-spend users who show low sensitivity to cashback.

Tools & Technologies

  Python: pandas, numpy, matplotlib

  Environment: Jupyter Notebook

  Techniques: Aggregation, segmentation, time-series analysis, incentive efficiency analysis
