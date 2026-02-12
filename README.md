## Interactive Dashboard

You can explore the interactive Tableau dashboard here:

[[View Interactive Dashboard on Tableau Public](https://public.tableau.com/authoring/MarketingCampaignAnalyticsDashboard1/MarketingCampaignAnalyticsDashboard#1)


# Marketing-Campaign-Analytics-Customer-Segmentation
 

Marketing Campaign Optimization, Segmentation & Response Modeling
Executive Summary

This project delivers a full analytics workflow to evaluate marketing campaign performance, segment customers, and build a baseline model to predict campaign response.
Using a dataset of 1,000 customer profiles, the analysis identifies channel and region differences, highlights actionable customer segments, and demonstrates how predictive modeling can support campaign targeting.

**Business Problem**

Marketing teams need to answer three key questions:

Which channels generate the highest conversion rates

Which customer groups are most responsive and valuable

Can we predict campaign response to optimize targeting and budget allocation

**Solution Approach**

The project follows a structured analytics pipeline:

**Data exploration and KPI definition**

Campaign performance analysis (channel, region)

Customer segmentation using RFM and clustering

Predictive modeling for response probability

Insights and business recommendations

**Dataset**

Synthetic dataset, 1,000 customers.

Target

campaign_response (0 = No, 1 = Yes)

Main variables

Demographics: age, income

Customer value: total_spent, purchase_frequency

Activity: last_purchase_days_ago (recency)

Marketing dimensions: channel, region

**Key Findings**
Campaign Performance

Overall conversion rate: 29.9%

Best channels: Social Media and Email

Channel performance varies by region, supporting a localized channel strategy.

Customer Segmentation (RFM + KMeans)

Customer base was segmented into:

High Value Loyal

Standard

At Risk / Inactive

**Key insight:**
Standard customers showed strong responsiveness, while At Risk customers represent reactivation potential.

Predictive Modeling (Baseline Logistic Regression)

A baseline logistic regression model was trained to predict response.

**Results:**

Accuracy: ~72%

AUC: ~0.50

**Interpretation:**
The baseline model performs close to random, indicating that richer behavioral variables are needed (engagement, previous campaign interactions, click-through behavior). This step serves as a benchmark and demonstrates the modeling framework.

**Visual Outputs**

The notebook includes:

Conversion rate by channel and region

Region × channel heatmap

Segment sizes and segment conversion rates

RFM radar chart for segment profiling

ROC curve and feature importance plot

**Business Recommendations**

Shift budget toward high-performing channels (Social Media, Email)

Personalize messaging by segment rather than using one general campaign

Run reactivation campaigns for At Risk customers

Collect engagement metrics to improve predictive targeting accuracy

**Tech Stack**

Python (pandas, numpy)

scikit-learn

matplotlib, seaborn

Google Colab
