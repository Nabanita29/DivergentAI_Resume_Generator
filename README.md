# DivergentAI_Resume_Generator
Resume Screening with Machine Learning
Overview
This project aims to develop a machine learning model that can screen resumes and identify candidates that are best suited for a particular job. The model is trained using a combination of real and synthetic resumes, and is tested on both diverse and non-diverse sets of resumes to detect any potential biases in the hiring process.

Requirements
To run this project, you'll need:

Python 3.x
OpenAI API key
MATLAB
MATLAB engine API for Python

Installation
Clone this repository to your local machine.
Install the required Python packages using pip: pip install -r requirements.txt.
Set up your OpenAI API key.
Install MATLAB on your machine.
Install the MATLAB engine API for Python.

Usage
Preprocess the real resumes by running the preprocess_real_resumes.py script. This script will clean and standardize the text data, and save the preprocessed resumes to a CSV file.
Generate synthetic resumes using OpenAI's GPT-3 API by running the generate_synthetic_resumes.py script. This script will prompt the API with various job titles, and save the generated resumes to a CSV file.
Preprocess the synthetic resumes by running the preprocess_synthetic_resumes.py script. This script will clean and standardize the text data, and save the preprocessed resumes to a CSV file.
Combine the preprocessed real and synthetic resumes into a single dataset by running the combine_datasets.py script. This script will merge the two CSV files into a single file, and save it to a new CSV file.
Train the machine learning model using the combined dataset by running the train_model.py script. This script will load the combined dataset, extract relevant features using MATLAB's feature extraction functions, and train an SVM model using MATLAB's machine learning functions.
Use the trained model to predict the outcomes of diverse and non-diverse resumes by running the predict_outcomes.py script. This script will load diverse and non-diverse resumes from CSV files, convert them to feature vectors using bag of words, use the trained SVM model to make predictions, and analyze the predictions to detect any potential biases in the hiring process.
