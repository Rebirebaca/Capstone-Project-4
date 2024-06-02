# Industrial-Copper-Modeling

## Introduction

* This project focuses on modelling industrial copper data using Python and various libraries such as pandas, numpy, scikit-learn.
* The objective of the project is to preprocess the data, handle missing values, detect outliers, and handle skewness. 
* Additionally, regression and classification models will be built to predict the selling price and determine if a sale was won or lost.
* The trained models will be saved as a pickle file for later use in a Streamlit application.

## Project Structure

The project consists of the following files and directories: data/: Directory containing the raw data file(s) for the industrial copper dataset. modeling.ipynb: Jupyter Notebook file containing the code for building regression and classification models. pickle_file_generator.ipynb: Jupyter Notebook file for generating the pickle file of the trained model. streamlit_app.py: Python file containing the Streamlit application code for using the trained model to predict selling price and status.

## Requirements

This project requires the following libraries to be installed:
*NumPy
*Pandas
*Matplotlib
*Seaborn
*Pickle
*Scikit-learn
*Xgboost
*Streamlit

## Approach

### Data Understanding:

*Identify variable types (continuous, categorical) and their distributions.
*Handle categorical variables with '00000' values and treat reference columns as categorical.
*Data preprocessing, including handling missing values and skewness.

### Exploratory Data Analysis (EDA):

Visualize outliers and skewness using Seaborn's boxplot, distplot, violinplot.

### Regression Model:

The copper industry deals with less complex data related to sales and pricing. However, this data may suffer from issues such as skewness and noisy data, which can affect the accuracy of manual predictions. Dealing with these challenges manually can be time-consuming and may not result in optimal pricing decisions. A machine learning regression model can address these issues by utilizing advanced techniques such as data normalization, outlier detection and handling, handling data in wrong format, identifying the distribution of features, and leveraging tree-based models, specifically the decision tree algorithm.

### Classification Model:

Another area where the copper industry faces challenges is in capturing the leads. A lead classification model is a system for evaluating and classifying leads based on how likely they are to become a customer. You can use the STATUS variable with WON being considered as Success and LOST being considered as Failure and remove data points other than WON, LOST STATUS values.

## Getting Started:

1. Clone the repository.
2. Install the required libraries.
3. Run the Streamlit app using the command: streamlit run app.py.
4. Enter the values for each column to get the Selling_Price predicted value or Status (Won/Lost).


