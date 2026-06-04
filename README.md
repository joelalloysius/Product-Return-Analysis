## Product-Return-Analysis

**Executive Summary**

Aurowick, a luxury candle manufacturer, faced profitability losses driven by high product return rates. EDA showed that shipping and packaging damages were key contributors, with damaged packaging and product damage as the main return reasons. ABC Shipping accounted for the majority of deliveries (68%) but had the highest return rate (28%). Logistic regression confirmed ABC Shipping significantly increased return probability by approximately 9 percentage points compared to In-house delivery. A cost-benefit analysis indicated that shifting to greater In-house delivery could improve profitability by approximately 9%, despite a 10% increase in shipping costs.

**Business Problem**

Aurowick, a luxury candle manufacturer, is experiencing profitability challenges due to a high volume of product returns. The company suspects that logistical factors are contributing to return related losses. Management needs you to determine the key drivers of returns, assess the financial impact , and evaluate whether alternative strategies could reduce losses and improve overall profitability.

**Tools Used:** 

Excel | Python (Pandas, Matplotlib, Scikit-learn)

**Techniques Applied:** 

Data Cleaning & Transformation (Joins, Aggregations) | Exploratory Data Analysis (EDA) | Data Visualization | Logistic Regression | Cost-Benefit Analysis

**Methodology**

- Data was extracted from multiple internal system tables, including Orders, Returns, and Cost datasets. These tables were integrated through data joining techniques to create a single analysable dataset.
- Exploratory Data Analysis (EDA) was conducted to identify key patterns and relationships in return behaviour, supported by data visualisations.
- A logistic regression model was developed to quantify the impact of shipping methods on product return probability, providing statistical evidence of key drivers.
- Model performance was evaluated using cross-validation techniques to ensure reliability and generalisability.
- Finally, predictive analysis was used to estimate the impact of different shipping strategies and support data-driven business recommendations.

**Key Findings**

- Major reasons for Product returns include Damaged Product and Packaging
- ABC Shipping limited had the highest volume of deliveries (68%) but had a 28% return rate as opposed to In-house shipping ( 28% deliveries ; 17% return rate).
- Among returned products ABC shipping reported 47% of the returns due to damaged packaging and 31% due to product damage. In-house shipping method accounted for 58% of products returned due to damaged packaging however, no product damages
- ABC Shipping had a coefficient of 0.5051 with a statistically significant p-value (<0.05), indicating a positive association with product returns.
- Average marginal effects suggested that using ABC Shipping increased the probability of a return by approximately 9 percentage points.
- Switching to in-house shipping method would increase cost by 10% but also increase profitability by 9%

**Recommendations**

- Gradually move to In-house shipping methods and identify challenges
- Try and reduce hurdles among In-house drivers that cause damaged packaging and product returns
