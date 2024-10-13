

# 🏦 Loan Status Prediction System  

This project demonstrates how to predict loan statuses using machine learning models such as **RandomForestClassifier** and **XGBClassifier**. We preprocess categorical data, train models, and generate predictions for loan statuses. The system is intended to help financial institutions or lenders predict whether a loan will be approved or not based on various factors.

---

## 📋 Project Overview  

The **Loan Status Prediction System** uses historical loan data to train machine learning models that predict the loan status (approved or denied). We employ **Random Forest** and **XGBoost** classifiers to achieve high accuracy. The system handles categorical data, trains models, and generates predictions for test data, which can be exported to CSV files.

---

## 🛠️ How the Project Works  

1. **Dataset Preprocessing**:  
   - Categorical features such as `person_home_ownership` and `loan_intent` are converted to numerical values using the `replace()` method.  
   - The `id` column is dropped, and target and feature variables are separated.

2. **Model Training and Prediction**:  
   - Two models are used: **RandomForestClassifier** and **XGBClassifier**.
   - The dataset is split into **training and testing sets** (80% training, 20% testing) using `train_test_split`.
   - Models are trained and evaluated using **accuracy score** on both the training and test data.

3. **Generating Predictions for Test Data**:  
   - Test data is processed similarly, and predictions are saved to CSV files.

---

## 🗂️ Dataset Features  

The dataset includes the following features:

- **person_home_ownership**: Categorical values representing ownership status (e.g., RENT, MORTGAGE).  
- **loan_intent**: Reason for taking the loan (e.g., EDUCATION, MEDICAL).  
- **loan_grade**: Loan grade assigned by the institution (A-G).  
- **cb_person_default_on_file**: Whether the borrower has defaulted before (Y/N).  
- **loan_status**: The target variable indicating loan approval status.

---

## 🚀 Running the Project  

### Prerequisites  

Ensure you have the following libraries installed:

```bash
pip install pandas scikit-learn xgboost
```

### Steps to Run  

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/Ashwadhama2004/loan-status-prediction.git
   cd loan-status-prediction
   ```

2. **Place the Dataset**:  
   Ensure that `train.csv` and `test.csv` are in the project folder.

3. **Run the Code**:  
   You can execute the script using:

   ```bash
   python loan_prediction.py
   ```

---

## 🛠️ Code Breakdown  

1. **Data Preprocessing**:
   - Replace categorical values with numerical ones using `replace()`.
   - Drop unnecessary columns (e.g., `id`).
   - Split data into **X** (features) and **Y** (target).

2. **Model Training**:
   - Use **RandomForestClassifier** to train on `X_train` and `Y_train`.
   - Train **XGBClassifier** on the entire dataset for enhanced predictions.

3. **Generating Predictions**:
   - Predict loan status for test data using trained models.
   - Save predictions to `solution5.csv` and `solution6.csv`.

4. **Handling Data Types**:
   - Convert object columns to numeric using `pd.to_numeric()`.

---

## 📈 Results  

The models yield high accuracy for loan status prediction. Sample performance:

- **Random Forest Accuracy (Test Data)**: 85%
- **XGBClassifier Accuracy**: 88%

The system can be further improved by tuning hyperparameters or adding new features.

---

## 📜 License  

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## 🤝 Connect  

For any questions or feedback, feel free to reach out:

- **GitHub**: [Ashwadhama2004](https://github.com/Ashwadhama2004)

---

This project showcases how machine learning models can be effectively applied to financial data for predictive analysis. Happy coding! 🚀
