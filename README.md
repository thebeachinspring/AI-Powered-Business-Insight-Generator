# AI-Powered Business Insight Generator  
*(US Superstore Dataset)*

## Overview
This project demonstrates how AI can **augment the work of a Data Analyst** by automatically converting monthly business performance data into **clear, executive-ready insights**.

The solution calculates core KPIs, detects trends and anomalies using explainable statistical methods, identifies key business drivers, and generates concise performance commentary suitable for senior stakeholders.

The focus is on **business value, explainability, and analyst productivity** rather than complex or opaque machine learning models.

---

## What the Notebook Does

1. Loads and prepares the US Superstore sales dataset
2. Aggregates data to a **monthly reporting grain**
3. Calculates core performance KPIs
4. Detects:
   - Month-over-month trends
   - Unusual movements (anomalies)
5. Identifies **key drivers** by Region and Category
6. Produces an **executive-style performance summary**
7. *(Optional)* Uses an LLM to generate AI-assisted insight commentary

---

## Core KPIs

- **Total Sales**
- **Total Profit**
- **Profit Margin (%)**
- **Order Volume**

Derived metrics:
- Month-over-Month % change
- Rolling behaviour via z-score anomaly detection
- Contribution analysis by Region and Category

---

## Trend & Anomaly Detection

To ensure transparency and professional suitability:

- Trends are identified using **month-over-month percentage change**
- Anomalies are flagged using a **z-score on MoM changes**
- Thresholds are intentionally simple and explainable:
  - Trend: ±5%
  - Anomaly: |z| > 2

This mirrors how analytics is commonly validated in real business environments.

---

## Insight Generation

The notebook produces:
- A **rule-based executive summary** (default, no API required)
- An **optional AI-generated summary** using a Large Language Model (LLM)

The LLM is provided with:
- KPI values
- Trend direction
- Anomaly flags
- Identified business drivers

This ensures the AI output remains factual, grounded, and auditable.

---

This is a demo only using open source data from Kaggle


