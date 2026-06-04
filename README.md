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
  
![Figure 1](Tables%20and%20plots/Figure%201.png)

- ABC Shipping limited had the highest volume of deliveries (68%) but had a 28% return rate as opposed to In-house shipping ( 28% deliveries ; 17% return rate).

![Figure 2](Tables%20and%20plots/Figure%202.png)

- Among returned products ABC shipping reported 47% of the returns due to damaged packaging and 31% due to product damage. In-house shipping method accounted for 58% of products returned due to damaged packaging however, no product damages

![Figure 3](Tables%20and%20plots/Figure%203.png)

- ABC Shipping had a coefficient of 0.5051 with a statistically significant p-value (<0.05), indicating a positive association with product returns.

![Figure 4](Tables%20and%20plots/Figure%205.png)
  
- Average marginal effects suggested that using ABC Shipping increased the probability of a return by approximately 9 percentage points.

![Figure 5](Tables%20and%20plots/Figure%206.png)

- Switching to in-house shipping method would increase cost by 10% but also increase profitability by 9%

![Figure 6](Tables%20and%20plots/Figure%207.png)

**Recommendations**

- **Gradually move towards in-house shipping** , while monitoring cost, delivery time, and return rates to ensure a controlled transition from third-party providers.
- **Implement driver training and handling standards**, focusing on proper packaging care, loading/unloading procedures, and damage-prevention protocols to reduce returns caused by mishandling.
- **Introduce performance tracking and feedback systems** for in-house deliveries, including return reason analysis, driver-level KPIs, and corrective actions to continuously reduce packaging and product damage.
