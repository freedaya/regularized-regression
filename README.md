# 🏠 House Price Prediction using Regularized Regression

## 👋 Hi again!
This project explores **house price prediction** using the Boston Housing Dataset with a focus on **regularized regression techniques**. The analysis compares **Ridge Regression** and **Lasso Regression** to understand feature influence, handle multicollinearity, and improve prediction stability.

## 🎯 Project Goals
- Understand the relationship between housing features and price
- Handle multicollinearity using regularization techniques
- Build and compare **Ridge** and **Lasso Regression** models
- Select the best model using a validation-based approach
- Evaluate model performance using regression metrics
- Interpret feature impact on house prices

## 📂 Dataset Overview
The dataset contains socio-economic, environmental, and structural attributes
related to housing prices.

- **crim**: Crime rate per town  
- **zn**: Proportion of large residential land  
- **indus**: Proportion of industrial area  
- **chas**: Proximity to Charles River (0 = No, 1 = Yes)  
- **nox**: Nitric oxide concentration  
- **rm**: Average number of rooms per dwelling  
- **age**: Proportion of older buildings  
- **dis**: Distance to employment centers  
- **rad**: Accessibility to major highways  
- **tax**: Property tax rate  
- **ptratio**: Student–teacher ratio  
- **black**: Demographic indicator  
- **lstat**: Percentage of lower-status population  
- **medv**: Median house price (**Target**)

## 🛠 Tools & Libraries
- Python  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Scikit-learn  
- Google Colab (or any Jupyter-based environment)

## 📝 Project Workflow

### 1️⃣ Data Preparation
- Loaded Boston Housing dataset
- Checked missing values and data consistency
- Split data into **training**, **validation**, and **test** sets

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualized distributions of numerical features
- Identified skewed variables
- Analyzed correlation between features and target variable

### 3️⃣ Correlation Analysis & Feature Selection
- Created correlation heatmap
- Identified highly correlated features to detect multicollinearity
- Used regularization instead of manual feature removal

### 4️⃣ Modeling: Ridge & Lasso Regression
- Trained Ridge and Lasso models with multiple regularization strengths (lambda)
- Selected optimal lambda using **validation RMSE**
- Compared coefficient behavior between models

### 5️⃣ Model Evaluation
- Evaluated final models using:
  - MAE
  - RMSE
  - MAPE

## 📊 Analysis & Insights

### Feature Interpretation
- **rm** (number of rooms) shows a strong **positive** impact on house price  
- **lstat** (lower-status population percentage) has a strong **negative** impact  
- Environmental and accessibility factors (nox, tax, rad) negatively influence prices  
- Results are consistent with housing economics theory

### Ridge vs Lasso Regression
- **Ridge Regression**
  - Retains all features with reduced coefficients
  - Handles multicollinearity more effectively
  - Produces more stable predictions

- **Lasso Regression**
  - Performs feature selection by shrinking some coefficients to zero
  - Produces a simpler, more interpretable model
  - Slightly lower predictive accuracy compared to Ridge

### Model Evaluation Results
- Ridge Regression achieved slightly lower **MAE** and **RMSE**
- RMSE values are similar, indicating comparable robustness
- Ridge shows lower **MAPE**, meaning better relative accuracy

### Model Conclusion
- **Ridge Regression** is more suitable for **prediction accuracy**
- **Lasso Regression** is useful for **feature selection and interpretability**
- Choice of model depends on business goal: prediction vs explanation

## 📌 Key Takeaways
- Regularization is crucial for handling multicollinearity
- Ridge provides stable and reliable predictions
- Lasso helps simplify the model by selecting key drivers
- Combining statistical insight with domain understanding improves model trustworthiness
