# Data Projects

As well as demonstrating a technical skills, a key goal of each of these projects was to solve real work problems. 

Each project contains a link to the full analysis, and where relevant, code.

---

## HESA KFI Analysis

**Skills used:** working with stakeholders to understand a business problem; Python (numpy, pandas, matplotlib); cleaning data; finding and handling outliers; data visualisation; presenting results to stakeholders.

This project takes open data from HESA, the UK Higher Education Statistics Agency.

I was asked to review whether there is a significant correlation between two of the Key Financial Indicators collected by HESA:
* Surplus/(deficit) as a % of total income
* Net cash inflow from operating activities as a % of total income

One of my employer's projects was to improve cash forecasting, and the Financial Planning Team requested that I look into whether surplus/deficit % was correlated with net cash inflow, and whether the budgeted surplus/deficit % could be used to forecast net cash inflow. (NB: In a for-profit company, the surplus/deficit would be the profit/loss).

I downloaded ten years of data on Key Financial Indicators for UK Higher Education Institutions and cleaned, transformed, analysed and visualised the data, and presented my conclusions.

### image here

### link to code

### Conclusions
Calculating R² tells us how much of the difference in net cash positions across universities is associated with differences in surplus. For example, an R² of 0.35 would mean about 35% of the variation in net cash can be statistically linked to surplus.

In this case, R² was **0.07**, which means 7% of the variation in net cash can be statistically linked to surplus. This makes surplus a poor predictor of net cash. There are many other influences on cash, such as timing of payments, exchange rates, investment decisions, etc.

After presenting my findings to the Financial Planning team, they could revise their approach to forecasting net cash accordingly, and discount using surplus as a predictor of net cash.

