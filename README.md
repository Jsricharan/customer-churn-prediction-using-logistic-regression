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

## Installation and Setup

### Prerequisites

- **Python 3.8 or higher**
- **MongoDB Atlas account** (or local MongoDB instance)
- **Git** (optional, for cloning the repository)

### 1. Install Dependencies

```
pip install -r requirements.txt
```
### 2. Set Up MongoDB

- Create a MongoDB Atlas account or set up a local MongoDB instance.
- Update the MongoDB connection string in `app.py`:

```python
client = MongoClient("mongodb+srv://<username>:<password>@cluster0.b4j8abw.mongodb.net/")
```
### 3. Train the Model

- Place your dataset (`BankCustomerData.csv`) in the `datasets` folder.

- Run the model training script:

```bash
python model_train.py
```
- This will generate `churn_model.pkl` and `scaler.pkl` in the `models` folder.

### 4. Run the Application

```bash
python app.py
```
- The application will start at [http://127.0.0.1:5000](http://127.0.0.1:5000).

### 5. Access the Web Interface

- Open a browser and navigate to [http://127.0.0.1:5000](http://127.0.0.1:5000).
- Register or log in to start using the churn prediction system.

---

## Usage

### Single Prediction

- Navigate to the **Explorer** tab.
- Adjust sliders or input fields for customer attributes.
- View the churn probability and risk level.

### Batch Prediction

- Navigate to the **Batch** tab.
- Upload a CSV file containing customer data.
- View and download predictions for all records.

### View History

- Navigate to the **History** tab to see past predictions.

---

## Future Enhancements

- **Real-Time Alerts:** Notify businesses when high-risk churn customers are identified.
- **Advanced Models:** Experiment with Random Forest, XGBoost, or neural networks.
---



