# BoomBikes Demand Prediction Case Study
## Project Overview

BoomBikes, a US-based bike-sharing provider, has experienced a significant decline in revenue due to the COVID-19 pandemic. As the lockdown ends and the economy begins to recover, the company aims to anticipate the demand for shared bikes to optimize their business strategy and stand out from competitors.

This case study seeks to identify the key factors that influence bike-sharing demand in the American market. By developing a linear regression model, we will quantify the relationship between bike demand and various independent variables, such as temperature, humidity, weather conditions, and whether it is a working day.

## Objective
- Primary Goal: To develop a linear model that identifies the significant factors affecting bike demand.
- Secondary Goal: To provide actionable insights to BoomBikes' management, helping them refine their business strategy to meet post-pandemic demand levels and customer expectations.

## Dataset
-   Source: The dataset includes historical data on bike-sharing demand, including various features like temperature, humidity, weather conditions, working days, holidays, etc.

- Features:
    - temp: Normalized temperature in Celsius.
    - humidity: Normalized humidity levels.
    - weather: Categorical data representing weather conditions.
    - working_day: Binary indicator for whether the day is a working day or not.
    - holiday: Binary indicator for public holidays.
    - Target Variable:
        - demand: The count of total rentals.

## Methodology

1. Exploratory Data Analysis (EDA):

    -   Analyzed the distribution and relationships between features and demand.
    -   Identified potential outliers and data imbalances.

2. Data Preprocessing:

    -   Handled missing values, if any.
    -   Performed feature engineering to create new variables that may improve the model.
    -   Categorical variables were encoded, and numerical variables were scaled.

3. Model Development:

    -   Developed multiple linear regression models.
    -   Evaluated the models using metrics such as R-squared, Adjusted R-squared, and Root Mean Squared Error (RMSE).

4. Model Interpretation:

    -   Identified significant variables impacting bike demand.
    -   Interpreted the coefficients to understand the relationship between each feature and the demand.

5. Model Validation:

    -   Tested the model on unseen data to evaluate its predictive power.
    -   Compared the model's predictions with actual demand to assess accuracy.

## Results

-   The final model identified [holiday, temp, windspeed, Winter and Summer Season, September month, Year (2019), weathersit( Light Snow, Mist + Cloudy)] as the key factors influencing bike demand.
-   The model's accuracy, as measured by R-squared, was [83%], indicating a [strong/moderate] relationship between the features and bike demand.
-   Insights derived from the model can be used by BoomBikes' management to optimize their operations and marketing strategies.

## Conclusion

This case study provides a robust analysis of the factors influencing the demand for shared bikes in the post-pandemic scenario. The model developed can serve as a tool for BoomBikes to predict demand and adjust their strategies accordingly, ensuring they meet customer expectations and maximize profitability as the market recovers.

## Repository Structure

All files related to this project are located in the master branch of this repository:

-   day: The dataset used for the analysis.
-   BIKE+Sharing+Linear+Regression+Assignment.ipynb: The Jupyter notebook containing the analysis.
-   Data Dictionary-Readme.rtf: A rich text format file with the data dictionary.
-   Linear+Regression+Subjective+Questions.pdf: A PDF document with the conclusion of the analysis in a question-and-answer format.
-   README.md: Project overview and details (this file).

## Usage Instructions

1. Clone the Repository:

    - git clone https://github.com/HelloShibani/BoomBikes_BikeSharing_CASEStudy.git

2. Navigate to the project directory:
    -   cd BoomBikes-Demand-Prediction

3. Set up a Python environment with the necessary libraries. If you don't already have the required packages installed, you can install them using:
    -   pip install pandas numpy matplotlib seaborn scikit-learn

4. Run the Jupyter notebook:
    -   jupyter notebook

5. Open the BIKE+Sharing+Linear+Regression+Assignment.ipynb notebook to explore the analysis and model development.

## Future Work
-   Explore non-linear models to potentially improve prediction accuracy.
-   Investigate additional features such as economic indicators or social factors.
-   Test the model in different geographical locations to generalize its applicability.