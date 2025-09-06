# California Housing Price Prediction Project

## Overview
This project focuses on predicting housing prices in California using a dataset from scikit-learn. The goal is to build a machine learning model that can accurately estimate house prices based on various features such as median income, house age, average rooms, and location coordinates.

## Dataset
The dataset used is the `fetch_california_housing` dataset from scikit-learn, which contains the following features:
- MedInc: Median income in block group
- HouseAge: Median house age in block group
- AveRooms: Average number of rooms per household
- AveBedrms: Average number of bedrooms per household
- Population: Block group population
- AveOccup: Average number of household members
- Latitude: Block group latitude
- Longitude: Block group longitude
- Target variable: price (median house value)

## Project Structure
The project is organized in a Jupyter notebook (`california_housing.ipynb`) with the following steps:

1. **Import Libraries**: Necessary libraries including numpy, pandas, matplotlib, seaborn, and scikit-learn components are imported.

2. **Load Data**: The California housing dataset is loaded and converted into a pandas DataFrame for easier manipulation.

3. **Data Exploration**: Basic exploration of the dataset including viewing the first few rows and checking correlations between features.

4. **Data Visualization**: A heatmap is created to visualize correlations between different features in the dataset.

5. **Data Preprocessing**: 
   - Independent and dependent variables are separated
   - Data is standardized using StandardScaler
   - Data is split into training and testing sets (80/20 split)

6. **Model Training**: A Linear Regression model is trained on the standardized training data.

7. **Model Evaluation**: Predictions are made on the test set, and the model's performance is evaluated using R² score.

## Results
The initial Linear Regression model achieved an R² score of **0.59** (59% accuracy) on the test set. While this provides a baseline performance, there is significant room for improvement.

## Next Steps
I plan to improve the model's performance by:
- Trying more sophisticated regression models
- Performing feature engineering to create more informative features
- Tuning hyperparameters of the models
- Exploring different data preprocessing techniques
- Potentially using neural networks for this regression task

## Requirements
To run this project, you'll need:
- Python 3.x
- Jupyter Notebook
- Libraries: numpy, pandas, matplotlib, seaborn, scikit-learn

## Author
Salaheddine Boumazough
