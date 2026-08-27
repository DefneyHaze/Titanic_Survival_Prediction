# Titanic_Survival_Prediction

The sinking of the RMS Titanic in 1912 is one of the most infamous maritime disasters in history. Out of more than 2,200 passengers and crew, only around 710 survived. This dataset, made famous by Kaggle, provides passenger details such as age, sex, class, fare, and port of embarkation, along with whether they survived.

The goal of this project is to build a predictive model that estimates the likelihood of survival based on passenger attributes. The workflow follows a complete data science pipeline.

---

## 📂 Project Structure
titanic-survival-prediction/
│
├── data/              # raw dataset (CSV)
├── notebooks/         # Jupyter notebooks (EDA, modeling)
├── images/            # plots for README
├── src/               # optional Python scripts
├── requirements.txt   # dependencies
└── README.md          # project overview


---

## ⚙️ Steps in the Workflow
1. **Data Cleaning** — handled missing values (Age median, Embarked mode, dropped Cabin).
2. **Exploratory Data Analysis (EDA)** — visualized distributions and survival patterns.
3. **Feature Engineering** — created FamilySize, extracted Title, encoded categorical variables.
4. **Modeling** — trained Logistic Regression and Random Forest models.
5. **Evaluation** — compared accuracy and feature importance.
6. **Conclusion** — summarized insights and future improvements.

---

## 📊 Results
| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | ~78%     |
| Random Forest       | ~82%     |

- **Random Forest Feature Importance**:  
  - Sex, Pclass, and Fare were the strongest predictors.  
  - Title and FamilySize added meaningful context.  
  - Embarked had smaller impact.

---

## 📸 Key Visuals
1. Survival by Sex <img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/4fe254d0-5418-4e1a-9e35-0710d66968a3" />

2. Feature Importance <img width="912" height="547" alt="image" src="https://github.com/user-attachments/assets/759180e1-274f-43b4-87f4-6447b79ff9b3" />


---

## 🎯 Insights
- Women had much higher survival rates than men.  
- 1st class passengers survived more often than 3rd class.  
- Higher fares correlated with survival.  
- Small families had better odds than large ones.  
- Social status (Title) influenced survival outcomes.

---

## 🚀 Future Work
- Hyperparameter tuning and cross-validation.  
- Try advanced models (XGBoost, LightGBM).  
- Deploy as a simple web app for interactive predictions.

---

## 🛠 Tech Stack
- Python, pandas, numpy  
- seaborn, matplotlib  
- scikit-learn  
- Jupyter Notebook

