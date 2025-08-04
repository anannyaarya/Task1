# Task 1: Data Cleaning & Preprocessing – Titanic Dataset

## Internship Task Overview
This repository contains the solution to **Task 1** of the AI & ML Internship, focused on **data cleaning and preprocessing** using the Titanic dataset. The goal was to transform raw data into a clean and machine-learning-ready format.

## Task Objectives
- Identify and handle missing values
- Convert categorical data into numerical form
- Normalize and scale numerical features
- Detect and remove outliers
- Export the cleaned dataset for ML use

## Technologies Used
- **Python**
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn

## Key Steps Performed
1. **Exploratory Data Analysis (EDA)**  
   - Used `.info()`, `.describe()`, `.isnull().sum()` to explore the data

2. **Handling Missing Values**  
   - Filled `Age` with **median**  
   - Filled `Embarked` with **mode**  
   - Dropped `Cabin` column due to excessive nulls

3. **Encoding Categorical Variables**  
   - Applied `LabelEncoder` for `Sex`  
   - Applied `OneHotEncoding` for `Embarked`

4. **Feature Scaling**  
   - Used `StandardScaler` on `Age` and `Fare`

5. **Outlier Detection & Removal**  
   - Visualized outliers using **boxplots**  
   - Removed `Fare` outliers using **IQR method**

6. **Exported Final Cleaned Dataset**  
   - Saved cleaned data to `titanic_cleaned.csv`


## Repository Structure
Task-1
- Titanic-Dataset.csv # Original dataset
- titanic_cleaned.csv # Cleaned dataset
- Task1.ipynb # Complete code notebook
- boxplot_outliers.png # Outlier visualization
- README.md # Task summary and steps

The data is now cleaned, scaled, and ready to be used for training classification or regression ML models such as Logistic Regression, SVMs, or Decision Trees.
This task built a strong foundation in data cleaning and preprocessing, which is essential for real-world machine learning pipelines.
