# Machine Learning with Python: Model Persistence using Pickle and Joblib

## Project Overview

This project demonstrates how to train a Machine Learning model using Scikit-Learn's Linear Regression algorithm and persist the trained model using two popular serialization techniques: **Pickle** and **Joblib**.

Model persistence is an essential step in the Machine Learning lifecycle, enabling trained models to be stored and reused for inference without retraining.

---

## Objectives

* Train a Linear Regression model on housing price data.
* Predict house prices based on area.
* Save the trained model using Pickle.
* Save the trained model using Joblib.
* Load saved models and perform predictions.
* Understand model serialization techniques used in production environments.

---

## Dataset

The dataset contains housing information with the following attributes:

| Feature | Description               |
| ------- | ------------------------- |
| Area    | House area in square feet |
| Price   | House price               |

Sample Data:

| Area | Price  |
| ---- | ------ |
| 2600 | 550000 |
| 3000 | 565000 |
| 3200 | 610000 |
| 3600 | 680000 |
| 4000 | 725000 |

---

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-Learn
* Pickle
* Joblib
* Jupyter Notebook

---

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas and prepared for training.

### 2. Model Training

A Linear Regression model is trained using house area as the independent variable and house price as the target variable.

### 3. Prediction

The trained model predicts house prices for new input values.

### 4. Model Persistence

The trained model is serialized and stored using:

* Pickle (`.pkl`)
* Joblib (`.joblib`)

### 5. Model Reloading

Saved models are loaded back into memory and used for prediction without retraining.

---

## Results

Model Parameters:

* Coefficient: `135.78767123`
* Intercept: `180616.43835616432`

Prediction Example:

| Area (sq ft) | Predicted Price |
| ------------ | --------------- |
| 5000         | 859,554.79      |

---

## Pickle vs Joblib

| Feature                             | Pickle   | Joblib    |
| ----------------------------------- | -------- | --------- |
| Built into Python                   | ✓        | ✗         |
| Suitable for General Python Objects | ✓        | ✓         |
| Optimized for NumPy Arrays          | ✗        | ✓         |
| Recommended for Scikit-Learn Models | Good     | Preferred |
| Performance with Large Models       | Moderate | Better    |

---

## Real-World Relevance

Model persistence is widely used in production Machine Learning systems for:

* House Price Prediction
* Loan Approval Systems
* Fraud Detection
* Recommendation Engines
* Customer Churn Prediction
* Healthcare Analytics

By saving trained models, organizations reduce computation costs and enable faster deployment of Machine Learning solutions.

---

## Repository Structure

```text
├── homeprices.csv
├── jupyter_notebooks.ipynb
├── model_pickle.pkl
├── model_joblib.joblib
└── README.md
```

## Learning Outcomes

Through this project, I gained hands-on experience with:

* Linear Regression
* Model Serialization
* Pickle
* Joblib
* Scikit-Learn
* Machine Learning Deployment Fundamentals

---

## Future Enhancements

* Build a Flask/FastAPI prediction API
* Create a Streamlit web application
* Deploy the model on cloud platforms
* Add model evaluation metrics
* Extend to multiple feature regression models

---


