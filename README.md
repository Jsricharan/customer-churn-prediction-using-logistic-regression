# Customer Churn Prediction Using Logistic Regression

## Project Overview

This project is a machine learning-based system designed to predict customer churn using Logistic Regression. It analyzes historical customer data to identify customers likely to discontinue a service or subscription, enabling businesses to implement proactive retention strategies. The system includes a web-based application with a Flask backend, MongoDB for data storage, and an interactive frontend built with HTML, CSS, and JavaScript.


---

## Key Features

- **Machine Learning Model:** Uses Logistic Regression to predict churn probability based on customer attributes like credit score, tenure, age, and estimated salary.

- **Web Application:** Provides an intuitive dashboard for visualizing churn predictions and customer insights.

- **User Management:** Secure login and registration system with MongoDB for storing user data and prediction history.

- **Batch Prediction:** Supports bulk predictions by uploading CSV files.

- **Data Preprocessing:** Includes normalization and feature selection to improve model accuracy.

---

## Technologies Used

### Backend
- **Flask:** Web framework for handling routing, sessions, and API endpoints.
- **PyMongo:** MongoDB integration for storing user data and prediction history.
- **Werkzeug:** Password hashing and security utilities.

### Machine Learning
- **Scikit-learn:** Implements the Logistic Regression model and data preprocessing.
- **Pickle:** Serializes and saves the trained model for reuse.
- **NumPy & Pandas:** Handles numerical operations and data manipulation.

### Frontend
- **HTML, CSS, JavaScript:** Builds the interactive user interface and dashboard.

### Database
- **MongoDB:** NoSQL database for storing user credentials and prediction logs.

---

## Installation

### Prerequisites

- **Python 3.8 or higher**
- **MongoDB Atlas account** (or local MongoDB instance)
- **Git** (optional, for cloning the repository)
