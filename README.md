# 🚚 Supply Chain Delivery Delay Prediction Engine

## 📌 Project Overview

Timely delivery is one of the most critical aspects of supply chain management. Delivery delays can increase operational costs, reduce customer satisfaction, and negatively impact business performance.

This project develops a **Machine Learning-based Supply Chain Delivery Delay Prediction Engine** that predicts whether a shipment is likely to be delivered on time or delayed based on historical logistics, shipment, supplier, and transportation data.

The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and model deployment preparation.

---

# 🎯 Problem Statement

Develop a predictive model that identifies potential delivery delays before shipment completion, enabling businesses to take proactive measures to improve logistics efficiency and customer satisfaction.

---

# 🎯 Business Objectives

- Predict delivery delays before shipment
- Improve customer satisfaction
- Optimize logistics planning
- Reduce transportation costs
- Improve supplier performance monitoring
- Enhance supply chain efficiency
- Support data-driven operational decisions

---

# 📊 Dataset

The dataset contains shipment, supplier, transportation, and delivery information.

### Example Features

| Feature | Description |
|----------|-------------|
| Order ID | Unique order identifier |
| Product ID | Product identifier |
| Supplier | Supplier name |
| Warehouse | Warehouse location |
| Shipping Mode | Air, Road, Rail, Sea |
| Carrier | Logistics provider |
| Order Date | Date order was placed |
| Dispatch Date | Shipment dispatch date |
| Expected Delivery | Expected delivery date |
| Distance | Delivery distance |
| Traffic Level | Traffic conditions |
| Weather Condition | Weather during transport |
| Vehicle Type | Delivery vehicle |
| Shipment Weight | Weight of shipment |
| Delivery Time | Actual delivery duration |
| Delay Status | Target Variable |

### Target Variable

| Value | Meaning |
|--------|----------|
| 0 | Delivered On Time |
| 1 | Delivery Delayed |

---

# ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- Joblib
- Jupyter Notebook

---

# 📚 Libraries Used

```python
import pandas as pd
import numpy as np

import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.preprocessing import OneHotEncoder

from sklearn.compose import ColumnTransformer
from sklearn.pipeline import Pipeline

from sklearn.linear_model import LogisticRegression
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier
from sklearn.ensemble import GradientBoostingClassifier

from sklearn.metrics import (
    accuracy_score,
    precision_score,
    recall_score,
    f1_score,
    confusion_matrix,
    classification_report,
    roc_auc_score
)

import joblib
```

---

# 📂 Project Structure

```
Supply-Chain-Delivery-Delay-Prediction-Engine/
│
├── data/
│      └── supply_chain_data.csv
│
├── notebooks/
│      └── Delivery_Delay_Prediction.ipynb
│
├── models/
│      └── delivery_delay_model.pkl
│
├── src/
│      ├── preprocessing.py
│      ├── train.py
│      ├── predict.py
│
├── app.py
├── requirements.txt
├── README.md
└── assets/
```

---

# 🔍 Exploratory Data Analysis (EDA)

Performed analysis includes:

- Dataset Overview
- Missing Value Analysis
- Duplicate Detection
- Statistical Summary
- Delivery Delay Distribution
- Supplier Performance Analysis
- Shipping Mode Analysis
- Delivery Time Distribution
- Warehouse Performance
- Correlation Matrix
- Heatmap
- Box Plot
- Count Plot
- Pair Plot

---

# 🧹 Data Preprocessing

Performed preprocessing includes:

- Handling Missing Values
- Duplicate Removal
- Feature Encoding
- Feature Scaling
- Train-Test Split
- Feature Selection
- Pipeline Creation

---

# ⚙️ Feature Engineering

Feature engineering techniques include:

- One-Hot Encoding
- Standard Scaling
- Date Feature Extraction
- Delivery Duration Calculation
- Distance-Based Features
- Shipment Category Encoding

---

# 🤖 Machine Learning Models

The following models were trained and compared:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Gradient Boosting Classifier
- XGBoost (Optional)
- LightGBM (Optional)

The best-performing model was selected using classification metrics.

---

# 📈 Model Evaluation

Evaluation metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

---

# 🔄 Project Workflow

```
Supply Chain Dataset
         │
         ▼
Data Cleaning
         │
         ▼
EDA
         │
         ▼
Feature Engineering
         │
         ▼
Encoding
         │
         ▼
Scaling
         │
         ▼
Train-Test Split
         │
         ▼
Model Training
         │
         ▼
Model Evaluation
         │
         ▼
Model Saving
         │
         ▼
Delivery Delay Prediction
```

---

# 💾 Model Saving

The trained model is saved using Joblib.

```python
joblib.dump(model, "delivery_delay_model.pkl")
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Supply-Chain-Delivery-Delay-Prediction-Engine.git
```

Navigate to the project directory

```bash
cd Supply-Chain-Delivery-Delay-Prediction-Engine
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

---

# 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
joblib
```

---

# 📸 Example Prediction

### Shipment Information

```
Supplier: ABC Logistics

Shipping Mode: Road

Distance: 850 km

Weather: Heavy Rain

Traffic: High

Vehicle: Truck
```

### Prediction

```
Delivery Status:

⚠️ Delayed

Probability of Delay: 91%
```

---

# 📊 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Visualization
- Feature Scaling
- Feature Encoding
- Classification Algorithms
- Pipeline Development
- Model Evaluation
- Model Serialization
- Business Analytics
- Supply Chain Analytics
- Python Programming

---

# 💼 Business Impact

This project helps organizations:

- Predict shipment delays before delivery
- Improve customer satisfaction
- Reduce logistics costs
- Optimize transportation routes
- Monitor supplier performance
- Improve warehouse efficiency
- Enhance supply chain planning
- Support proactive decision-making

---

# 🔮 Future Improvements

- Hyperparameter Tuning
- Real-Time Shipment Tracking
- GPS-Based Delay Prediction
- Streamlit Dashboard
- FastAPI/Flask Deployment
- Docker Containerization
- Cloud Deployment (AWS, Azure, GCP)
- MLOps Integration
- Explainable AI (SHAP/LIME)
- Time Series Forecasting for Logistics

---

# 📖 Learning Outcomes

Through this project, I learned:

- Building end-to-end machine learning classification pipelines.
- Working with logistics and supply chain datasets.
- Performing exploratory data analysis for operational insights.
- Engineering features from shipment and delivery data.
- Comparing classification algorithms using multiple evaluation metrics.
- Saving and deploying machine learning models for production use.

---

# 👨‍💻 Author

**Mahesh Gurme**

### Skills

- Data Science
- Machine Learning
- Python
- SQL
- Power BI
- Supply Chain Analytics
- Business Analytics
- Artificial Intelligence

---

# ⭐ If you found this project useful, consider giving it a star on GitHub!
