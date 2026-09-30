# 📊 PULSE Analytics — SaaS Product Analytics & User Behavior Dashboard

> End-to-end SaaS product analytics project built with Python, Pandas, SQL concepts, and Power BI to analyze user acquisition, engagement, conversion, recurring revenue, churn, and cohort retention.

---

## 🚀 Project Overview

**PULSE Analytics** is an end-to-end SaaS product analytics solution designed to understand the complete customer lifecycle:

**Acquisition → Engagement → Conversion → Monetization → Retention**

The project transforms user, subscription, and product-event data into analysis-ready datasets and an interactive **Power BI dashboard**.

The final dashboard provides four analytical views:

- Executive Overview
- Growth & Acquisition
- Revenue & Monetization
- Retention & Engagement

The goal was not simply to visualize data, but to build a business-oriented analytics product that answers practical SaaS questions around growth, revenue, customer behavior, and retention.

---

## 🎯 Business Problem

SaaS businesses generate data across multiple parts of the customer lifecycle.

User acquisition data shows **where users come from**, product events show **how they engage**, subscription data shows **how they monetize**, while churn and retention analysis shows **whether users continue creating value**.

Looking at these datasets separately makes it difficult to answer questions such as:

- How active is the user base?
- Which acquisition channels generate the most users?
- How many users become engaged?
- How many users convert to paid subscriptions?
- How is MRR changing over time?
- Which subscription plans contribute the most revenue?
- What is the average revenue per paid user?
- How much churn is occurring?
- How does user activity change across signup cohorts?

PULSE Analytics brings these questions together into a single analytical solution.

---

## 📌 Key Metrics

| Metric | Value |
|---|---:|
| Total Users | 2,000 |
| User Events | 33,987 |
| Paid Users | 988 |
| Paid Conversion | 49.4% |
| Overall Churn | 28.8% |
| Latest MRR Snapshot | ~₹2M |
| Latest ARPU | ~₹3,274 |
| Active Subscribers | 1,429 |
| Avg. Session Duration | 15.5 min |

---

## 📂 Dataset

The project uses three core source datasets:

### Users

Contains one record per user.

**Key fields:**

- `user_id`
- `signup_date`
- `country`
- `acquisition_channel`

### Subscriptions

Contains subscription information.

**Key fields:**

- `user_id`
- `plan_type`
- `start_date`
- `monthly_price`
- `end_date`

Plans:

- Free — ₹0
- Basic — ₹2,000
- Pro — ₹5,000

### Events

Contains product interaction data.

**Key fields:**

- `user_id`
- `event_date`
- `event_type`
- `session_duration`

Event types include:

- Login
- Feature Use
- Upgrade
- Cancel

---

## 🛠️ Data Preparation

Python and Pandas were used to transform the source data into analysis-ready datasets.

### Generated analytical datasets

```text
users.csv
subscriptions.csv
events.csv
user_360.csv
monthly_metrics.csv
funnel_metrics.csv
cohort_retention.csv