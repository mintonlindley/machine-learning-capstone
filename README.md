# 🏡 Airbnb Listing Price Classification

## Overview

This project applies the machine learning lifecycle to predict whether an Airbnb listing is **high-priced** or **low-priced** based on listing characteristics. The project was completed as part of the **Break Through Tech AI Fellowship** and demonstrates the end-to-end process of data exploration, preprocessing, model development, evaluation, and comparison between traditional machine learning and deep learning approaches.

## Problem Statement

Pricing is one of the most important factors for Airbnb hosts and travelers. This project aims to build a binary classification model that predicts whether a listing belongs to a high-price category using property and listing features.

## Dataset

The project uses an Airbnb listings dataset containing information about:

- Property characteristics
- Number of bedrooms
- Accommodation capacity
- Availability throughout the year
- Neighborhood information
- Pricing category (target variable)

**Target Variable**
- `price_category`
  - High-priced
  - Low-priced

The dataset can be downloaded here:
https://www.dropbox.com/scl/fi/udov4ctievf0140smhzk0/airbnbListingsData.csv?rlkey=mtjhgr2sc11gqzs4j3r4tmfp5&st=e5ha11ds&dl=0

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras

## Machine Learning Workflow

### 1. Exploratory Data Analysis (EDA)

Performed exploratory analysis to:

- Examine class distribution
- Identify missing values
- Explore feature relationships
- Detect potential data quality issues

### 2. Data Preparation

Data preprocessing included:

- Removing rows with missing values
- Selecting relevant predictive features
- One-hot encoding categorical variables
- Feature scaling for the neural network
- Stratified train-test split to preserve class balance

## Models

### Logistic Regression

A Logistic Regression classifier was trained as the baseline model.

Model tuning included:

- GridSearchCV
- Hyperparameter optimization
- Cross-validation

### Neural Network

A feedforward neural network was implemented using TensorFlow/Keras with:

- Input layer
- Two hidden layers (32 and 16 neurons)
- ReLU activation
- Sigmoid output layer
- Binary Cross-Entropy loss
- Stochastic Gradient Descent (SGD)

## Results

| Model | Accuracy | F1 Score |
|--------|----------|----------|
| Logistic Regression | **80.42%** | **0.519** |
| Neural Network | **80.88%** | **0.522** |

The neural network achieved slightly better performance than logistic regression, though the improvement was minimal. This demonstrates that for this dataset, a simpler linear model performed nearly as well as a more complex deep learning model.

## Key Takeaways

- Applied the complete machine learning lifecycle from problem definition to model evaluation.
- Compared traditional machine learning with deep learning approaches.
- Learned how feature engineering and preprocessing significantly impact model performance.
- Evaluated models using both Accuracy and F1 Score to account for class imbalance.
- Considered ethical implications of predictive models in housing-related datasets.

## Future Improvements

- Experiment with Random Forests and Gradient Boosting models
- Perform additional feature engineering using text-based listing descriptions
- Address class imbalance using oversampling techniques (SMOTE)
- Improve neural network performance through hyperparameter tuning
- Deploy the model as a simple web application

## Author

**Lindley Minton**

Honors Student, Florida State University  
B.S. Cyber Criminology (Expected May 2027)
