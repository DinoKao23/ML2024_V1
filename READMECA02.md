# Email Spam Classifier using Naive Bayes
## Overview
This email spam classifier is a machine learning program that uses the Naive Bayes algorithm to differentiate between spam and non-spam emails. It's designed to be a supervised learning solution, requiring training data to learn the characteristics of spam and ham emails. 

## Requirements and imports
Python 3.x: the version of python that is being used.
NumPy: fundamental packages for numerical computations in Python.
scikit-learn: open-source machine learning library for the Python programming language.
NLTK: used to import the stopwords set from the Natural Language Toolkit (NLTK).

Counter class within the collections module: it is a subclass of dict and is used for counting hashable objects.
os: provides a way of using operating system dependent functionality.

## Installation
Ensure that Python 3.x is installed on your system. You can download and install it from Python's official website.

Once Python is installed, use the following commands to install the required libraries:

pip install numpy
pip install scikit-learn
pip install nltk

(use "!" before the pip for jypter notebook enviornments)

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
The program consists of several key functions and variables:

make_Dictionary(root_dir): This function creates a frequency dictionary of words from the training emails. It considers the most common words found in the emails. Essentially, this function is a part of text preprocessing, often used in natural language processing (NLP) tasks, where you want to create a list of the most frequent words in a dataset, filtering out non-alphabetic and too short words.

extract_features(mail_dir): This function extracts features from the emails in the specified directory. It creates a feature matrix where each row corresponds to an email, and each column represents one of the most frequent words in the training set. It creates a feature vector based on the frequency of dictionary words in each file and assigning labels based on whether the file is spam or not. This function is typically part of a text classification workflow in machine learning.

TRAIN_DIR, TEST_DIR, and T_DIR: used to define variables that store the paths to different directories containing email data for training and testing purposes

Output: A feature matrix (train_features_matrix, test_features_matrix). Where each row represents an email, and each column corresponds to one of the words in the dictionary. The values in the matrix represent the frequency of these words in each email. A label vector (train_labels, test_labels), where each element is a label (like 0 or 1) indicating the classification of the email (e.g., spam or not spam).

Accuracy Score:
GaussianNB: coding the algorithm (specific type of Naive Bayes classifier that assumes features follow a normal distribution).
- Within the model.fit: Put in the training feauture matrix (dictionary we have for each word) and training label to predict which email is spam and which email is not spam.
- Predicting the trained model (Naive Bayes) data
- Pred: after training, the model is used to predict the labels of the test data
- accuracy_score: evaluates the performance of the model in terms of accuracy.
- This is a common workflow in supervised machine learning tasks.

## Training and Prediction:

The program trains a Gaussian Naive Bayes model using the GaussianNB() class from scikit-learn.
The model is trained on the feature matrix and labels from the training data.
It then predicts labels for the test data and calculates the accuracy of these predictions.
Output
The program outputs the accuracy of the model, which is the proportion of the test emails that were correctly classified as spam or non-spam. 
The program also outputs a confusion matrix, predicting the number of correctly and incorrectly categorized emails in the model

## Customization
You can modify the paths for the training and test data if your folder structure is different. Ensure the paths in the TRAIN_DIR and TEST_DIR variables are updated accordingly.

## Author
Dino Kao, Kendall Prager, Kali Recker

