# 🛒 BigMart Pricing Optimization

This project predicts the **sales of products at BigMart outlets** using machine learning. It involves detailed data preprocessing, feature engineering, model evaluation, and final prediction generation — optimized for real-world retail pricing strategy.

---

## 📁 Project Structure

| Notebook | Description |
| `1_DataCleaning.ipynb` | Handles missing values and inconsistent labels |
| `2_EDA.ipynb` | Visual exploration of sales drivers and data distribution |
| `3_Feature_Engineering.ipynb` | Encoding categorical variables, feature transformations |
| `4_Model_Building_&_Evaluation.ipynb` | Trains multiple ML models and evaluates using RMSE and CV |
| `5_Test_preprocessed.ipynb` | Preprocesses test data using the same pipeline |
| `submission.csv` | Final output file for submission |
| `test_final_processed.pkl` | Pickled test dataset after preprocessing |
| `final_model.pkl` | (Optional) Trained model for reuse or deployment |

---

## ✅ Problem Statement

BigMart wants to **estimate sales** for each product at their various outlets, enabling better pricing and inventory decisions.

---

## 💡 Features Used

- `Item_Weight`
- `Item_Fat_Content`
- `Item_Visibility`
- `Item_Type`
- `Item_MRP`
- `Outlet_Size`
- `Outlet_Location_Type`
- `Outlet_Type`
- `Outlet_Establishment_Year`

---

## ⚙️ Models Trained & Evaluated

| Model | RMSE | CV RMSE |
| Linear Regression | 1069.10 | 1132.91 |
| Ridge Regression | 1069.23 | 1132.89 |
| Random Forest | 1098.76 | 1148.57 |
| **XGBoost Regressor** | **1065.42** | **1125.92** ✅ Best

---

## 📦 Libraries Used

- Python 3.9+
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- xgboost
- joblib / pickle

---

## 📊 Final Output

- Predictions stored in `submission.csv`
- Test data transformed and saved as `test_final_processed.pkl`

---

## ✨ Author

**Debabrath Debabrath**  
👨‍💻 Aspiring Data Scientist  
📧 debabrath07@gmail.com

---

## 📌 Notes

- All categorical features were encoded consistently across train and test.
- The preprocessing was done manually (without pipelines) for transparency.
- Feature distributions and correlations were visualized for better insight.
