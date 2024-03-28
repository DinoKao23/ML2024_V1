# EDA on Real Estate data
## Overview
To perform machine learning on dataset, we need to explore the dataset and see if the dataset meet the requirement of machine learning. We will perform various steps to clean the dataset. For instance, we need to deal with **Outliers, Missing Value, Repetitive data, and Normalization**. This notebook provides the basic step by step guidance with clear comment to explain what each cells is doing and how these steps makes the final dataset.

## Requirements 
Python 3.x
NumPy
Pandas
scikit-learn
matplotlib
seaborn
statsmodels

## Installation
Ensure that Python 3.x is installed on your system. You can download and install it from Python's official website.

Once Python is installed, use the following commands to install the required libraries:

pip install matplotlib
pip install pandas
pip install numpy
pip install scikit-learn
pip install seaborn
pip install seaborn
pip install statsmodels

## Data Source
Use the URL to extract the CSV file from Dr.Brahma's [Github]https://github.com/ArinB/MSBA-CA-Data/raw/main/CA01/house-price-train.csv "From Here")
 

## Program Files
CA01-checkpoint.ipynb: This Jupyter Notebook contains the entire code and logic for the spam classifier.
Running the Program
Open the CA01-checkpoint.ipynb.ipynb file in Jupyter Notebook.
Make sure you download the the require package before you run the notebook.
If you didn't run it the order or try to rerun specific cells, it might fail due to the variable might have been modified.

## Code Explanation
The program consists of Three parts:

## Part 1: Variable Observation
Observing variables is essential in data analysis. At first, we select different type of data and perform different grpahing on object or number. And we use a for-loop to make multiple histograms makes it easier to explore the data. We can look at how different categories behave by creating these histograms one after another. This method helps us observe trends and differences in the data. Mosaic graphs are good tool to explore and make it simple to compare categories. You can set your own category data and decide what variable you want to put it  in.

## Part 2: Pre-Processing
Getting data ready for analysis is important. First, we remove any empty values. We check how much data is missing to see if it's a lot or a little. Then, we fill in the missing data with the median if the data is numeric or most frequent word if data is object. Lowercasing makes everything consistent, and dropping duplicates ensures we don't have the same info repeated. Looking for outliers, particularly using the Interquartile Range (IQR) method, helps us identify unusual data points in the dataset. Turning categorical data into dummy variables makes it easier to work with Machine Learning. Lastly, standardizing data with MinMaxScaler make sure all the data within range 0 to 1.

## Part 3:
Finally, we check multicollinearity and use feature selection to choose the right data for machine learning. We use two methods to determine multicollinearity: VIF and Heatmap. With VIF, we quantify the extent of correlation among predictors. And Heatmap can visualize intricate relationships between variables, making us more informed in our decision-making. After dropping columns with high correlation, this is the final dataset.


## Author
Dino Kao, Kendall Prager, Kali Recker

