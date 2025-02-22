# Virat-Kohli-Intl-Centuries-Dataset

## Overview
As I am a big cricket fan,this project is for all the cricket lovers. This project focuses on classifying and predicting the match outcomes based on our legendary Indian Batsman King Virat Kohli. Using historical data of his centuries, a Decision Tree algorithm is applied to analyse patterns and make predictions regarding future match results.

## Dataset Files
- ViratKohli.csv: The dataset containing details of Kohli's centuries, match results, and other relevant attributes.
- Virat Kohli Intl Centuries.ipynb:  Jupyter Notebook containing data preprocessing, model training, and evaluation.

## Features
- Predicts match outcomes based on Virat Kohli's centuries
- Use Decision Tree algorithm for classication
- Utilizes Historical data to identify trends and patterns.

## Tech Stack
- Machine Learning Algorithm: Decision Tree
- Jupyter Notebook: For model development and Evaluation
  
## Study our dataset
- We have ten attributes in our dataset:No.,Runs,Team,Format,Position,Innings,Venue,Date,Ground,Result.
- Our feature variables are Team,Format,Position,Innings,Venue,Ground which will help us in classifying our dataset.
- Our target variable is Result with possible outcomes:Won,Lost and Draw.

## Important Libraries implemented in our model
- Pandas:  It is a Python library used for working with data sets. It has functions for analysing, cleaning, exploring, and manipulating data. Pandas allows us to analyze big data and make conclusions based on statistical theories. We used pandas to load the dataset, explore the dataset and clean the dataset.
- Matplotlib: Matplotlib is a low level graph plotting library in python that serves as a visualization utility. It is open source and we can use it freely
- Sklearn: It is a powerful open-source machine learning library in Python that provides tools for data preprocessing, model training, evaluation, and deployment. It is built on top of NumPy, SciPy, and Matplotlib, making it a popular choice for data science and machine learning tasks. This library has a module named tree which has a function DecisionTreeClassifier( ) which we will be using to classify our datasets.

## Implementation
- Load the dataset,ViratKohli.csv and explore it using pandas library.
- Clean the dataset by removing all the inconsistent values from the dataset.
- Convert all categorical values in the dataset to numerical values because most Machine Learning models, including Decision Trees can effectively process numerical data.
- Removing the attributes which are not needed.
- Choose our feature variables i.e team,format,position,innings,venue and ground
- Choose our target variable i.e result
- Train our model and check its accuracy (I get around 98%)
- Finally we plot the decision tree using plot_tree function and predict the outcomes

## Installation and Usage
- Clone the repository
  
