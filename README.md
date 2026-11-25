# Online Shoppers Purchasing Intention Prediction

An end-to-end Machine Learning project that predicts whether an online visitor is likely to complete a purchase during a browsing session.

## 🌐 Live Web Application

**Try the application here:**

[Online Shoppers Purchasing Intention Prediction](https://online-shoppers-purchase-intention.streamlit.app/)

The application allows users to enter visitor and browsing-session information and receive a purchase prediction with the estimated purchase probability.

---

## 📌 Project Overview

Understanding online customer purchasing behaviour is important for e-commerce businesses. Identifying visitors who are more likely to make a purchase can help businesses improve marketing strategies, personalize customer experiences, and optimize website performance.

This project applies supervised Machine Learning classification techniques to predict the purchasing intention of online shoppers based on their browsing and session-related characteristics.

The target variable is **Revenue**, which indicates whether a visitor completed a purchase.

## 🎯 Objectives

- Analyse online shopping session behaviour.
- Perform data preprocessing and exploratory data analysis.
- Identify important factors influencing purchasing intention.
- Handle class imbalance using appropriate techniques.
- Build and compare multiple classification models.
- Evaluate model performance using suitable classification metrics.
- Develop an interactive web application for purchase prediction.

## 📊 Dataset Information

The project uses the Online Shoppers Purchasing Intention dataset.

The dataset contains visitor information, browsing behaviour, session characteristics, and the target variable `Revenue`.

### Features Used

| Category | Features |
|---|---|
| Page Activity | Administrative, Informational, ProductRelated |
| Page Duration | Administrative_Duration, Informational_Duration, ProductRelated_Duration |
| Session Behaviour | BounceRates, ExitRates, PageValues, SpecialDay |
| Visitor Information | VisitorType, Weekend |
| Technical Information | OperatingSystems, Browser, Region, TrafficType |
| Temporal Information | Month |
| Target Variable | Revenue |

## 🤖 Machine Learning Approach

The project follows a structured Machine Learning workflow:

1. Data loading and inspection
2. Exploratory Data Analysis (EDA)
3. Data cleaning and preprocessing
4. Feature engineering
5. Handling class imbalance
6. Model training and comparison
7. Hyperparameter tuning
8. Threshold selection
9. Final model evaluation
10. Model serialization and deployment

### Model Evaluation

Since the target variable is imbalanced, model performance is evaluated using multiple metrics rather than relying only on accuracy.

The evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- PR-AUC
- Confusion Matrix

The classification threshold is selected using a separate validation dataset.

## 🧠 Prediction Models

The deployed application provides two model options:

**1. Full Feature Model**

Uses all available input features to generate a purchase prediction.

**2. Reduced Feature Model**

Uses a reduced set of features by excluding selected session-related variables to examine model performance with fewer predictors.

Both models use their respective saved classification thresholds.

## 💻 Web Application Features

The Streamlit application provides:

- Professional and interactive user interface.
- Input fields for all required prediction features.
- Full Feature and Reduced Feature model selection.
- Purchase probability estimation.
- Purchase / No Purchase classification.
- Visual prediction results.
- Interactive probability gauge.

## 🛠️ Technologies Used

- **Python** – Programming language
- **Pandas** – Data manipulation
- **NumPy** – Numerical computing
- **Scikit-learn** – Machine Learning algorithms and preprocessing
- **XGBoost** – Gradient boosting
- **Imbalanced-learn** – Class imbalance handling
- **Matplotlib & Seaborn** – Data visualization
- **Plotly** – Interactive visualizations
- **Streamlit** – Web application development
- **Joblib & Cloudpickle** – Model serialization
- **GitHub** – Version control and project hosting
- **Streamlit Community Cloud** – Application deployment


## ⚙️ Installation and Usage

To run the application locally:

### 1. Clone the repository

```bash
git clone https://github.com/dishishah051/ml-project.git
```

### 2. Navigate to the project directory

```bash
cd ml-project
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

### 4. Activate the virtual environment

**Windows PowerShell:**

```powershell
.\.venv\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Streamlit application

```bash
python -m streamlit run app.py
```

The application will open in your browser.

## 📈 Project Outcome

This project demonstrates an end-to-end Machine Learning classification workflow, from data analysis and model development to deployment through an interactive web application.

It provides an accessible interface for exploring how browsing-session characteristics can be used to estimate online shoppers' purchasing intentions.

## ⚠️ Limitations

- Predictions depend on the quality and representativeness of the training dataset.
- The model identifies patterns in historical session data and does not guarantee actual purchasing behaviour.
- The reduced-feature model is an alternative feature-set experiment, not necessarily a real-time prediction model.
- Model performance may vary when applied to different e-commerce platforms or customer populations.
---

**Live Application:** [Open Online Shoppers Purchasing Intention Prediction](https://online-shoppers-purchase-intention.streamlit.app/)
