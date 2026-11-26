# B2B SaaS Customer Churn & Revenue Analysis

**Author:** Khushi Singhal

## 1. Project Overview

This project analyses customer churn, product engagement, and recurring revenue in a B2B SaaS business.

The objective is to identify customer behaviour patterns, understand differences between retained and churned customers, evaluate revenue contribution across subscription plans, and provide actionable recommendations to improve customer retention.

The analysis uses a simulated B2B SaaS customer dataset containing **50,000 records and 18 columns**.

## 2. Business Objectives

- Analyse overall customer churn and retention.
- Identify subscription plans with higher churn rates.
- Understand the relationship between product engagement and customer churn.
- Compare support activity between retained and churned customers.
- Evaluate Monthly Recurring Revenue (MRR) across subscription plans.
- Provide data-driven recommendations to improve customer retention.

## 3. Dataset Information

| Attribute | Details |
|---|---|
| Dataset Name | B2B SaaS Churn Dataset |
| Source | Hugging Face |
| Total Records | 50,000 |
| Total Columns | 18 |
| Data Type | Simulated customer subscription data |
| Business Domain | B2B SaaS Analytics |

**Dataset Links:**
- [Hugging Face Dataset](https://huggingface.co/datasets/MPSynthetics2026/b2b-saas-churn-dataset)
- [Download CSV](https://huggingface.co/datasets/MPSynthetics2026/b2b-saas-churn-dataset/resolve/main/MP_Synthetics_50000_Rows.csv)

The dataset contains customer details, subscription plans, revenue, payment status, product usage, support tickets, churn risk scores, and churn status.

> **Note:** This is a synthetic dataset. It does not represent actual customer records or the real business performance of VirtuBox Infotech.

## 4. Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data exploration, cleaning, calculations and analysis |
| Google Colab | Python development environment |
| Pandas | Data manipulation and analysis |
| Looker Studio | Interactive dashboard and visualization |
| ChatGPT | Occasional assistance with Python issues, visualization ideas and brainstorming |

## 5. Data Cleaning & Preparation

The following data preparation activities were performed:

1. Checked missing values and duplicate records.
2. Verified duplicate customer IDs.
3. Converted signup and last active dates into proper date formats.
4. Identified 59 records where the last active date was earlier than the signup date and flagged them for review.
5. Converted feature adoption percentages from text into numeric values.
6. Investigated potential MRR outliers using the Interquartile Range (IQR) method.
7. Retained 5,051 potential high-MRR outliers after investigation, as they belonged to the Enterprise subscription plan.
8. Calculated seat utilization using active seats and total seats allowed.

**Calculated Metric:**

Seat Utilization = (Active Seats Used / Total Seats Allowed) × 100

## 6. Key Business Findings

### Customer Churn

| Metric | Result |
|---|---:|
| Total Customers | 50,000 |
| Churned Customers | 916 |
| Retained Customers | 49,084 |
| Overall Churn Rate | 1.83% |

### Churn by Subscription Plan

| Plan | Churn Rate |
|---|---:|
| Starter | 2.28% |
| Pro | 1.16% |
| Enterprise | 1.13% |

**Insight:** Starter customers recorded the highest churn rate.

### Product Engagement

| Metric | Retained Customers | Churned Customers |
|---|---:|---:|
| Average Feature Adoption | 70.12% | 52.05% |
| Average Seat Utilization | 64.18% | 47.01% |

**Insight:** Churned customers showed lower average feature adoption and seat utilization than retained customers.

### Customer Support

| Customer Status | Average Support Tickets (Last 30 Days) |
|---|---:|
| Retained | 3.32 |
| Churned | 4.97 |

**Insight:** Churned customers had a higher average number of recent support tickets.

### Revenue Analysis

| Subscription Plan | Total MRR |
|---|---:|
| Enterprise | 25.21 Million |
| Pro | 5.39 Million |
| Starter | 2.67 Million |
| **Total** | **33.27 Million** |

**Major Discovery:** Enterprise customers represent approximately 10.1% of the customer base but contribute approximately 75.8% of total recurring revenue.

*MRR values are expressed in dataset currency units.*

## 7. Business Recommendations

Based on the analysis, three recommendations were proposed:

1. **Strengthen Enterprise Retention:** Conduct regular account reviews and provide personalized support to high-value customers to protect recurring revenue.
2. **Improve Product Engagement:** Strengthen customer onboarding, encourage feature adoption, and improve seat utilization.
3. **Improve Customer Support:** Monitor frequent support tickets, reduce resolution time, and follow up with customers regularly.

## 8. Interactive Looker Studio Dashboard

An interactive dashboard was developed to help management explore customer retention, product engagement, support activity, and revenue performance.

**[View Interactive Dashboard](https://datastudio.google.com/reporting/a88f4101-8099-43e7-ad25-18f888c99ccf)**

### Dashboard Highlights

- Executive KPI scorecards.
- Churn rate by subscription plan.
- Feature adoption by customer status.
- Seat utilization by customer status.
- Support tickets by customer status.
- MRR by subscription plan.
- Interactive filters for plan tier, industry, country, billing cycle, and company size.

## 9. Project Limitations

- The dataset is synthetic and may not represent actual SaaS customer behaviour.
- Historical monthly snapshots are unavailable, so actual monthly churn trends and revenue growth cannot be analysed.
- Specific customer churn reasons are not provided.
- The analysis identifies associations between customer engagement and churn but does not establish causation.

## 10. AI Usage Disclosure

ChatGPT was used occasionally for limited assistance with understanding complex dataset elements, Python coding issues, visualization suggestions, and brainstorming business recommendations.

Dataset exploration, data cleaning, analysis, calculations, interpretation, and final decisions were independently reviewed and completed by me.

## 11. Project Conclusion

This analysis highlights the importance of customer engagement and retention in a B2B SaaS business.

The findings show that churned customers have lower average feature adoption and seat utilization, while Enterprise customers contribute the majority of recurring revenue.

Focusing on Enterprise retention, better onboarding, and improved customer support could help protect recurring revenue and strengthen long-term customer relationships.

---

**Project completed by: Khushi Singhal**
Linkedin : https://www.linkedin.com/in/khushi-singhal-
Email- khushisinghal694@gmail.com
