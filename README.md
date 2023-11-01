# NYC Taxi Fare Prediction project

## Author: Abd Ur Rehman

## Date: 10/07/2023

## Table of Content

- [Project Overview](#project-overview)
- [Results and Conclusion](#results-and-conclusions)
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
4. Convert type of columns.

#### EDA(Exploratory Data Analysis )

We used a variety of techniques to understand our dataset better including but not limited to:

1. Descriptive statistics for each variable.
2. Visualizations such as histograms, box plots, scatterplots etc.
3. Correlation matrix heatmap.
4. Pair plotting.
5. Univariate analysis using distributions.
6. outltiers handling
7. IQR methoed to remove Outliers
8. Missing value methodology (Imputation)
9. Feature selection by correlation with target variable.

### Model Building

In this phase of the project, we focused on constructing a multiple linear regression model to predict taxi fares using the dataset provided by the NYC Taxi and Limousine Commission (New York City TLC). The model building process involved the following key steps:

1. Data Preprocessing
2. Model Selection
3. Model Training
4. Model Evaluation
5. Interpretation
6. Residual Analysis
The model building process was thorough, and the results are outlined in the earlier section, demonstrating the model's effectiveness in predicting taxi fares. It paves the way for data-driven decisions and service quality improvements for the benefit of New Yorkers.

### Results and Conclusions

**Results:**

After a comprehensive analysis of the NYC Taxi and Limousine Commission's dataset and the construction of a multiple linear regression model, the following key results were observed:

- The R-squared (R^2) value for the test dataset is approximately 0.868, indicating that 86.8% of the variance in the `fare_amount` variable is explained by the model.
- The Mean Absolute Error (MAE) for the test data is around 2.1337, suggesting that, on average, the model's fare predictions closely match actual values.
- The Mean Squared Error (MSE) for the test dataset is 14.3264, indicating lower prediction errors.
- The Root Mean Squared Error (RMSE) for the test dataset is 3.7850, representing a reasonable level of prediction error.

**Conclusions:**

Based on the results and analysis, the following conclusions can be drawn:

1. **Model Effectiveness:** The multiple linear regression model built for predicting taxi fares demonstrates strong performance. The high R-squared value and low prediction errors indicate that the model effectively captures the relationships between various factors and fare amounts.

2. **Generalization Capability:** The model performs well on both the training and test datasets, which suggests that it avoids overfitting and generalizes effectively to unseen data.

3. **Actionable Insights:** The model can be used as a valuable tool for optimizing fare predictions and improving service quality for the New York City TLC. It offers actionable information for data-driven decision-making, which can benefit the residents of New York City.

Overall, this project successfully combines exploratory data analysis (EDA) and multiple linear regression to create an accurate predictive model for taxi fare optimization, with the potential to enhance service quality and pricing decisions for the New York City TLC.

### Recommendations

- The New York City Taxi and Limousine commission can use these findings to create an app that allows users (TLC riders) to see the estimated fare before their ride begins.
- The model provides a generally strong and reliable fare prediction that can be used in downstream modeling efforts.

### Limitations

The approach to handling outliers using the IQR method may impact the representation of extreme fare amounts.