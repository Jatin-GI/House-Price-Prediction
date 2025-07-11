# 🏠 Bengaluru House Price Prediction using Machine Learning & Optuna

This project focuses on predicting **house prices in Bengaluru** using supervised machine learning models combined with **Optuna hyperparameter tuning**. The objective is to build an accurate regression model that can estimate housing prices based on key features.

---

## 📌 Problem Overview

- Predict housing prices based on various property attributes such as:
  - Area type
  - Location
  - Total square footage
  - Number of bathrooms and balconies
- The project addresses challenges like **missing values**, **data cleaning**, and **hyperparameter tuning** for robust price prediction.

---

## 📊 Dataset Summary

- **Dataset:** `Bengaluru_House_Data.csv`
- **Total Records:** 13,300 (after cleaning)
- **Key Features:**
  | Feature      | Description                                 |
  |------------- |--------------------------------------------- |
  | `area_type`  | Type of property area (Built-up, Plot, etc.) |
  | `availability` | Availability status                        |
  | `location`   | Property location within Bengaluru           |
  | `total_sqft` | Total area in square feet                    |
  | `bath`       | Number of bathrooms                          |
  | `balcony`    | Number of balconies                          |
  | `price`      | Price in lakhs (Target)                      |

---

## 🚀 Technologies Used

- Python 🐍
- Pandas & NumPy 📊
- Scikit-learn 🤖
- XGBoost 🌲
- Optuna ⚙
- Matplotlib & Seaborn 📈
- Jupyter Notebook

---

## 🔍 Data Cleaning & Preprocessing

- Filled missing values in `bath` and `balcony` using **mean imputation**.
- Processed `total_sqft` values with formats like `1000 - 1200` by taking the average.
- Dropped high-missing columns (`society` and `size`).
- Removed extreme outliers in `bath`, `total_sqft`, and `price`.
- Applied **log transformation** to the target variable (`price`) to normalize skewed data.
- Used **OneHotEncoder** for categorical variables and **StandardScaler** for numerical features via **ColumnTransformer**.

---

## ⚙ Model Building & Hyperparameter Tuning

- Built an end-to-end pipeline combining:
  - **Preprocessing** (`OneHotEncoder`, `StandardScaler`)
  - **Regression models**: 
    - Linear Regression
    - Random Forest Regressor
    - XGBoost Regressor
- Used **Optuna** for automated:
  - Model selection
  - Hyperparameter tuning
  - Train-test split optimization

---

## 📈 Best Model & Performance

- ✅ **Best Model:** XGBoost Regressor
- ✅ **Best R² Score:** 0.8614 on test data
- ✅ Model pipeline saved as:  

```bash
---

## 🖥 How to Run the Project

```bash
# 1️⃣ Clone the repository
git clone https://github.com/Jatin-GI/bengaluru-house-price-prediction.git
cd bengaluru-house-price-prediction

# 2️⃣ (Optional) Create and activate a virtual environment
python -m venv venv
venv\Scripts\activate       # On Windows
source venv/bin/activate    # On Mac/Linux

# 3️⃣ Install the dependencies
pip install -r requirements.txt

# 4️⃣ Run the Jupyter Notebook
jupyter notebook
```
## ✅ Key Takeaways

- Built a complete **end-to-end regression pipeline** for Bengaluru house price prediction.
- Applied extensive **data cleaning** (missing value imputation, outlier removal, feature engineering).
- Used **Optuna** for **automated model selection and hyperparameter tuning** across Linear Regression, Random Forest, and XGBoost.
- Achieved a solid **R² score of 0.8614** on the test set (log-transformed prices).
- The final model pipeline is reusable, scalable, and saved as a `.pkl` file for future deployment.

---

## 🚀 Future Improvements

- 🌐 **Deployment:** Build a user-friendly web app using **Streamlit** or **Flask** for live price predictions.
- ⚙ **Model Enhancements:** Experiment with additional models like **CatBoost**, **LightGBM**, or **Stacked Ensembles**.
- 📊 **Explainability:** Add **SHAP** or **LIME** for interpretable machine learning and better decision transparency.
- 📈 **Data Expansion:** Incorporate additional features (proximity to metro, schools, hospitals) for better accuracy.
- ⏱ **Real-Time Serving:** Deploy as a REST API using **FastAPI** or **Docker** for production use cases.

---

## 🤝 Contributions

Contributions are always welcome! Here’s how you can help:

- ⭐ **Star this repository** to show your support.
- 🐛 **Report bugs** or **open issues** for improvements.
- 🔀 **Submit pull requests** with new features, better models, or enhanced visualizations.

Please make sure to follow good coding practices and provide clear explanations in your contributions.

---

## 📜 License

This project is shared **for educational and research purposes only**.  
All content is provided **“as-is” without any warranty or guarantees**.  
Please use responsibly, especially when applying to real-world financial or decision-making systems.

---

## 👨‍💻 Author

**Jatin Gupta**  
📧 [guptajatin0416@gmail.com](mailto:guptajatin0416@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/jatin-gupta-b02b37292/)  
🔗 [GitHub](https://github.com/Jatin-GI)

---
