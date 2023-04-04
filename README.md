# Testing for Data Bias with Google's Perspective API
# I310D Assignment 10, Spring 2023

## Table of Contents
1. Introduction 
2. Project Goals
3. Documentation
4. Project Directory
5. Results

## Introduction
This project was competed as coursework for I310D: Introduction to Human-Centered Data Science at the University of Texas at Austin. The assignment required students to test the Perspective API for potential bias by creating a hypothesis about the model's performance, designing tests on a sample set of data, and interpreting the results. 

The Perspective API is a tool developed by Google's Jigsaw team that uses machine learning models to assess the "toxicity" of text input. The API has been used by various online platforms to moderate comments and conversations in realtime. 

## Project Goals
The goal of this project was to determine whether the Perspective API can accurately predict the toxicity of a text input containing profanity if the profane language is censored using asterisks. To do this, a dataset of test comments were written and manually labeled and the Perspective API was used to assess their toxicity labels. The accuracy of the API was analyzed to determine if censorship is a bias present in the model.

## Documentation 
To complete this project, several APIs and Python libraries were used. Documentation for each is linked below. 
- [Perspective API](https://developers.perspectiveapi.com/s/docs?language=en_US)
- [Google API Client for Python](https://googleapis.github.io/google-api-python-client/docs/)
- [JSON](https://docs.python.org/3/library/json.html#module-json)
- [SciKit Learn](https://scikit-learn.org/stable/modules/model_evaluation.html#model-evaluation).
- [Pandas](https://pandas.pydata.org/docs/)

## Project Directory 
- `Data_Bias_Code.ipynb`: This is the code that was used for all steps of this project; written and hosted in a Jupyter notebook. 
- `Test_Comments_with_API_Scores.csv`: This is the set of test comments and the related attributes

## Results
It was determined that the API is effective in scoring toxicity when profanity is censored. There are several implications and conclusions that can be drawn from this, more details are in `Data_Bias~Code.ipynb` under **2. Results and Insights**
