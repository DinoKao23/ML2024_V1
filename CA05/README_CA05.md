# CA05

## Movie Recommendation using K-Nearest Neighbors (KNN) Algorithm

### Introduction
Welcome to the Movie Recommendation System using the K-Nearest Neighbors (KNN) algorithm! This system is designed to provide personalized movie recommendations based on user preferences and similarities between movies. This README file will guide you through the setup, usage, and customization of the recommendation model.

### Setup
Before running the recommendation system, ensure you have the following prerequisites installed:

Python (version 3.12)
Required Python libraries: pandas, scikit-learn, plotly
You can install these libraries using pip:

Copy code
```
pip install plotly pandas scikit-learn
```
Once you have the prerequisites installed, download the following files:

CA05.ipynb: Notebook showing the step applying algorithm.



### Dataset
The movie_data.csv file contains the following columns:

Movie ID: Unique identifier for each movie. <br />
Movie Name: Title of the movie. <br />
IMDB Rating: Rating by users from IMDB. <br />
Biography: 1 means this is Biography, 0 means this is not Biography <br />
Drama: 1 means this is Drama, 0 means this is not Drama <br />
Thriller: 1 means this is Thriller, 0 means this is not Thriller <br />
Comedy: 1 means this is Comedy, 0 means this is not Comedy <br />
Crime: 1 means this is Crime, 0 means this is not Crime <br />
Mystery: 1 means this is Mystery, 0 means this is not Mystery <br />
History: 1 means this is History, 0 means this is not History <br />
Label: Use for KNN algorithm prediction


### EDA
Using Plotly, we can create interactive visualizations that allow us to explore various aspects of the data more effectively. We will examine the distribution of movie genres, user ratings, and other relevant features to better understand the dataset's structure.

By visualizing the dataset, we can identify any patterns or trends that may inform our recommendation system. This exploration will guide us in preprocessing the data and selecting appropriate features for our K-Nearest Neighbors (KNN) algorithm.


### KNN
The K-Nearest Neighbors (KNN) algorithm is a powerful technique for making recommendations based on similarity metrics. In this project, we will implement KNN with  n=5, meaning we will consider the five closest neighbors when making recommendations.

We take an user input "The Post" as the movie he/she likes, and use the algorithm to find the movie recommendation to this user.



### Feedback and Support
If you encounter any issues or have suggestions for improvement, please feel free to reach out to us. We are committed to providing the best possible movie recommendation experience and welcome your feedback.

Happy movie watching!

