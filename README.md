# London Housing Data & ML Pipeline

This project focuses on building a machine learning-ready dataset for predicting **London house prices**, using real-world data from government and public sources. The goal is to create a full end-to-end ML pipeline — from raw data gathering and preparation, through to model training and evaluation.

While the modeling stages are still in progress, the **data collection and preparation phase is complete**, and represents a significant part of this project’s technical depth and value.

---

## Project Objective

The objective of this project is to predict house prices in London using a variety of external and internal features. Unlike typical pre-cleaned datasets (e.g., from Kaggle), this project starts from raw, real-world public data and emphasizes:
- Data sourcing from government portals
- Complex merging across datasets with different structures
- Feature construction and transformation
- Building a usable ML dataset from scratch

---

##  1. Data Collection & Preparation

All raw data was pulled manually from public and government sources, including:

- **UK House Price Index (HPI)** from HM Land Registry  
- **Crime rates** from the UK Home Office  
- **Interest rates** from the Bank of England  
- **Unemployment rates and economic indicators** from official statistics portals  
- **Geographic data** to support matching and merging

### Key Data Engineering Steps (see `data_preparation.ipynb`)

- Merged multiple datasets by **location** (e.g., borough or area) and **time** (e.g., month or year)
- Cleaned and standardized column formats across inconsistent sources
- Aligned **economic indicators** like interest rates and crime stats to monthly sale records
- Constructed a usable column for bedroom count using proximity-matching logic
- Output a **clean, ready-for-EDA dataset** with rich contextual features

> Final output file: `final_cleaned_dataset.csv`  
> This dataset is the product of extensive real-world data wrangling and preparation work.

---

## 2. Exploratory Data Analysis (EDA)  
**_Status: In Progress_**

- Understand distributions, relationships, and correlations
- Identify key drivers of house prices
- Detect skewed variables or further outliers

---

## 3. Data Splitting & Preprocessing  
**_Status: In Progress_**

- Train-test split (chronological or random)
- Imputation, encoding, and scaling within a pipeline
- Outlier correction (if needed)

---

## 4. Feature Selection & Engineering  
**_Status: In Progress_**

- Identify most predictive variables
- Add new features (e.g., price per square meter, time since last sale)
- Reduce multicollinearity

---

## 5. Model Selection & Training  
**_Status: In Progress_**

- Compare baseline models (Linear Regression, Decision Tree)
- Tune and evaluate ensemble models (Random Forest, XGBoost)

---

## 6. Evaluation & Validation  
**_Status: In Progress_**

- Metrics: MAE, RMSE, R²
- Cross-validation strategies
- Visualizations: predictions vs. actuals

---

## 7. Model Interpretation  
**_Status: In Progress_**

- Feature importances
- Model diagnostics

---

## What's Next?

The modeling and evaluation phases are actively being developed. In the meantime, feel free to explore the `data_preparation.ipynb` to see the full depth of real-world data wrangling already completed.

Stay tuned for updates!
