# 🤖📞 Model Arena:The Ultimate Classifier Showdown🎯📊


A machine learning project to predict customer churn for a telecom company using supervised classification techniques. This project includes model comparison, hyperparameter tuning, feature importance analysis, and Power BI dashboard visualization.


## 🚀 Objective

To build a robust machine learning model that accurately predicts whether a customer is likely to churn, empowering telecom companies to proactively retain customers and reduce churn rates.


## 📁 Files in This Repository

🗂️ Dataset & Code:
- 📄 `WA_Fn-UseC_-Telco-Customer-Churn.csv` — Original dataset
- 🧠 `Hackathon_Implementation.ipynb` — Notebook for EDA, modeling & evaluation
- 📝 `Model_scores_before_tuning.csv` — Performance before tuning
- 📝 `Model_scores_after_tuning.csv` — Performance after tuning
- 📊 `Feature_importance_gradient_boosting.csv` — Important features
- 💾 `best_model.pkl` — Final model (Gradient Boosting)

---



## 🧠 ML Workflow

### 🔹 Data Preprocessing
- Null value handling
- Label encoding for categorical features
- Feature scaling and transformation


## 🧠 Models Used

🔍 Trained and compared:
- ✔️ Logistic Regression
- ✔️ Random Forest
- ✅ Gradient Boosting *(Best)*
- ✔️ XGBoost
- ✔️ Support Vector Machine
- ✔️ K-Nearest Neighbors

### 🔹 Hyperparameter Tuning
- Tuned top models using GridSearchCV for optimal performance.

### 🔹 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score


## 🥇 Best Performing Model: Tuned Gradient Boosting
- Accuracy: 0.801
- F1-Score: 0.592
- Selected due to high performance after tuning and balance of metrics.

## 🔑 Top 5 Important Features

🔥 Features that most influence churn:
1. 📃 Contract Type
2. 📅 Tenure
3. 🛠️ Tech Support
4. 💰 Monthly Charges
5. 🌐 Internet Service

## 📊 Power BI Dashboard

- Interactive charts to visualize model comparisons
- Feature importance bar graphs
- Customer churn insights by contract, tenure, and payment method

# 👥 Contributors

- Zoya Naseer - Project Lead, Model Development, Dashboard Visualization
- Ujwal Reddy - Model Development, Hyperparameter Tuning, Model Evaluation
- Nisha Rana - KPI's, PowerBi Dasboard

#  Conclusion 🔚
This project demonstrates a comprehensive approach to predicting customer churn in the telecom industry. By leveraging various machine learning models, performing hyperparameter tuning, and creating an insightful Power BI dashboard, this solution equips telecom companies with the tools necessary to proactively address churn and retain customers. The chosen Gradient Boosting model offers a good balance of accuracy and performance, making it a reliable tool for real-world business applications. The model is ready for deployment, providing a scalable solution for further use and improvement.

## 💾 Model Export (.pkl)

Model is saved in .pkl format using pickle for easy deployment.

```python
import pickle

# Save the best model
with open("best_model.pkl", "wb") as file:
    pickle.dump(best_gb, file)

# Load the model
with open("best_model.pkl", "rb") as file:
    loaded_model = pickle.load(file)
