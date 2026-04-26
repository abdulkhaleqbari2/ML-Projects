# Car Price Prediction
A supervised machine learning project that predicts the resale price of used cars based on key vehicle attributes — built using Linear Regression and Lasso Regression with comprehensive model evaluation.


📌 Problem Statement
The used car market is highly dynamic and pricing a vehicle fairly is challenging for both buyers and sellers. This project builds a predictive model that estimates the selling price of a used car based on features like manufacturing year, fuel type, transmission, and more — enabling data-driven pricing decisions.

📊 Dataset
The dataset (car data.csv) contains real-world used car listings with the following features:
FeatureDescriptionYearManufacturing year of the carPresent_PriceCurrent ex-showroom price (in lakhs)Kms_DrivenTotal kilometers drivenFuel_TypePetrol / Diesel / CNGSeller_TypeDealer / IndividualTransmissionManual / AutomaticOwnerNumber of previous ownersSelling_Price⭐ Target variable — resale price (in lakhs)

🔧 Tech Stack

Language: Python 3
Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
Models: Linear Regression, Lasso Regression
Environment: Jupyter Notebook


🚀 Project Workflow
1. Data Loading & Exploration

Loaded the dataset using Pandas
Inspected shape, data types, and null values
Analyzed distribution of categorical features: Fuel_Type, Seller_Type, Transmission

2. Data Preprocessing

Encoded categorical variables using label encoding:

Fuel_Type: Petrol → 0, Diesel → 1, CNG → 2
Seller_Type: Dealer → 0, Individual → 1
Transmission: Manual → 0, Automatic → 1


No missing values found — dataset was clean

3. Feature Engineering

Features (X): Year, Present_Price, Kms_Driven, Fuel_Type, Seller_Type, Transmission, Owner
Target (y): Selling_Price
Train-Test Split: 90% training / 10% testing (random_state=2)

4. Model Training & Evaluation
📈 Linear Regression
SplitR² ScoreTraining Set~87%Test Set~83%
📉 Lasso Regression
SplitR² ScoreTraining Set~87%Test Set~84%

Lasso Regression performed slightly better on the test set, suggesting it handled overfitting more effectively through L1 regularization.

5. Visualization

Scatter plots comparing Actual vs Predicted prices for both train and test sets across both models

6. Prediction on New Data

Demonstrated real-world inference by predicting prices for custom car inputs using both trained models


📂 Project Structure
car-price-prediction/
│
├── Project1.ipynb       # Main Jupyter Notebook
├── car data.csv         # Dataset
└── README.md            # Project documentation

▶️ How to Run

Clone the repository

bash   git clone https://github.com/your-username/car-price-prediction.git
   cd car-price-prediction

Install dependencies

bash   pip install pandas numpy matplotlib seaborn scikit-learn

Launch the notebook

bash   jupyter notebook Project1.ipynb

💡 Key Learnings

Applied the complete ML pipeline — from EDA to model deployment-ready inference
Compared Linear vs Lasso Regression and understood the role of regularization
Gained hands-on experience in feature encoding for categorical variables
Evaluated model performance using R² score on both training and test splits




🔮 Future Improvements

 Try ensemble models like Random Forest or XGBoost for better accuracy
 Add hyperparameter tuning using GridSearchCV
 Build an interactive web app using Streamlit or Flask
 Perform deeper EDA with correlation heatmaps and feature importance plots

#Author: Mohammed Abdul khaleq bari
