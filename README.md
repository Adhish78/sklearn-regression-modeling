# Steel Industry Energy Consumption Analysis and Prediction Using Regression Models

## Overview

This project focuses on the analysis and prediction of energy consumption in the steel industry using various regression models. The dataset is sourced from the UCI Machine Learning Repository and includes a variety of features related to energy usage, including CO2 levels, power factors, and load types.

## Table of Contents
- [Dataset Description](#dataset-description)
- [Usage](#usage)
- [Analysis and Models](#analysis-and-models)
- [Results](#results)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## Dataset Description

| Variable Name                                 | Type       | Description                    | Units |
|-----------------------------------------------|------------|--------------------------------|-------|
| date                                          | Date       |                                |       |
| Usage_kWh                                     | Continuous | Industry Energy Consumption    | kWh   |
| Lagging_Current_Reactive.Power_kVarh          | Continuous |                                | kVarh |
| Leading_Current_Reactive_Power_kVarh          | Continuous |                                | kVarh |
| CO2(tCO2)                                     | Continuous |                                | ppm   |
| Lagging_Current_Power_Factor                  | Continuous |                                | %     |
| Leading_Current_Power_Factor                  | Continuous |                                | %     |
| NSM (Number of Seconds from Midnight)         | Integer    |                                | s     |
| WeekStatus                                    | Categorical| Weekend (0) or a Weekday (1)   |       |
| Day_of_week                                   | Categorical| Sunday, Monday, ..., Saturday  |       |
| Load_Type                                     | Categorical| Light Load, Medium Load, Maximum Load |       |


## Usage

1. Ensure the dataset (`Steel_industry_data.csv`) is placed in the project directory.

2. Run the Jupyter Notebook.

3. Follow the steps in the notebook to load, preprocess, analyze, and model the data.

## Analysis and Models

The project includes the following steps:

1. **Data Loading and Inspection**: Load and inspect the dataset for initial understanding.
2. **Data Preprocessing**: Convert date columns, handle missing values, and transform categorical variables.
3. **Exploratory Data Analysis (EDA)**:
    - Univariate Analysis: Distribution of continuous variables.
    - Bivariate Analysis: Relationship between continuous variables and Load type.
    - Time Series Analysis: Trends over time.
    - Correlation Analysis: Heatmap of the correlation matrix.
    - Energy usage analysis by WeekStatus and Day of week.
4. **Statistical Analysis**:
    - Hypothesis testing on energy consumption between weekdays and weekends.
    - Regression analysis to determine the impact of CO2 levels on energy consumption.
5. **Regression Modeling**: Build and evaluate multiple regression models, including Linear Regression, Decision Tree, Random Forest, Gradient Boosting, and SVR.

## Results

The evaluation metrics for each regression model are calculated and compared. Metrics include Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² Score. Plots of actual vs. predicted values and residuals are provided for visual analysis.

## Acknowledgments

This dataset is provided by:
V E, Sathishkumar, Shin, Changsun, and Cho, Yongyun. (2023). Steel Industry Energy Consumption. UCI Machine Learning Repository. https://doi.org/10.24432/C52G8C.

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/Adhish78/sklearn-regression-modeling/blob/main/LICENSE) file for details.
