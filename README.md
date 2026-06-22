# Iris Classification CI/CD Pipeline

## 📌Project Overview

This project demonstrates a complete Machine Learning Classification Pipeline using the Iris Dataset and GitHub Actions for Continuous Integration and Continuous Deployment (CI/CD).

The pipeline performs:

* Data Loading and Preprocessing
* Feature Engineering
* Model Training
* Model Evaluation
* Confusion Matrix Visualization
* Feature Importance Analysis
* Automated Execution using GitHub Actions

---

## 📊Dataset

The project uses the famous Iris Dataset containing three flower species:

* Setosa
* Versicolor
* Virginica

### 🚀Features

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

### Target

* Flower Species

---

## ⚙️Feature Engineering

Two additional features are created:

### Sepal Length Width Ratio

```python
dataset['sepal_length_width_ratio'] = dataset['sepal_length'] / dataset['sepal_width']
```

### Petal Length Width Ratio

```python
dataset['petal_length_width_ratio'] = dataset['petal_length'] / dataset['petal_width']
```

These engineered features help improve model performance.

---

## 🤖Machine Learning Models

### Logistic Regression

Used for multi-class flower classification.

### Random Forest

Used to analyze feature importance and compare performance.

---

## 📈Evaluation Metrics

The following metrics are calculated:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## 📂Project Structure

```text
1030am_cicd_deployment/
│
├── .github/
│   └── workflows/
│       └── run.yaml
│
├── iris.csv
├── requirements.txt
├── scores.txt
├── train_model.py
└── README.md
```

---

## 🛠️Installation

Clone the repository:

```bash
git clone https://github.com/your-username/1030am_cicd_deployment.git
```

Move into the project directory:

```bash
cd 1030am_cicd_deployment
```

Install required packages:

```bash
pip install -r requirements.txt
```

---

## Run the Project

```bash
python train_model.py
```

The script will:

* Train Machine Learning Models
* Generate Evaluation Metrics
* Create Confusion Matrix
* Generate Feature Importance Plot
* Save Performance Scores

---

## 📦Requirements

```text
numpy
pandas
scikit-learn
matplotlib
seaborn
```

---

## 🔄CI/CD Pipeline

This project uses GitHub Actions to automate model execution whenever code is pushed to the repository.

### Workflow Steps

1. Checkout Repository
2. Setup Python Environment
3. Install Dependencies
4. Execute Model Training Script
5. Validate Successful Execution

---

## 📋Sample Output

The project generates:

* scores.txt
* Confusion Matrix Visualization
* Feature Importance Visualization

Example metrics:

```text
Logistic Regression Accuracy
Precision Score
Recall Score
F1 Score

Random Forest Accuracy
Precision Score
Recall Score
F1 Score
```

---


## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Seaborn
* GitHub Actions

---

## 👨‍💻Author

### Manas Ranjan Meher

GitHub: https://github.com/manasranjanmeher99

LinkedIn: https://www.linkedin.com/in/manas-ranjan-meher-606181280/

---

⭐ If you found this project useful, please consider giving it a star.
