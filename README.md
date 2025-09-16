# Car Price Prediction with Python  

This repository contains my beginner-friendly **machine learning project** to predict used car prices.  
Starting from a raw dataset, I cleaned and preprocessed the data, explored key trends, and built several regression models to predict selling prices.

---

## 🎯 Objectives
- Prepare and clean raw car data for analysis and modelling.
- Explore the dataset to understand how factors like age, mileage, fuel type and transmission affect price.
- Build and evaluate multiple regression models to predict car selling price.
- Learn and demonstrate essential data science skills (EDA, preprocessing, model evaluation) in a real-world context.

---

## 📚 Skills Demonstrated
- **Data Cleaning & Preprocessing:**  
  Handling missing values, dropping duplicates, standardising column names, converting year to car age, creating new features like price per kilometre, dealing with outliers.
- **Exploratory Data Analysis:**  
  Descriptive statistics, value counts, correlations, histograms, scatter plots, bar charts, heatmaps.
- **Feature Engineering:**  
  Binning ages, encoding categories, deriving new ratios.
- **Machine Learning Models:**  
  Linear Regression, Lasso, Ridge, Polynomial Regression with `scikit-learn`.
- **Model Evaluation:**  
  R² Score, Mean Squared Error, residual analysis, cross-validation, GridSearchCV for hyperparameter tuning.
- **Communication:**  
  Visualising trends, comparing models and summarising findings.

---

## 📝 Project Workflow

### 1. Data Cleaning & Preprocessing
- Loaded the dataset into a Pandas DataFrame and reviewed column meanings.
- Checked for missing values (counts and percentages) and dropped rows where the target (`selling_price`) was missing.
- Filled missing mileage values with the column mean.
- Removed duplicate rows.
- Converted “year” to car age (e.g. 2025–2015 = 10 years).
- Standardised categorical values (e.g. transmission casing) and column names.
- Detected and filtered out unrealistic price outliers (<10,000 or >5,000,000).
- Converted any numeric strings to numbers.
- Created a new feature “price_per_kilometre” by dividing selling price by mileage.
- Reset index and saved the cleaned dataset as `cleaned_cars.csv`.

### 2. Exploratory Data Analysis
- Calculated average selling price and most common fuel type.
- Plotted histogram of selling prices and scatter plot of car age vs. price.
- Grouped cars by fuel type to compute average prices.
- Created bar charts for cars per transmission type.
- Identified car with highest mileage.
- Computed correlation between mileage and selling price and visualised correlations in a heatmap.
- Compared manual vs automatic prices.
- Calculated average selling price by year of manufacture and plotted the trend.
- Found most expensive car per fuel type and most frequent brand.
- Examined top 5 combinations of fuel type and transmission.

### 3. Machine Learning
- Reviewed Linear Regression assumptions (linearity, residuals, multicollinearity, etc.) and checked them with plots/statistics.
- Trained a Linear Regression model on selected features and evaluated it using R² and MSE.
- Applied Lasso and Ridge Regression and compared their performance.
- Used cross-validation for Ridge model.
- Tuned Ridge alpha using GridSearchCV.
- Tried Polynomial Regression and compared with Linear model.
- Plotted predicted vs. actual prices for the best model.
- Summarised which model performed best and potential improvements.



