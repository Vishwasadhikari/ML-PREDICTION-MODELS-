# Energy Consumption Prediction and Classification Using Machine Learning

## Overview

This project explores household energy consumption data and applies machine learning techniques to understand and predict energy usage patterns. The goal was not only to predict appliance energy consumption using regression but also to transform the problem into a classification task and compare the performance of multiple machine learning algorithms.

The project follows a complete machine learning workflow, starting from data preprocessing and exploratory analysis to model building, evaluation, and comparison.

---

## Dataset

The dataset contains information related to household energy consumption, indoor environmental conditions, and weather measurements collected over time.

Some of the key features include:

* Appliance energy consumption
* Indoor temperatures
* Humidity levels
* Weather-related measurements
* Time-based information

### Regression Target

The regression task focuses on predicting:

**Appliances** – the amount of energy consumed by household appliances.

### Classification Target

Since the dataset does not include a predefined classification target, a new binary target variable was created:

* High Usage (1) – energy consumption above the median value
* Low Usage (0) – energy consumption at or below the median value

This allowed the same dataset to be used for both regression and classification tasks.

---

## Data Preprocessing

Several preprocessing steps were performed before training the models:

### Data Cleaning

* Checked for missing values
* Checked for duplicate records
* Removed duplicate rows where necessary

### Feature Engineering

The original date column was converted into a datetime format and additional features were extracted, including:

* Month
* Day
* Hour
* Weekday

The original date column was then removed since the extracted features captured the relevant information.

### Feature Scaling

Standardization was applied using StandardScaler to ensure that numerical features were on a similar scale before training the models.

---

## Exploratory Data Analysis

Exploratory analysis was carried out to better understand the dataset and identify relationships between variables.

Visualizations included:

* Correlation heatmap
* Distribution of appliance energy consumption
* Actual vs predicted plots
* Residual analysis
* Model performance comparison charts

These visualizations helped identify important patterns and relationships within the data.

---

## Regression Modeling

### Linear Regression

Linear Regression was used to predict appliance energy consumption.

The model was evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

Additional visualizations such as Actual vs Predicted and Residual Plots were used to assess model performance and prediction quality.

---

## Classification Modeling

After creating the binary target variable, several classification algorithms were trained and compared.

### Models Used

#### Logistic Regression

Used as a baseline classification model to distinguish between high and low energy usage.

#### Decision Tree

Implemented to capture nonlinear relationships and decision rules within the data.

#### Random Forest

An ensemble-based model that combines multiple decision trees to improve prediction performance.

#### Support Vector Machine (SVM)

Used to classify energy consumption patterns by finding the optimal decision boundary.

#### Naive Bayes

A probabilistic model based on Bayes' theorem that assumes feature independence.

#### K-Nearest Neighbors (KNN)

A distance-based algorithm that classifies observations using their nearest neighbors.

#### AdaBoost

A boosting algorithm that combines multiple weak learners into a stronger predictive model.

#### XGBoost

A gradient boosting algorithm known for its efficiency and strong predictive performance.

---

## Model Evaluation

### Regression Evaluation

The Linear Regression model was evaluated using:

* MAE
* RMSE
* R² Score

### Classification Evaluation

Each classification model was evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

This allowed a detailed comparison of model performance across different algorithms.

---

## Results

The project demonstrates how different machine learning models perform on the same dataset when solving both regression and classification problems.

The comparison highlights:

* Differences in predictive performance across models
* Trade-offs between simplicity and accuracy
* The effectiveness of ensemble methods such as Random Forest, AdaBoost, and XGBoost

Performance comparison graphs were created to visualize and compare results across all models.

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost

---

## Project Structure

```text
Energy-Consumption-ML-Project/

├── KAG_energydata_complete.csv
├── Energy_Consumption_Analysis.ipynb
├── README.md
└── requirements.txt
```

---

## What I Learned

Working on this project helped strengthen my understanding of:

* Data preprocessing techniques
* Feature engineering from datetime data
* Exploratory data analysis
* Regression modeling
* Classification modeling
* Model evaluation and comparison
* Visualization of machine learning results

It also provided practical experience in comparing multiple machine learning algorithms on the same dataset and understanding their strengths and limitations.

---

## Future Improvements

Potential improvements for future work include:

* Hyperparameter tuning
* Cross-validation
* Feature selection techniques
* Time series forecasting approaches
* Deep learning models for energy prediction
* Advanced ensemble methods

---

