# California Housing Price Prediction: Comparative Analysis

## Description
This project implements and compares multiple machine learning regression models to predict median house values in California districts. Using the California Housing dataset, the study evaluates the effectiveness of linear models versus ensemble-based methods in capturing complex spatial and economic relationships.

## Dataset
The project utilizes the California Housing dataset fetched from Scikit-Learn. The dataset includes 20,640 samples with 8 features:
* MedInc: Median income in block group
* HouseAge: Median house age in block group
* AveRooms: Average number of rooms per household
* AveBedrms: Average number of bedrooms per household
* Population: Block group population
* AveOccup: Average number of household members
* Latitude and Longitude: District location coordinates.

## Methodology
The following preprocessing and modeling steps were implemented:
1. Data Visualization: Correlation heatmaps were used to identify relationships between features.
2. Feature Scaling: Standardized features using StandardScaler to ensure uniform contribution to model training.
3. Model Training: Comparison of three distinct algorithms:
   * Linear Regression (Baseline).
   * Random Forest Regressor (Ensemble learning).
   * Gradient Boosting Regressor (Boosting technique).

## Model Performance
The models were evaluated using the R-squared ($R^2$) metric on the test set.

| Model | Hyperparameters | R2 Score |
| :--- | :--- | :--- |
| Linear Regression | Default | 0.594 |
| Random Forest | n_estimators=400, random_state=0 | 0.801 |
| Gradient Boosting | n_estimators=400, learning_rate=0.1 | 0.821 |

## Installation
Ensure you have Python installed, then install the required dependencies:
```bash
pip install -r requirements.txt
