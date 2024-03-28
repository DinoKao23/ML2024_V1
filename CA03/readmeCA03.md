# Census Income Prediction using Decision Tree Classifier

## Project Overview
This project aims to predict individual income levels using a Decision Tree Classifier. The dataset is sourced from the U.S. Census Bureau and includes demographic and employment-related information. The goal is to classify individuals into two income categories: those who earn more than 50K a year and those who earn 50K or less.

## Data Source
The dataset is obtained from the U.S. Census Bureau and includes several demographic variables. It contains the following characteristics:
- Number of target classes: 2 ('>50K' and '<=50K')
- Number of attributes: 7
- Number of instances: 48,842

## Methodology
The project involves several key steps:
1. Data Quality Analysis: Identifying missing values, outliers, and performing descriptive statistics.
2. Data Preprocessing: Handling categorical data using label encoding and splitting the dataset into training and testing sets.
3. Model Building: Using `DecisionTreeClassifier` from scikit-learn to build and train the decision tree model.
4. Model Evaluation: Calculating performance metrics like accuracy, precision, recall, and F1 score.
5. Hyperparameter Tuning: Experimenting with different hyperparameters to optimize model performance.
6. Model Visualization: Visualizing the decision tree to interpret the model's decision-making process.
7. Prediction: Making income predictions for new individuals using the trained model.

## Results
The project successfully identifies the best-performing decision tree model through systematic hyperparameter tuning. The model's accuracy and other performance metrics are discussed in detail in the Jupyter notebook.

## How to Run
- Clone the repository to your local machine.
- Ensure that Python and necessary libraries (`pandas`, `matplotlib`, `seaborn`, `scikit-learn`) are installed.
- Open the Jupyter notebook (`CA03.ipynb`) and run the cells sequentially to replicate the analysis.

## Dependencies
- Python 3.x
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Authors
- Dino Kao, Kendall Prager, Kali Recker

## Acknowledgements
- Thanks to the U.S. Census Bureau for providing the dataset.
- This project is part of Introduction to Machine Learning under the guidance of Professor Brahma.


