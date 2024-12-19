# 🚗 How Driving Scenarios Affect the Choice of In-Vehicle Coupons

Welcome to our project repository! This work explores how various driving scenarios and user demographics influence the acceptance of in-vehicle coupons. The analysis is based on the **In-Vehicle Coupon Recommendation Dataset** from the UCI Machine Learning Repository.

---

## 📖 Introduction

In the modern marketing landscape, coupons play a significant role in influencing consumer behavior. This project investigates the factors driving coupon acceptance, including demographic, environmental, and behavioral variables, using a structured dataset obtained through surveys on Amazon Mechanical Turk.

The primary goal is to predict the likelihood of a user accepting a coupon based on these factors, leveraging machine learning models for actionable insights.

---

## ❓ Problem Statement

We aim to address the following research questions:
1. How do demographic factors (e.g., occupation, gender, education) affect coupon acceptance?
2. What environmental conditions (e.g., weather, time of day) impact coupon redemption?
3. How do driving scenarios (e.g., travel distance, trip purpose) influence user behavior?

---

## 📊 Dataset

The dataset contains **26 features** and **12,684 records**, providing detailed information about users, their demographics, and driving scenarios.  
**Dataset Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/603/in+vehicle+coupon+recommendation).  
For detailed descriptions of features, refer to the `data_dictionary.md` file in this repository.

### Key Features:
- **Demographic**: Gender, age, occupation, marital status, education level.  
- **Environmental**: Weather, temperature, time of day.  
- **Behavioral**: Destination type, passenger type, coupon type, distance to the coupon location.  

---

## 🔍 Exploratory Data Analysis (EDA)

Key insights from the dataset:
- **Destination**: "No Urgent Place" was the most common trip purpose.
- **Weather**: Most users drove on sunny days.
- **Coupon Types**: Coffee House coupons were most popular.
- **Acceptance Rate**: Approximately 57% of coupons were accepted.

Visualizations, descriptive statistics, and feature engineering steps can be found in the `eda/` folder.

---

## ⚙️ Methodology

### 1. **Feature Engineering**
- One-hot encoding for categorical variables.
- Normalization of numerical features.
- Correlation analysis to select top 10 impactful features.

### 2. **Machine Learning Models**
We implemented and compared the following models:
- **Decision Tree**: Best performance with 68.86% accuracy on the test set.
- **Logistic Regression**: Effective for linear relationships.
- **K-Nearest Neighbors (KNN)**: Non-parametric approach with moderate results.

### 3. **Model Evaluation**
Metrics used:
- Accuracy
- Precision
- Recall
- F1 Score  

Evaluation results can be found in the `models/` folder.

---

## 💡 Key Findings
1. Decision Tree was the most effective model, achieving:
   - **Accuracy**: 68.86%
   - **Precision**: 68%
   - **Recall**: 75%
2. Sunny weather and shorter travel distances positively influenced coupon acceptance.
3. Demographic factors like age and occupation significantly impacted user behavior.

---

## 📂 Repository Structure
