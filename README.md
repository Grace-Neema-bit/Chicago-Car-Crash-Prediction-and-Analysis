# Chicago-Traffic-Crash-Prediction-and-Analysis

## Project Overview

Traffic accidents are a major public safety concern in Chicago.
Understanding the conditions that lead to crashes resulting in injuries
can help city authorities design safer roads and implement preventative
safety measures.

This project builds a **machine learning classification model** to
predict whether a car crash will result in injuries based on
environmental and crash-related factors such as weather conditions,
visibility, and the number of vehicles involved.

The goal is to identify patterns associated with injury-causing crashes
and provide insights that can support better road safety decisions.

------------------------------------------------------------------------

## Business Understanding

### Problem Statement

Traffic accidents are a major concern in Chicago. Understanding the
conditions that lead to severe crashes can help the Vehicle Safety Board
and city authorities improve road safety.

This project aims to build a classification model that predicts whether
a crash will result in injuries. The insights generated from this model
can help identify high‑risk driving conditions and support preventative
measures to reduce injury-related accidents.

### Stakeholders

**Vehicle Safety Board** - Responsible for improving road safety - Can
use insights from the model to identify high-risk driving conditions -
Can implement safety programs and issue alerts during dangerous
conditions

**City of Chicago** - Responsible for transportation infrastructure and
traffic regulation - Can use insights to improve road design, traffic
policies, and emergency response planning

### Key Questions

1.  What environmental or crash-related factors contribute most to
    injury-causing crashes?
2.  Under what conditions are crashes most likely to result in injuries?
3.  Can we predict whether a crash will result in injuries based on
    environmental conditions?
4.  What patterns can be identified that help authorities reduce
    injury-related accidents?

------------------------------------------------------------------------

## Dataset

The dataset was obtained from **Kaggle** and contains records of Chicago
car crashes between **2019 and 2022**.

The dataset includes information such as:

-   Crash conditions
-   Environmental factors (temperature, windspeed, visibility)
-   Number of vehicles involved
-   Injury outcomes

This data enables analysis of how crash conditions influence whether an
accident results in injuries.

------------------------------------------------------------------------

## Project Workflow

The project follows the **standard data science workflow:**

1.  Business Understanding
2.  Data Understanding
3.  Data Preparation
4.  Modeling
5.  Evaluation
6.  Conclusion and Recommendations

------------------------------------------------------------------------

## Data Preparation

Several preprocessing steps were performed before training the models:

-   Cleaning missing values
-   Mapping injury values to numeric format
-   Creating a binary target variable (`injury_outcome`)
-   Feature engineering from crash dates
-   One-hot encoding categorical variables
-   Selecting relevant model features
-   Standardizing numerical variables using StandardScaler

Target Variable:

`injury_outcome` - 1 = crash resulted in injuries - 0 = crash resulted
in no injuries

------------------------------------------------------------------------

## Feature Selection

The following features were selected for modeling:

-   num_vehicles_in_crash
-   days_feelslike
-   days_temp
-   latitude
-   days_uvindex
-   cloudcover
-   visibility
-   windspeed

These features represent environmental conditions and crash
characteristics that may influence injury outcomes.

------------------------------------------------------------------------

## Models Used

Two machine learning models were used in this project:

### 1. Logistic Regression (Baseline Model)

Logistic Regression was used as the baseline classifier. It provides a
simple and interpretable model for binary classification problems.

### 2. Decision Tree Classifier

A Decision Tree model was used as the second model to capture more
complex relationships between variables.

------------------------------------------------------------------------

## Model Evaluation

Models were evaluated using:

-   Accuracy Score
-   Confusion Matrix
-   Classification Report (Precision, Recall, F1-score)

These metrics help measure how well the models predict injury outcomes.

------------------------------------------------------------------------

## Results

The performance of the models was compared using accuracy scores.

The comparison helps determine which model performs better in predicting
injury-related crashes.

------------------------------------------------------------------------

## Key Insights

The analysis helps identify:

-   Environmental conditions associated with higher injury risk
-   Crash patterns linked to severe accidents
-   Predictive indicators of injury-causing crashes

These insights can help authorities implement preventative measures to
improve road safety.

------------------------------------------------------------------------

## Future Improvements

The following improvements can further enhance the project:

-   Implement Ridge and Lasso regularization
-   Add more exploratory visualizations (boxplots, histograms,
    pairplots)
-   Experiment with ensemble models such as Random Forest or Gradient
    Boosting
-   Perform hyperparameter tuning
-   Deploy the model as a prediction tool