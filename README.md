# Heart Disease Prediction System

A machine learning-based classification application that predicts the presence or absence of heart disease based on user-provided health-related numerical data. The project uses a pre-trained Logistic Regression model and an interactive Streamlit interface to generate binary classification predictions.

## Overview

This project implements a supervised machine learning classification system designed to identify potential indications of heart disease.

It uses a trained **Logistic Regression Model (LRM)** to classify input data into two categories:

- **0 – No Heart Disease:** The model predicts the absence of heart disease.
- **1 – Heart Disease:** The model predicts the presence of heart disease.

The application integrates the trained machine learning model with a Streamlit web interface, allowing users to submit numerical health-related inputs and receive classification results.

## Key Features

- **Heart Disease Classification:** Predicts the presence or absence of heart disease.
- **Supervised Machine Learning:** Implements a binary classification approach.
- **Logistic Regression:** Uses a probabilistic classification algorithm.
- **Pre-trained Model Integration:** Loads a serialized model using Python Pickle.
- **Numerical Input Processing:** Converts comma-separated user inputs into numerical arrays.
- **Interactive Web Application:** Provides a Streamlit-based interface for generating predictions.
- **Real-Time Inference:** Produces predictions without requiring model retraining during application execution.

## Machine Learning Workflow

The system follows a straightforward classification pipeline:

1. **User Input:** Accepts numerical health-related data through the Streamlit interface.
2. **Input Processing:** Splits comma-separated values and converts them into numerical data.
3. **Feature Preparation:** Organizes the input values into a two-dimensional NumPy array.
4. **Model Loading:** Loads the pre-trained Logistic Regression model from `LRM.pkl`.
5. **Classification:** Passes the processed input features to the trained model.
6. **Prediction Output:** Generates a binary classification result.
7. **Result Display:** Displays the predicted classification through the Streamlit interface.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Machine Learning | Scikit-learn |
| Classification Algorithm | Logistic Regression |
| Numerical Processing | NumPy |
| Data Processing | Pandas |
| Web Application | Streamlit |
| Model Serialization | Pickle |

## Project Structure

```text
heart_disease_prediction.model/
│
├── Streamlit Website Application/
│   └── Streamlit application deployment
│
├── LRM.pkl
│   └── Trained Logistic Regression model
│
├── heart.py
│   └── Streamlit application and prediction logic
│
├── requirements.txt
│   └── Project dependencies
│
└── .gitignore
```



## Usage

The application accepts comma-separated numerical inputs representing the health-related features used during model training.

**Input Format**

```text
feature_1, feature_2, feature_3, ..., feature_n
```

The input values must follow the exact feature order and format expected by the trained model.

After submitting the input, click the prediction button to obtain the classification result.

**Possible Outputs:**

- No heart disease predicted.
- Heart disease predicted.

## Model Implementation

The project uses a **Logistic Regression classifier** stored in `LRM.pkl`.

Logistic Regression is a supervised classification algorithm that estimates the probability of an observation belonging to a particular class.

The trained model is loaded using Python's Pickle module and performs inference on the numerical input features.


## Medical Disclaimer

This project is developed for educational and machine learning experimentation purposes only. It is not a clinically validated diagnostic system and must not be used as a substitute for professional medical advice, diagnosis, or treatment.

A model prediction does not establish whether an individual has heart disease. Consult a qualified healthcare professional for medical evaluation.

