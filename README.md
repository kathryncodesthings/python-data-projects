# Data Projects

These projects showcase my technical data skills and my ability to solve real business problems. Each one starts with a practical question from stakeholders, uses data analysis to test assumptions, and ends with clear, actionable insights.

Where relevant, I include links to the full analysis and code.

---

## HESA KFI Analysis

**Skills demonstrated:** stakeholder engagement; problem definition; Python (pandas, numpy, matplotlib); data cleaning and transformation; statistical analysis; outlier handling; data visualisation; communicating insights to non-technical audiences.

This project uses open data from HESA (the UK Higher Education Statistics Agency), which publishes standardised financial metrics for UK universities.

### Business question
While working at **University College London (UCL)**, I was asked to test an assumption within the Financial Planning team:

> Does an organisation’s annual surplus (or deficit) reliably predict its cash position?

Improving cash forecasting was a key organisational priority. The team had historically assumed that institutions with higher surpluses would also generate more cash by year-end. My task was to assess whether this assumption was supported by evidence.

(In a commercial setting, “surplus/deficit” is equivalent to profit/loss.)

### Approach

I downloaded ten years of publicly available financial data for UK universities and:

* Cleaned and standardised the dataset
* Identified and handled outliers
* Analysed the relationship between:
  - Surplus/(deficit) as a percentage of income
  - Net cash generated from operations as a percentage of income
* Visualised the results to support clear communication with stakeholders

![Scatterplot of Net cash vs. Surplus/deficit for UK HEIs, 2015-2024](https://github.com/kathryncodesthings/python-data-projects/blob/main/HESA_data_scatterplot.png "Scatterplot of Net cash vs. Surplus/deficit for UK HEIs, 2015-2024")

### Juptyer Notebook
The complete code I produced is here: [HESA KFI Analysis Python code](https://github.com/kathryncodesthings/python-data-projects/blob/main/HESA%20data%20analysis.ipynb)

### Conclusions
To quantify the strength of the relationship, I calculated R², which measures how much of the variation in one variable can be explained by another.
* An R² of 1.0 would indicate a perfect relationship
* An R² of 0.35 would suggest that around 35% of the variation in cash could be explained by surplus

In this analysis, R² was **0.07**. 

This means that only 7% of the variation in cash generation can be statistically linked to surplus, making surplus a very weak predictor of cash position.

In practice, this is because cash levels are driven by many other factors, such as:
* Timing of cash receipts and payments
* Capital investment decisions
* Financing and borrowing

### Impact
To communicate the results, I used a clear scatterplot alongside a plain-English explanation of the statistics. This made the lack of a consistent relationship immediately visible to non-technical stakeholders.

Following the presentation:
* The Financial Planning team revised their cash-forecasting approach
* Surplus was no longer used as a proxy for cash performance

This project demonstrates my ability to challenge assumptions with data and translate statistical results into practical business decisions.

### Possible improvemnts
#### Segment the data
This analysis uses sector-wide data covering over 200 universities, which makes it highly relevant and comparable. However, UCL is significantly larger and more complex than many institutions in the dataset.

A potential extension would be to:
* Segment the data to include only organisations with similar size and income profiles
* Test whether the relationship strengthens within more comparable peer groups.

