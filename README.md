# London Crime Rate Analysis & Prediction

This project provides a comprehensive analysis and predictive modeling of crime rates in London using historical crime data. The workflow includes data extraction, cleaning, exploratory data analysis (EDA), visualization, feature engineering, and machine learning for crime rate prediction.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Features](#features)
- [Installation & Requirements](#installation--requirements)
- [Usage](#usage)
- [Data Processing Pipeline](#data-processing-pipeline)
- [Modeling Approach](#modeling-approach)
- [Results & Interpretation](#results--interpretation)
- [Author](#author)
- [License](#license)

---

## Project Overview

The goal of this project is to analyze patterns in London crime data and build a predictive model to estimate crime rates based on time, location, and crime type. The project leverages Python data science libraries for data handling, visualization, and machine learning.

---

## Project Structure

```
crime.zip
London_crime_rate_.ipynb
README.md
```

- **crime.zip**: Compressed archive containing monthly crime CSV files.
- **London_crime_rate_.ipynb**: Main Jupyter notebook for data analysis, visualization, and modeling.
- **README.md**: Project documentation.

---

## Features

- **Automated Data Extraction**: Loads and merges multiple months of London crime data from a ZIP archive.
- **Data Cleaning & Preprocessing**: Handles missing values, converts date columns, and prepares data for analysis.
- **Exploratory Data Analysis**: Visualizes crime frequencies, types, and geographic distributions.
- **Feature Engineering**: Aggregates crime counts by month, location, and type for modeling.
- **Predictive Modeling**: Trains a linear regression model using scikit-learn to predict crime rates.
- **Interactive Prediction**: Provides a function to predict crime rates for user-specified month, location, and crime type.
- **Performance Evaluation**: Calculates RMSE for baseline and trained models.

---

## Installation & Requirements

**Python Version:** 3.x

**Required Libraries:**
- pandas
- numpy
- seaborn
- matplotlib
- plotly
- scikit-learn
- statsmodels

**Install dependencies:**
```sh
pip install pandas numpy seaborn matplotlib plotly scikit-learn statsmodels
```

---

## Usage

1. **Prepare Data**: Place `crime.zip` in the project root directory.
2. **Run Notebook**: Open `London_crime_rate_.ipynb` in Jupyter Notebook or VS Code and execute cells sequentially.
3. **Explore Data**: Review visualizations and summary statistics generated in the notebook.
4. **Model Training**: The notebook automatically trains and evaluates a linear regression model.
5. **Make Predictions**: Use the `make_prediction` function to estimate crime rates for specific inputs.

**Example:**
```python
make_prediction("2022-08", "On or near A1", "Bicycle theft")
```

---

## Data Processing Pipeline

1. **Data Loading**: Extracts and concatenates CSV files from the ZIP archive.
2. **Preprocessing**: Converts date columns, handles missing values, and encodes categorical variables.
3. **EDA & Visualization**: Generates bar plots, scatter plots, and time series visualizations to understand crime patterns.
4. **Feature Engineering**: Aggregates data by month, location, and crime type.
5. **Modeling**: Splits data into training and testing sets, trains a linear regression model, and evaluates performance.
6. **Prediction**: Provides an interface for user-driven predictions.

---

## Modeling Approach

- **Baseline Model**: Uses the mean crime rate as a naive predictor.
- **Linear Regression Model**: Incorporates one-hot encoding for categorical features and fits a regression model to predict crime rates.
- **Evaluation Metrics**: Uses Root Mean Squared Error (RMSE) for both baseline and trained models.

---

## Results & Interpretation

- **Visual Insights**: The notebook provides insights into the most frequent crime types, their distribution over time, and geographic hotspots.
- **Model Performance**: RMSE values are reported for both training and testing sets, allowing for assessment of model accuracy.
- **Prediction Functionality**: Users can input a month, location, and crime type to receive a predicted crime rate.

---

## Author

- **Onwumelu Chiderah**

---

## License

This project is intended for educational and research purposes only.

---