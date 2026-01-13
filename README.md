# 📰 Online News Popularity Prediction
> **Selected as an Outstanding Project** in the Pattern Recognition course at Ewha Womans University.

This project focuses on predicting the "virality" of online news articles (whether an article exceeds 1,400 shares) by analyzing various features of the content. Our team achieved high predictive performance through advanced data preprocessing and ensemble modeling.

## 🏆 Achievement
- **Selected as a Top Project**: Recognized for excellence in methodology and analysis within the Pattern Recognition course, followed by an official class presentation.

## 👥 Team Members (Team 5)
- Doyoon Kim, Minha Woo, Yeeun Kim, Jiwon Lee

## 🎯 Project Objective
- **Goal**: Build a binary classification model to predict news popularity.
- **Target Variable**: `y=1` (Popular, >1,400 shares), `y=0` (Not popular)
- **Dataset**: 22,200 samples with 46 features (approx. 10% missing values).

## 🛠️ Key Workflow & Technical Strengths

### 1. Advanced Data Preprocessing
- **Regression-based Imputation**: Instead of simple mean/median filling, we performed **Linear/Polynomial Regression** to impute missing values for highly correlated variable pairs (r > 0.7).
- **Outlier Handling with DBSCAN**: Utilized **Density-Based Spatial Clustering (DBSCAN)** to identify and handle outliers in high-dimensional spaces, improving model robustness.
- **Feature Engineering**: Applied **Log Transformation** to skewed numerical data and utilized **StandardScaler** for normalization.

### 2. Modeling & Evaluation
- **Algorithm Exploration**: Evaluated multiple models including Logistic Regression, Random Forest, XGBoost, CatBoost, and LightGBM.
- **Final Model**: Developed a **Stacking Ensemble** (Meta Model: Logistic Regression) to maximize predictive accuracy.
- **Performance**: Achieved a final **Mean Score of 0.6955**.

## 📂 Project Structure
- **[FINAL CODES](./FINAL%20CODES)**: Final Python source code for preprocessing and modeling (`code.ipynb`).
- **[REPORTS](./REPORTS)**: Detailed project report and presentation slides (`report.pdf`, `PPT.pdf`).

## 📈 Key Visuals
*(I recommend inserting the following images here for maximum impact)*
1. **DBSCAN Clustering Plot**: To showcase your advanced outlier detection skills.
2. **Correlation Heatmap**: To justify your regression-based imputation strategy.
3. **Model Performance Comparison**: To highlight the superiority of the Stacking model.
