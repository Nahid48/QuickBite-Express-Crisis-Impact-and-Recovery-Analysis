QuickBite Express — Crisis Recovery Analysis & Strategic Roadmap


In June 2025, QuickBite Express lost 70% of its customer base in less than 90 days. This repository contains a complete Power BI analysis of what went wrong — and how data can guide the recovery.



A comprehensive, data-driven analysis of a food delivery startup's crisis and evidence-based recovery strategy.

Project Type: Business Case Analysis · Data Analytics · Strategic Consulting
Domain: Food Delivery & Consumer Analytics
Time Period Analyzed: January – September 2025
Focus: Crisis Analysis & Recovery Strategy Development
Tools Used: Power BI, DAX, Statistical Analysis
Audience: Data Analysts, Business Strategists, Recruiters


📋 Table of Contents


Project Overview
Problem Statement
Dataset Description
Methodology
Key Findings
Recommendations
Technical Implementation



🎯 Project Overview

Executive Summary

In June 2025, QuickBite Express — a Bengaluru-based food delivery startup (founded 2020) — faced a critical crisis triggered by:


A viral food safety incident involving partner restaurants
A week-long delivery infrastructure outage during monsoon season
Aggressive competitor campaigns capitalizing on operational failures


Crisis Impact:

MetricImpactCustomers churned73,000 (70% of active base)Revenue lost₹27 million (4 months)Customer ratingsCollapsed from 4.5 → 2.3 starsRestaurant partner exodus20%

Key Discovery: Despite the severity, 30% of churned customers (22,000) were recoverable — they left due to operational failure, not dissatisfaction.

Strategic Output: A data-driven ₹70–80M recovery roadmap with 4 strategic pillars, expected to achieve 80–90% recovery within 6–9 months with a 3–4x ROI on reactivation.


💼 Problem Statement

Business Challenge

QuickBite Express requires a comprehensive analysis of its June–September 2025 crisis to:


Understand Crisis Severity — quantify impact across all business metrics
Identify Root Causes — determine what triggered the cascade of failures
Analyze Customer Impact — segment churned customers by recovery probability
Benchmark Competitively — compare against industry peers during the crisis
Design a Recovery Strategy — a data-backed turnaround plan with timelines & ROI
Surface Operational Insights — identify systemic vulnerabilities to prevent recurrence


Analysis Questions Addressed

Primary Analysis (10 questions)


Monthly order decline comparison (pre-crisis vs. crisis)
Top 5 cities by order decline percentage
Top 10 high-volume restaurants with the largest decline
Cancellation rate trend analysis and geographic impact
Delivery SLA performance degradation
Monthly customer rating fluctuations
Negative keyword sentiment analysis
Revenue impact quantification
Loyalty impact on customers with 5+ orders and 4.5+ ratings
High-value customer (top 5%) decline patterns


Secondary Analysis (5 questions + 3 supplementary details)


Competitor comparison (Swiggy, Zomato performance)
External factors contributing to CAC tripling
Most effective recovery strategies
Restaurant type churn risk assessment
Lapsed customer return probability
Priority cities risk analysis
Customer order value shift behavior
Review spike correlation with the delivery outage



📊 Dataset Description

Data Sources

Data TypeSourceTime PeriodRecordsKey MetricsOrdersQuickBite transactional DBJan–Sep 2025149K ordersorder_id, customer_id, order_date, order_total, phaseCustomersCRM systemJan–Sep 2025105K customerscustomer_id, acquisition_date, total_spend, LTVReviews & RatingsReview systemJan–Sep 202548K reviewsrating, sentiment, review_text, dateRestaurant DataPartner DBJan–Sep 202520K restaurantsrestaurant_id, cuisine_type, order_count, statusOperational MetricsDelivery/Operations DBJan–Sep 2025Daily logsdelivery_time, sla_compliance, cancellations, delays

Key Fields & Definitions

Phase Classification


Pre-Crisis: January – May 2025 (5-month baseline)
Crisis: June – September 2025 (4 months of operational failure)


Customer Segmentation

SegmentCountDefinitionTotal Customers105,000All unique customersActive (Pre-Crisis)100,000Placed 1+ orders Jan–MayActive (Crisis)27,000Placed 1+ orders Jun–SepChurned73,000Orders pre-crisis, zero orders during crisisNew18,000First order Jun–Sep 2025Retained14,000Orders in both periods

Order Metrics


Pre-Crisis Monthly Average: 24,000 orders/month
Crisis Monthly Average: 9,000 orders/month
Decline: 69% (24K → 9K)


Revenue Metrics


Pre-Crisis Total: ₹3.8 crore (5 months)
Crisis Total: ₹1.1 crore (4 months)
Difference: ₹2.7 crore lost
Decline: 71%



🔬 Methodology

1. Data Analysis Framework

A. Descriptive Analysis

Purpose: Understand current state and crisis severity

Metrics calculated:


Order volume by month, city, and cuisine
Revenue by component (subtotal, delivery fee, discounts)
Customer counts by status (active, churned, new, retained)
Cancellation rates and SLA compliance trends
Average ratings and sentiment scores


Tools: Power BI aggregations, DAX measures, statistical functions

B. Comparative Analysis

Purpose: Quantify pre-crisis vs. crisis changes

Decline % = (Pre-Crisis Value − Crisis Value) / Pre-Crisis Value × 100

Example — Order Decline:
= (24,000 − 9,000) / 24,000 × 100
= 62.5% decline

Applied to: orders, revenue, ratings, cancellations, SLA compliance

C. Customer Segmentation

Purpose: Identify recoverable customers

SegmentCriteriaSample SizeRationaleHigh Return (60% chance)Pre-crisis orders ≥ 5 AND avg rating ≥ 4.5 AND crisis orders = 022,000Loyal customers lost due to failure, not dissatisfactionMedium Return (40% chance)Pre-crisis orders 3–4 AND avg rating ≥ 3.5 AND crisis orders = 028,000Mixed experience, cost-conscious, winnable backLow Return (15% chance)Pre-crisis orders ≤ 2 AND avg rating < 3.523,000Never fully engaged, low potential

D. Revenue Impact Analysis

Purpose: Quantify financial loss across components

Total Revenue = Subtotal Amount + Delivery Fee + Discounts Applied

ComponentPre-CrisisCrisisDeclineSubtotal₹36.34 Cr₹10.56 Cr70.95%Delivery Fee₹3.47 Cr₹1.01 Cr70.84%Discounts₹2.19 Cr₹0.63 Cr71.34%Total Revenue Lost₹27 million (70.92%)

E. Sentiment Analysis

Purpose: Understand customer perception changes

Rating-based sentiment scoring:

Rating RangeSentimentScore4.5 – 5.0Positive+1.03.5 – 4.4Neutral+0.52.5 – 3.4Mixed−0.5< 2.5Negative−1.0

Average Sentiment = Sum of All Sentiment Scores / Total Reviews

Pre-Crisis Avg Rating: 4.55 → Positive Sentiment
Crisis Avg Rating:     2.30 → Negative Sentiment
Sentiment Change:     −0.49 (1.42-point drop on a −1 to +1 scale)

Keyword Analysis: text parsing on 48K reviews, frequency analysis of negative keywords, clustering by issue category (food quality, delivery, packaging, etc.), crisis vs. pre-crisis comparison.

2. Customer Acquisition Cost (CAC) Analysis

CAC = Total Marketing Spend / Number of New Customers Acquired

Pre-Crisis CAC: ₹50/customer
Crisis CAC:     ₹150/customer
Increase:       300%

Contributing Factors (research-backed):

FactorImpactSource18% GST implementation (Sept 22)+₹20 CACBusiness Standard, Sept 2025Google Ads CPC +42%+₹25 CACMarket data, competitive biddingMonsoon seasonality (−15–20% orders)+₹15 CACIndustry reportsBrand reputation damage+₹40 CACCalculated from conversion rate dropTotal+₹100 (300%)

Implication for Strategy: Reactivating existing customers (₹50/customer) is 3x more cost-effective than acquiring new customers at ₹150/customer during a crisis.

3. Recovery Strategy ROI Modeling

Pillar 1 — Customer Reactivation


Target: 22,000 high-probability customers
Incentive: 40% off + 3 months premium membership
Expected reactivation: 60% (industry benchmark) → 13,200 customers recovered
Avg customer LTV: ₹8,500 → Revenue recovered: ₹1.12 Cr
Investment: ₹20–25M · ROI: 3–4x within 12 months


Pillar 2 — Food Safety Certifications


Investment: ₹15–20M (FSSAI/HACCP audits, badges, promotion)
Expected trust impact: 35–40% improvement
Timeline: 2–3 months to certification
Permanent benefit: ongoing compliance & customer confidence


Pillar 3 — Operational Excellence


Weather-adaptive routing: ₹8–10M
Fleet expansion: ₹12–15M
SLA monitoring systems: ₹5–7M
Total investment: ₹25–30M
Expected SLA improvement: 12% → 40%+ · Cancellation reduction: 11.6% → <7% · Timeline: 6 months


Pillar 4 — Restaurant Support


Commission reduction: 5–10% for 6 months on <50 orders/month
Marketing support: featured listings, campaigns
Financial assistance: working capital support
Target: small cloud kitchens (highest risk)
Expected retention: 85% (vs. current 79%) · Investment: ₹10–15M


Total Recovery Roadmap

Total Investment₹70–80MTimeline6–9 monthsExpected Recovery80–90% of pre-crisis metricsCumulative ROI2.5–3x on total investment

4. Competitive Benchmarking

Methodology: analyzed public financial reports and news articles, tracked market share and revenue growth trends, researched competitor strategies during QuickBite's crisis period, and validated findings against industry reports.

CompetitorJun–Sep 2025ZomatoMarket share 58% (up from 56%) · Revenue growth 67% YoY (29% in July) · Profitable · Strategy: aggressive expansion, captured QuickBite's market shareSwiggyMarket share 42% (maintained) · App installs up 20–25% · Revenue growth 35% YoY · Improving profitability · Strategy: capitalized on QuickBite's operational failures

Impact on QuickBite:


App ranking: #3 → #8
15–25% of lost customers captured by competitors
Market consolidation favored larger, more stable platforms



📈 Key Findings

Crisis Impact Summary

MetricPre-CrisisCrisisChange% ChangeMonthly Orders24,0009,000−15,000−62.5%Monthly Revenue₹7.6M avg₹2.75M avg−₹4.85M−63.8%Total Revenue (period)₹38M₹11M−₹27M−71%Active Customers100,00027,000−73,000−73%Avg Rating4.55 stars2.30 stars−2.25−49%SLA Compliance44%12%−32%−73%Avg Delivery Time40 min60 min+20 min+50%Cancellation Rate6.2%11.6%+5.4%+87%

Root Causes

Primary (Operational)


SLA compliance collapsed from 44% → 12%
Delivery infrastructure failed during monsoon
High cancellations cascaded into negative reviews


Secondary (Reputational)


Food safety viral incident
Negative review sentiment hit 90% by September
Top complaints: Quality (1,596), Safety (1,076), Packaging (997)


Tertiary (Competitive)


Swiggy/Zomato captured 15–25% of lost customers
Competitors ran aggressive campaigns during the crisis
Market consolidation favored larger players


External (Market)


18% GST on delivery (Sept 22) increased costs
Google Ads CPC +42% from competitive bidding
Monsoon seasonality reduced organic demand 15–20%


Recovery Opportunity


High-priority segment: 22,000 customers (60% recovery probability)
Revenue at risk: ₹1.12 Cr annually from the top-5% segment alone
Geographic concentration: Bengaluru (27%) and Mumbai (15%)
Order frequency recovery potential: 4.1 → 2.5+ orders/month



Key Insight: Customers didn't leave due to a preference shift; they left due to service failure. This is reversible through targeted reactivation and operational fixes.




💡 Recommendations

Immediate Actions (Month 1)


Launch VIP Reactivation Campaign — target 22,000 high-return customers with 40% off + 3 months premium; expected 13,200 returns and ₹1.12 Cr recovery
Begin Food Safety Certification — FSSAI + HACCP audits for all partners, visible hygiene badges on the app; expected 35–40% trust improvement
Restaurant Support Program — 5–10% commission reduction for small partners, marketing support for vulnerable cuisines (focus: North Indian/Biryani, 75% at-risk)


Medium-Term (Months 2–6)


Operational Infrastructure Overhaul — weather-adaptive routing, expanded delivery fleet in monsoon-heavy zones, real-time SLA monitoring
Customer Retention Program — tiered loyalty benefits, regular engagement campaigns, continuous feedback loops


Long-Term (Months 6–9)


Market Repositioning — competitive differentiation based on reliability, premium segment recovery (vs. budget), geographic expansion from the recovered base



🛠️ Technical Implementation

Tools & Technologies Used

Data Visualization


Power BI Desktop — interactive dashboards, 7 comprehensive pages
Visual types: cards, charts, tables, donut charts, heatmaps, word clouds
DAX functions: CALCULATE, SWITCH, IF, DIVIDE, DISTINCTCOUNT, SUMMARIZE


Data Analysis


50+ custom DAX measures for segmentation, risk scoring, and ROI
Statistical aggregations, trend analysis, probability scoring
Modeling: customer lifetime value, churn probability, recovery potential



📂 Repository Structure

quickbite-express-crisis-recovery-analysis/
├── README.md
├── LICENSE
├── .gitignore
├── data/              # Raw and processed datasets
├── dashboards/        # Power BI (.pbix) files
└── docs/              # Supporting documentation, notes, references

📬 Contact

Feel free to open an issue or reach out with questions about the methodology or findings.
