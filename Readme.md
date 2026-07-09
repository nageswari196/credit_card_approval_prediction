# Credit Card Approval Prediction System

## Overview

The Credit Card Approval Prediction System is a Machine Learning-based web application that predicts whether a customer's credit card application is likely to be approved or rejected based on applicant information.

The project uses historical customer data, performs data preprocessing, feature engineering, model training, and provides predictions through a Flask web application.

---

## Features

- User-friendly web interface using Flask
- Predicts Credit Card Approval
- Machine Learning-based prediction
- Automatic categorical data encoding
- Feature Engineering
- Model Comparison
- Random Forest Best Model Selection
- Prediction Confidence Score
- Responsive UI

---

## Technologies Used

### Programming Language

- Python 3

### Machine Learning

- Scikit-learn
- XGBoost
- SMOTE (Imbalanced-Learn)

### Web Development

- Flask
- HTML
- CSS

### Data Processing

- Pandas
- NumPy

### Visualization

- Matplotlib
- Seaborn

### Model Saving

- Joblib

---

## Project Structure

```
Credit_card_approval_system/
│
├── app.py
├── prepare_data.py
├── train_model.py
├── requirements.txt
│
├── model.pkl
├── encoders.pkl
├── feature_names.pkl
├── model_comparison.csv
│
├── dataset/
│   ├── application_record.csv
│   ├── credit_record.csv
│   └── final_credit_dataset.csv
│
├── templates/
│   ├── index.html
│   └── result.html
│
├── static/
│   └── style.css
│
└── README.md
```

---

## Dataset

The project uses two datasets:

- application_record.csv
- credit_record.csv

The datasets are merged using the Applicant ID.

After preprocessing, a new dataset is created:

```
final_credit_dataset.csv
```

---

## Machine Learning Workflow

1. Load Dataset
2. Handle Missing Values
3. Feature Engineering
4. Label Encoding
5. Train-Test Split
6. Apply SMOTE
7. Train Multiple Models
8. Compare Model Performance
9. Save Best Model
10. Deploy using Flask

---

## Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

Random Forest achieved the best performance and is saved as the final model.

---

## Feature Engineering

The following features are created:

- AGE
- YEARS_EMPLOYED

The following columns are removed:

- DAYS_BIRTH
- DAYS_EMPLOYED
- FLAG_MOBIL

---

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Score

---

## Input Features

The web application accepts:

- Gender
- Own Car
- Own House
- Annual Income
- Number of Children
- Income Type
- Education Type
- Family Status
- Housing Type
- Age
- Years Employed
- Work Phone
- Phone
- Email
- Occupation
- Family Members

---

## Output

The application predicts:

- Approved
- Rejected

It also displays:

- Prediction Confidence (%)

---

## Installation

Clone the repository.

```bash
git clone <repository_url>
```

Install dependencies.

```bash
pip install -r requirements.txt
```

---

## Train the Model

Run:

```bash
python prepare_data.py
```

Then:

```bash
python train_model.py
```

The following files will be generated:

```
model.pkl
encoders.pkl
feature_names.pkl
model_comparison.csv
```

---

## Run the Application

Start the Flask server.

```bash
python app.py
```

Open your browser.

```
http://127.0.0.1:5000
```

---

## Project Workflow

```
Raw Dataset
      │
      ▼
Data Preprocessing
      │
      ▼
Feature Engineering
      │
      ▼
Label Encoding
      │
      ▼
SMOTE
      │
      ▼
Model Training
      │
      ▼
Model Comparison
      │
      ▼
Best Model Selection
      │
      ▼
Model Deployment
      │
      ▼
Prediction
```

---

## Future Enhancements

- Deep Learning Models
- Explainable AI (SHAP/LIME)
- User Authentication
- Database Integration
- Cloud Deployment
- REST API
- PDF Report Generation

---

## Author

**Nageswari**

B.Tech Computer Science and Engineering

Vignan's Lara Institute of Technology & Science

---

## License

This project is developed for educational and academic purposes.
