# Marketing Budget Optimization using Linear Regression

## Project Overview

This project focuses on analyzing marketing spend data and optimizing marketing budget allocation using Multiple Linear Regression.

The company invests in multiple marketing channels such as:

- TV Advertising
- Radio Advertising
- Social Media Advertising
- Search Ads
- Influencer Marketing

The objective of the project is to understand which marketing channels contribute most effectively to sales revenue and provide data-driven budget recommendations.

The project includes:

- Data Cleaning
- Exploratory Data Analysis
- Outlier Analysis
- Correlation Analysis
- Multiple Linear Regression Modeling
- Model Evaluation
- Channel Effectiveness Analysis
- Budget Optimization Recommendations


# Business Problem

Marketing budgets are limited, and companies need to allocate resources efficiently across different advertising channels.

The business wants to answer the following questions:

- Which marketing channels contribute most to sales revenue?
- Which channels generate the best return?
- Which channels are less effective?
- How should future marketing budgets be allocated?

By using regression analysis, the company can make data-driven decisions instead of relying on assumptions.


# Dataset Description

The dataset contains marketing campaign data and sales revenue information.

Each row represents one marketing campaign or observation period.

## Dataset Columns

| Column Name | Description |
|---|---|
| CampaignID | Unique campaign identifier |
| Month | Campaign month |
| Region | Campaign region |
| TV_Spend | Amount spent on TV advertising |
| Radio_Spend | Amount spent on radio advertising |
| SocialMedia_Spend | Amount spent on social media marketing |
| SearchAds_Spend | Amount spent on search ads |
| Influencer_Spend | Amount spent on influencer marketing |
| Sales_Revenue | Total sales revenue generated |


# Business Understanding

## Why Marketing Budget Optimization is Important

Marketing budgets are expensive, and businesses must ensure that spending generates maximum returns.

Budget optimization helps:
- improve return on investment
- reduce inefficient spending
- increase sales revenue
- improve campaign effectiveness

## Independent Variables

The following columns are independent variables (input features):

- TV_Spend
- Radio_Spend
- SocialMedia_Spend
- SearchAds_Spend
- Influencer_Spend

## Dependent Variable

- Sales_Revenue

## Why This is a Regression Problem

Sales_Revenue is a continuous numeric value, so this project uses regression analysis.

## Why Regression is Useful

Regression helps estimate how changes in marketing spend influence sales revenue.

This helps businesses:
- forecast revenue
- optimize budgets
- compare channel effectiveness
- improve decision-making


# Data Cleaning Summary

The dataset was checked for:
- missing values
- duplicates
- incorrect data types
- outliers

## Cleaning Steps Performed

- Removed duplicate records
- Filled missing values in SocialMedia_Spend using the median
- Verified numeric columns
- Performed summary statistics analysis
- Identified outliers using boxplots

The dataset was found to be relatively clean and suitable for regression modeling.


# Exploratory Data Analysis (EDA)

EDA was performed to understand:
- distribution of marketing spend
- distribution of sales revenue
- relationships between channels and sales
- channel effectiveness
- outlier behavior


# Key EDA Insights

## Distribution Analysis

- TV_Spend contains a few extremely high campaigns.
- Influencer_Spend has several outliers.
- Sales_Revenue follows an approximately normal distribution.

## Correlation Analysis

The correlation heatmap showed:

| Channel | Correlation with Sales |
|---|---|
| SearchAds_Spend | Strongest Positive Correlation |
| TV_Spend | Strong Positive Correlation |
| Radio_Spend | Strong Positive Correlation |
| SocialMedia_Spend | Moderate Positive Correlation |
| Influencer_Spend | Weak Positive Correlation |

## Scatter Plot Analysis

- Search Ads showed the clearest positive relationship with sales.
- TV and Radio spending also strongly influenced revenue.
- Influencer marketing showed weaker and less consistent impact.


# Regression Model Summary

A Multiple Linear Regression model was built using marketing spend variables as input features and Sales_Revenue as the target variable.

## Modeling Steps

- Split dataset into training and testing sets
- Trained Linear Regression model
- Predicted sales revenue on test data
- Evaluated model performance


# Model Evaluation Results

The model was evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

## Interpretation

- Lower MAE and RMSE indicate smaller prediction errors.
- A higher R² Score indicates the model explains a large portion of sales variation.

The Actual vs Predicted plot showed that predictions closely followed actual sales values, indicating good model performance.


# Coefficient Interpretation

The regression coefficients showed the estimated impact of each marketing channel on sales revenue.

## Key Findings

| Channel | Impact |
|---|---|
| Radio_Spend | Highest positive coefficient |
| SearchAds_Spend | Strong positive impact |
| TV_Spend | Strong positive impact |
| SocialMedia_Spend | Moderate impact |
| Influencer_Spend | Weakest impact |

## Business Interpretation

- Increasing Radio and Search Ads budgets is likely to improve sales significantly.
- TV advertising remains an important contributor.
- Social media provides moderate support.
- Influencer marketing appears less effective compared to other channels.


# Channel Effectiveness Analysis

## Most Effective Channels

- Search Ads
- Radio Advertising
- TV Advertising

## Moderately Effective Channel

- Social Media Advertising

## Least Effective Channel

- Influencer Marketing


# Budget Recommendations

## Increase Budget

### Search Ads
Search advertising showed the strongest relationship with sales revenue and should receive increased investment.

### Radio Advertising
Radio campaigns demonstrated strong regression coefficients and should receive additional funding.

### TV Advertising
TV advertising continues to perform well and should remain a major budget component.


## Maintain Moderate Investment

### Social Media Advertising
Social media campaigns showed moderate effectiveness and should continue with optimized targeting strategies.


## Reduce or Reevaluate Budget

### Influencer Marketing
Influencer campaigns showed weak correlation and low regression impact. The company should carefully evaluate influencer ROI before increasing investment.


# Additional Recommendations

- Monitor campaign ROI regularly
- Collect more historical campaign data
- Include customer-level conversion data in future analysis
- Consider seasonality and regional differences
- Test channel combinations using A/B testing


# Business Risks

Before changing budgets, the company should consider:

- Correlation does not always imply causation
- Market conditions may change
- Customer behavior evolves over time
- Brand awareness effects may not appear immediately

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

# Conclusion

This project successfully applied Multiple Linear Regression to analyze marketing budget effectiveness and predict sales revenue.
The analysis showed that:
Search Ads
Radio Advertising
TV Advertising
are the strongest contributors to revenue generation.
The project demonstrates how regression analysis can support strategic marketing budget decisions and improve business performance through data-driven insights.
