
# 🚢 Titanic Survival Prediction (Kaggle Competition + Flask Deployment)

This project is my solution for the **Kaggle Titanic - Machine Learning from Disaster** competition.  
I trained ML models in Jupyter Notebook and deployed a **Flask web app** with **Ngrok** so users can input passenger details and predict survival in real time.

---

## 📂 Project Structure




---

## 📊 Dataset (from Kaggle)
- **train.csv** → Training data (with survival labels)  
- **test.csv** → Test data (without labels)  
- **gender_submission.csv** → Example submission  

📌 [Competition Link](https://www.kaggle.com/c/titanic)

---

## ⚙️ Workflow
### 🔹 In Jupyter Notebook
1. Data Cleaning & Preprocessing (handled missing values, encoded categorical features)
2. Exploratory Data Analysis (EDA) with Matplotlib/Seaborn
3. Feature Engineering (created new features like `FamilySize`)
4. Model Training (Logistic Regression, Decision Trees, Random Forest, etc.)
5. Evaluation (cross-validation & accuracy comparison)
6. Saved best model → `logistic_regression_model.pkl`

### 🔹 In Flask App
- Built a web interface where users can enter:
  - Passenger Class, Sex, Age, SibSp, Parch, Fare, Embarked
- Flask receives inputs → model predicts survival (`0 = No, 1 = Yes`)
- Deployed using **Ngrok** for public access.

---

## 🚀 Deployment
Run the Flask app with Ngrok:

```bash
python app.py
