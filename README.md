# IBM Recommendations Project

## Overview

This project focuses on analyzing user interactions with articles on the IBM Watson Studio platform to make personalized article recommendations. The goal is to explore various recommendation techniques and evaluate their effectiveness.

## Table of Contents

1. [Introduction](#introduction)
2. [File Descriptions](#file-descriptions)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Future Work](#future-work)
6. [Acknowledgements](#acknowledgements)

## Introduction

The project involves several key tasks:

1. **Exploratory Data Analysis (EDA)**: Explore the dataset to understand user interactions and article popularity.
2. **Rank-Based Recommendations**: Recommend articles based on their interaction frequency.
3. **User-User Collaborative Filtering**: Use user similarity based on interactions to recommend articles.
4. **Matrix Factorization**: Apply Singular Value Decomposition (SVD) to predict user interactions with articles.

### Detailed Steps

1. **Exploratory Data Analysis**:
   - Analyze user interactions with articles to understand data distributions and user behavior.
   - Visualize data to gain insights into interaction patterns and article popularity.

2. **Rank-Based Recommendations**:
   - Identify and recommend the most popular articles based on interaction counts.
   - This approach is particularly useful for new users with no interaction history.

3. **User-User Collaborative Filtering**:
   - Create a user-item matrix where rows represent users and columns represent articles.
   - Identify similar users based on their interaction history and recommend articles that similar users have interacted with.

4. **Matrix Factorization**:
   - Use Singular Value Decomposition (SVD) to decompose the user-item matrix into latent features.
   - Predict potential user-article interactions and recommend articles based on these predictions.

## File Descriptions

- **Recommendations_with_IBM.ipynb**: Jupyter Notebook with the main implementation and analysis.
- **project_test.py**: Python script containing test solutions to validate the functions implemented in the notebook.
- **data/articles_community.csv**: CSV file containing metadata for articles available on the IBM platform.
- **data/user-item-interactions.csv**: CSV file with user-article interaction data.

## Installation

Ensure you have the following Python libraries installed:

- Pandas
- Numpy
- Matplotlib
- Pickle

These libraries are compatible with Python 3.5 and above. Installation can be managed via Anaconda or pip.

## Usage

1. Clone the repository and navigate to the project directory.
2. Open and run the Jupyter Notebook (`Recommendations_with_IBM.ipynb`) to execute the analysis and recommendation algorithms.
3. Execute the Python script (`project_test.py`) to validate the functionality of the implemented methods.

## Future Work

- **Content-Based Recommendations**: Develop a content-based recommendation system using NLP techniques to analyze article content and recommend similar articles.
- **A/B Testing**: Conduct A/B testing to compare the effectiveness of different recommendation systems in practice and gather user feedback.
- **Deployment**: Consider deploying the recommendation system using a web framework like Flask for real-time recommendations.

## Acknowledgements

- [Udacity](https://www.udacity.com) for providing the Data Scientist Nanodegree program and creating the projects for me to do.
- [IBM](https://www.ibm.com) for supplying the user interaction data used.
