# NYC Taxi Fare Prediction project

## Author: Abd Ur Rehman

## Date: 10/07/2023

## Table of Content

- [Project Overview](#project-overview)
- [Results and Findings](#results-and-findings)
- [Recommendation](#recommendations)

### Project Overview

**Project Purpose:**

The core objective of this project is to combine a comprehensive Exploratory Data Analysis (EDA) with the development of a multiple linear regression model. The project's focus is on the NYC Taxi and Limousine Commission's dataset, with the intent to unlock actionable insights that can enhance service quality and fare predictions for the benefit of the New York City TLC.

**Model Performance:**

The multiple linear regression model's performance is noteworthy. It exhibits high accuracy on both the training and test datasets, indicating that the model is unbiased and avoids overfitting. In fact, the model's performance on the test dataset surpasses that of the training dataset, reflecting its strong generalization capabilities.

Key Model Metrics:

- **R-squared (R^2):** The test dataset shows an R^2 value of approximately 0.868, signifying that 86.8% of the variance in the `fare_amount` variable can be accounted for by the model. This underscores the model's excellent fit to the data.

- **Mean Absolute Error (MAE):** The test data's MAE is about 2.1337, indicating that the model's fare predictions are generally close to actual values.

- **Mean Squared Error (MSE):** The test dataset's MSE stands at 14.3264, reflecting favorable model performance with lower MSE values.

- **Root Mean Squared Error (RMSE):** The test dataset's RMSE is 3.7850, indicating a reasonable level of prediction error.

- **Residual Analysis:** Residuals are normally distributed around a mean of -0.015. This suggests that the model's errors are evenly distributed and unbiased.

In summary, this project successfully combines EDA and multiple linear regression to create an effective predictive model for taxi fare optimization. With strong model performance and accurate predictions, the potential for improving fare predictions and service quality is significant, enabling data-informed decision-making for the betterment of New Yorkers.

### Data Source

The dataset used in this project is secondary data obtained from Google. It includes NYC Taxi and Limousine Commission (New York City TLC).

### Tools

- Jupyter Notebook
- Python
- python libraries
  - pandas
  - numpy
  - matplotlib.pyplot
  - seaborn
  - from datetime import datetime
  - from datetime import date
  - from datetime import timedelta
  - from sklearn.preprocessing import StandardScaler
  - from sklearn.model_selection import train_test_split
  - sklearn.metrics
  - from sklearn.linear_model import LinearRegression
  - from sklearn.metrics import mean_absolute_error,r2_score,mean_squared_error

### Data Cleaning/Preparation

In the initial data preparation phase, we performed the following tasks:

1. Data loading and inspections.
2. Handling missing values.
3. Data cleaning and formatting.

### Hypothesis Test

In this project, we conduct a two-sample t-test to investigate potential differences in verified status column

- **$H_0$**: There is no difference in number of views between TikTok videos posted by verified accounts and TikTok videos posted by unverified accounts (any observed difference in the sample data is due to chance or sampling variability).

- **$H_A$**: There is a difference in number of views between TikTok videos posted by verified accounts and TikTok videos posted by unverified accounts (any observed difference in the sample data is due to an actual difference in the corresponding population means).

### Results and Findings

Based on the analysis of the dataset, the following key findings were observed:

- The p-value for the t-test (pvalue=2.6088823687177823e-120) is extremely small, indicating a high level of statistical significance.
- With a p-value much smaller than the significance level of 5%, we reject the null hypothesis.

These findings lead to the following conclusions:

- There is a statistically significant difference in the mean video view count between verified and unverified accounts on TikTok.
- The analysis reveals that videos from verified accounts tend to have a significantly different average view count compared to videos from unverified accounts.

This suggests potential fundamental behavioral differences between these two groups of TikTok accounts.

### Recommendations

Based on the observed statistically significant difference in average view counts between videos from verified and unverified accounts, it is recommended to explore the underlying factors contributing to this behavioral difference. Consider the following next steps:

- Investigate the root causes of this difference, such as whether unverified accounts tend to post clickbait content or if they are associated with view count manipulation through spam bots.
- Explore the creation of a regression model focused on the 'verified_status' variable. A regression model can provide insights into user behavior within the group of verified users.
- The regression model can help analyze and predict behaviors and characteristics associated with verified accounts, leading to a deeper understanding of the factors influencing user interactions and engagement on TikTok.

Continuing the analysis with these recommendations can provide valuable insights and inform strategies for content creators and platform administrators on TikTok.

### Limitations

I had to remove all Null values from data because they would have affected the accuracy of my conclusions from the Hypothesis testing.
