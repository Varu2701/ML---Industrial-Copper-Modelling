# **Industrial Copper Modeling**

## **📌 Project Overview**
This project focuses on predicting the **delivery date difference** for industrial copper orders using **machine learning models**. The dataset includes real-world transactional data with multiple attributes such as product specifications, pricing, customer details, and dates. The goal is to enhance operational planning and improve customer satisfaction by accurately forecasting delivery lead times.

---

## **🧠 Problem Statement**
Given various features of copper transactions, the task is to:
- Clean and preprocess the data
- Engineer relevant features
- Handle missing values and outliers
- Build regression models to predict the number of days between order date and delivery date

---

## **📂 Dataset Description**
The dataset used in this project is `Copper_Set_Result.csv`, containing the following key columns:

- `quantity tons`
- `customer`, `country`
- `application`, `product_ref`, `item type`
- `thickness`, `width`, `selling_price`
- `item_date`, `delivery date`, `status`

---

## **🛠️ Technologies Used**
- **Programming Language**: Python
- **Libraries**: NumPy, Pandas, Seaborn, Matplotlib, Scikit-learn, XGBoost
- **Environment**: Google Colab

---

## **🔍 Data Preprocessing**
- Converted date columns (`item_date`, `delivery date`) to datetime format
- Cleaned invalid or default material references
- Removed or imputed missing values using mode and median strategies
- Applied log transformation to reduce skewness in numerical columns
- Handled outliers using IQR (Interquartile Range) method

---

## **📊 Exploratory Data Analysis**
- Plotted box plots, histograms, and violin plots to visualize distributions
- Generated a correlation heatmap to identify feature relationships
- Explored target variable (`Date_difference`) across different dimensions

---

## **📈 Feature Engineering**
- Extracted date components: day, month, year from `item_date`
- Created a new feature `Date_difference` = `delivery date` - `item_date`
- Encoded categorical columns using **OrdinalEncoder** and **Label Mapping**

---

## **🤖 Model Building**
Tested the following regression models:
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **Extra Trees Regressor**
- **AdaBoost Regressor**
- **Gradient Boosting Regressor**
- **XGBoost Regressor**

Evaluated models using:
- **R² Score**
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**

---

## **✅ Best Performing Model**
- **Random Forest Regressor** achieved the best performance with high accuracy and low error metrics.
- Hyperparameter tuning was done using **GridSearchCV**.

---

## **📦 Model Deployment**
Simulated outcome prediction using custom user input to forecast delivery delays. Also attempted binary classification (Won/Lost) based on predicted delivery difference.

---

## **📌 Conclusion**
This project demonstrates how machine learning can be applied to industrial data for predictive analytics. The model helps improve supply chain planning by forecasting delivery timelines more accurately.

---

## **📁 Folder Structure**
```
├── Copper_Set_Result.csv
├── Industrial_Copper_Modeling.ipynb
├── README.md
```

---

## **📝 Author**
**Varuna Sree**  
AI/ML Enthusiast | Data Science | Web Developer
