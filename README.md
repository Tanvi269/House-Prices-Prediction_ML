# 🏠 House Prices Prediction – Kaggle Competition

## 📌 Project Description
This project is a machine learning solution for the **Kaggle House Prices: Advanced Regression Techniques** competition.  
The objective is to predict the **final sale price of residential homes** in Ames, Iowa based on various housing features.

The project demonstrates an **end-to-end machine learning workflow**, from data preprocessing to Kaggle leaderboard submission.

---

## 📂 Dataset Information
The dataset is provided by Kaggle and contains **79 explanatory features** describing residential homes.

### Files Used
- `train.csv` – Training dataset (includes target variable `SalePrice`)
- `test.csv` – Test dataset (without target variable)
- `sample_submission.csv` – Sample submission format
- `data_description.txt` – Detailed explanation of all features

---

## 🛠️ Tools & Technologies
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Google Colab  
- Kaggle  

---

## ⚙️ Methodology

### 1. Data Loading
- Loaded training and test datasets using Pandas.

### 2. Data Preprocessing
- Combined train and test datasets for consistent preprocessing.
- Handled missing values:
  - Numerical features → filled with median values.
  - Categorical features → filled with `"None"`.

### 3. Feature Encoding
- Converted categorical variables into numerical form using **Label Encoding**.

### 4. Target Variable Transformation
- Applied **log transformation (`log1p`)** on `SalePrice` to reduce skewness and improve model performance.

### 5. Model Training
- Trained a **Random Forest Regressor** on the processed training data.

### 6. Prediction & Submission
- Generated predictions for the test dataset.
- Converted predictions back using `expm1`.
- Created `submission.csv` in Kaggle-required format.
- Successfully submitted predictions to the Kaggle leaderboard.


