# Global-Coffee-Health-Dataset-Analysis-and-BMI-Prediction

### Project Overview

This repository contains a Notebook (Global_Coffee_Health_Analysis_and_ML.ipynb) that explores the 'Global Coffee Health Dataset' to understand the relationships between coffee consumption, lifestyle factors, and health indicators. The project also develops and evaluates various machine learning models to predict Body Mass Index (BMI) based on other health and lifestyle features.

### Data Source

The dataset used in this project is the 'Global Coffee Health Dataset,' which includes synthetic data on 10,000 individuals across various countries. It features columns such as Age, Gender, Country, Coffee Intake (cups/day), Caffeine (mg), Sleep Hours, Sleep Quality, BMI, Heart Rate, Stress Level, Physical Activity Hours, Health Issues, Occupation, Smoking, and Alcohol Consumption.

### Technologies Used

  - Google Colab
  - Python
  - pandas (for data manipulation)
  - matplotlib, seaborn (for visualizations)
  - numpy (for numerical operations)
  - zipfile (for extracting data)
  - scikit-learn (for model selection, preprocessing, and machine learning models)

### Methodology

  1. **Data Loading & Initial Inspection:** Loading the dataset and performing initial checks (df.head(), df.info(), df.shape).
  2. **Data Sanity Checks:** Identifying missing values, duplicates, and unique categorical values.
  3. **Exploratory Data Analysis (EDA)**: Visualizing distributions (histograms, box plots), relationships (scatter plots), and correlations (heatmap).
  4. **Data Preprocessing:** Handling missing values in 'Health_Issues' (assuming NaN means 'No known health issues').
  5. **Data Splitting:** Dividing the data into training and testing sets (train_test_split).
  6. **Data Transformation:** Applying OrdinalEncoder and OneHotEncoder using ColumnTransformer for categorical features.
  7. **Model Training:** Training several regression models (Decision Tree, Linear Regression, SVR, Neural Network, Kernel Ridge Regression) to predict BMI.
  8. **Model Evaluation:** Evaluating models using Mean Absolute Percentage Error (MAPE) and comparing their performance.

### Results & Conclusion

The analysis revealed insights into the distribution of lifestyle factors and their correlations. After preprocessing and training, the Kernel Ridge Regression model achieved the lowest Mean Absolute Percentage Error (MAPE) of approximately 13.05%, suggesting it was the best-performing model among those tested for BMI prediction on this dataset.

