# Email Spam Classifier using Naive Bayes
## Overview
This email spam classifier is a machine learning program that uses the Naive Bayes algorithm to differentiate between spam and non-spam (ham) emails. It's designed to be a supervised learning solution, requiring training data to learn the characteristics of spam and ham emails. 

## Requirements and imports
Python 3.x: the version of python that is being used
NumPy: fundamental packages for numerical computations in Python
scikit-learn: open-source machine learning library for the Python programming language
NLTK: used to import the stopwords set from the Natural Language Toolkit (NLTK)

Counter class within the collections module: it is a subclass of dict and is used for counting hashable objects
os: provides a way of using operating system dependent functionality

## Installation
Ensure that Python 3.x is installed on your system. You can download and install it from Python's official website.

Once Python is installed, use the following commands to install the required libraries:

pip install numpy
pip install scikit-learn
pip install nltk

## Data Folder Structure
The program expects the data to be in a specific folder structure:

The training data should be in a folder named train-mails.
The test data should be in a folder named test-mails.
Both these folders should be in the same directory as the .ipynb (Jupyter Notebook) file.

## Program Files
Email Spam Classifier.ipynb: This Jupyter Notebook contains the entire code and logic for the spam classifier.
Running the Program
Open the Email Spam Classifier.ipynb file in Jupyter Notebook.
Ensure that the train-mails and test-mails folders are in the same directory as the notebook.
Run the cells in the notebook sequentially.

## Code Explanation
The program consists of several key functions:

make_Dictionary(root_dir): This function creates a frequency dictionary of words from the training emails. It considers the most common words found in the emails.

extract_features(mail_dir): This function extracts features from the emails in the specified directory. It creates a feature matrix where each row corresponds to an email, and each column represents one of the most frequent words in the training set.

## Training and Prediction:

The program trains a Gaussian Naive Bayes model using the GaussianNB() class from scikit-learn.
The model is trained on the feature matrix and labels from the training data.
It then predicts labels for the test data and calculates the accuracy of these predictions.
Output
The program outputs the accuracy of the model, which is the proportion of the test emails that were correctly classified as spam or ham.

## Customization
You can modify the paths for the training and test data if your folder structure is different. Ensure the paths in the TRAIN_DIR and TEST_DIR variables are updated accordingly.

## Author
Dino Kao, Kendall Prager, Kali Recker

