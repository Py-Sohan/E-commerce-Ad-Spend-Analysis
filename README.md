# E-commerce Ad Spend Analysis: Optimizing Ad Spend for Higher Conversion Rates
![image](https://github.com/user-attachments/assets/ba11c2d4-c2a5-481a-a3dd-110e0553200f)



## 📁 Project Overview

In this project, we conduct a detailed statistical analysis on an online advertisement dataset.  
Our goal is to determine whether **ad spend** and **conversion rates** differ significantly between **holidays** and **non-holidays**.  
Through hypothesis testing, data visualization, and correlation analysis, we generate actionable insights for better marketing budget allocation.

---

## 📊 Dataset Description

| Column Name    | Description                                   |
|----------------|-----------------------------------------------|
| `timestamp`    | Date of the data record                       |
| `page_views`   | Number of page views on that day              |
| `ad_spend`     | Amount spent on ads on that day               |
| `is_weekend`   | Boolean indicating if the day is a weekend    |
| `day_of_week`  | Name of the day (e.g., Monday, Tuesday)       |
| `is_holiday`   | Boolean indicating if the day is a holiday    |
| `conversion_rate` | page_views divided by ad_spend (feature engineering) |

---

## ❓ Hypothesis Testing Problem

### Research Question
> Is there a statistically significant difference in conversion rates between holidays and non-holidays?

---

## 🧠 Hypothesis Testing Approach

### 📏 Normality Test
- **Null Hypothesis (H₀):** Data is normally distributed.
- **Alternative Hypothesis (H₁):** Data is not normally distributed.

**Results:**
- Holiday Data: Normally distributed.
- Non-Holiday Data: Not normally distributed.

### 🧪 Variance Homogeneity Test
- **Null Hypothesis (H₀):** Variances of both groups are equal.
- **Alternative Hypothesis (H₁):** Variances of both groups are different.

**Result:**
- Variances are different (p-value: 0.0062).

### 🧪 Non-Parametric Test (Mann-Whitney U Test)
Due to non-normality and unequal variance, we use the Mann-Whitney U Test.

**Results:**
- U-Statistic: 1568.0
- P-Value: 6.01e-06

**Interpretation:**
- **Reject the null hypothesis.**
- There is a statistically significant difference in conversion rates between holidays and non-holidays.

---

## 📈 Data Visualization

- Box plots comparing ad spend and conversion rates between holidays and non-holidays.
- Statistical summaries for both groups.
- Correlation plots for conversion rates and ad spend.

---

## 🔗 Correlation Analysis

### Holiday Period
- **Correlation between ad spend and conversion rate:** -0.951
- Strong negative correlation: Higher ad spend tends to lower conversion rates during holidays.

### Non-Holiday Period
- **Correlation between ad spend and conversion rate:** -0.725
- Moderate negative correlation during non-holidays.

---

## 📌 Conclusion and Recommendations

### 📋 Summary
- Average ad spend is higher during holidays ($397.91) compared to non-holidays ($247.88).
- Conversion rates are lower during holidays (mean: 4.23) compared to non-holidays (mean: 6.71).
- A statistically significant difference exists in conversion rates.
- Stronger negative correlation between ad spend and conversion rate during holidays.

### 🛠️ Recommendations
- **Optimize ad spend during holidays** to avoid reduced efficiency in conversion rates.
- **Focus more ad budget during non-holidays** where conversion rates are stronger.
- **Monitor ad performance closely** during festive seasons and adjust bids dynamically.

---

## 📚 Skills and Tools Demonstrated

- Python (Pandas, Scipy, Seaborn, Matplotlib)
- Hypothesis Testing (Shapiro-Wilk Test, Levene's Test, Mann-Whitney U Test)
- Exploratory Data Analysis (EDA)
- Feature Engineering (Conversion Rate Calculation)
- Data Visualization
- Business Strategy and Data-Driven Decision Making

---

# 📞 Let's Connect!

- [LinkedIn](https://www.linkedin.com/in/lutfor-rahman-sohan/)

