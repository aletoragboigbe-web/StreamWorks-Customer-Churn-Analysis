# 🚀StreamWorks-Customer-Churn-Analysis
## Analyzes customer churn for a video streaming platform using Python, statistical analysis, and machine learning to uncover retention drivers and actionable business insights.
### 🎯 Business Goal
StreamWorks Media is a UK-based video streaming platform operating in a highly competitive market alongside global players such as Netflix and Amazon Prime. As customer acquisition costs continue to rise, retaining existing subscribers has become a critical business priority.
The purpose of this analysis is to understand why customers churn, identify early warning signals, and provide data-driven insights to support targeted retention strategies.

The primary business goals of this project are:
- Understand churn patterns and customer behaviour
- Identify factors influencing subscription cancellation
- Predict churn probability to enable early intervention
- Analyze revenue impacting behaviors such as watch time and tenure

### 🧩 Business Problem
StreamWorks Media faces increasing customer churn, which directly impacts recurring revenue and growth. Without understanding the behavioural and engagement drivers behind churn, retention efforts remain reactive rather than proactive.
This project aims to use customer data to uncover churn drivers and build predictive models that support smarter, earlier retention decisions.

### 🗂 Dataset Overview
The dataset contains anonymized user-level subscription and engagement data, including:
- Demographics such as age, gender, and country
- Subscription details, including plan type and monthly fee
- Engagement metrics such as average watch hours and mobile usage
- Marketing indicators such as promotions and referrals
- Churn indicator showing whether a user cancelled their subscription
The dataset represents a mix of active and churned users across multiple regions.
### 🎯 Purpose of the Analysis
The purpose of this analysis is to:
- Explore patterns and behaviours linked to customer churn
- Quantify the impact of engagement and tenure on churn likelihood
- Build predictive models to estimate churn probability
- Translate analytical findings into clear business recommendations
This project is designed to support non-technical decision-makers with actionable insights.

### 🛠 Tools & Technologies
- Python
- Pandas and NumPy for data manipulation
- Matplotlib and Seaborn for visualization
- Scikit-learn for machine learning model
- SciPy for statistical testing
- Jupyter Notebook for analysis and documentation

### 🧹 Data Cleaning Summary
The dataset required several preparation steps before analysis:
- Converted date columns to proper datetime format
- Created tenure_days from signup and last active dates
- Handled missing values by:
    - Filling numeric columns with median values
    - Filling categorical columns with "Unknown"
- Ensured churn labels were converted into binary format
- Verified data types and removed inconsistencies
- The following data cleaning steps were performed:
<img width="571" height="563" alt="Screenshot 2026-02-06 153402" src="https://github.com/user-attachments/assets/26630a1d-40b9-421e-82ed-894978865129" />

### 🧠 Feature Engineering Summary
New features were created to capture customer behaviour better:
- tenure_days: Number of days a user stayed active
- is_loyal: Flag indicating users with tenure greater than 180 days
- watch_per_fee_ratio: Engagement value relative to subscription cost
- heavy_mobile_user: Identifies users who predominantly watch on mobile
- Encoded categorical variables for modelling
These features helped capture user engagement and loyalty more effectively.

### 📈 Key Findings (i Statistical Analysis)
Statistical tests were used to validate behavioural differences between churned and retained users:
- Chi-square tests showed that:
o	Users who received promotions churned less
o	Referred users had lower churn rates
- T-tests revealed that:
o	Retained users had significantly higher average watch time
- Correlation analysis showed:
o	Strong negative relationships between churn and both tenure and watch time
Image placeholder:
📷 Add boxplot or bar chart comparing churn vs watch time or promotions

### ii Statistical Analysis
Correlation Analysis
<img width="1301" height="887" alt="Screenshot 2025-10-21 063004" src="https://github.com/user-attachments/assets/246f81e6-6fea-4317-9cea-f5498d237c0a" />
The correlation analysis reveals strong relationships between engagement metrics. Watch time and tenure show a strong positive correlation, while watch time has a negative relationship with churn. This indicates that lower engagement is a strong warning signal for cancellation.

<img width="959" height="565" alt="Screenshot 2025-10-21 080407" src="https://github.com/user-attachments/assets/e9a4db45-2f0e-447e-9edc-92d32176ddfd" />

<img width="894" height="645" alt="Screenshot 2025-10-21 080504" src="https://github.com/user-attachments/assets/2326ab77-4518-4022-9f26-c2a066089769" />

### 🤖 Predictive Modelling Summary
Logistic Regression (Churn Prediction)
- Successfully classified churned vs retained users
- Strong performance based on accuracy, F1 score, and AUC
- Most influential churn predictors:
1.	Average watch time
2.	Tenure duration
3.	Receipt of promotions
Image placeholder:
### 📷 Add ROC curve image here
<img width="912" height="585" alt="Screenshot 2025-10-21 081155" src="https://github.com/user-attachments/assets/179eafee-5d17-4c36-a19b-971bf0ca89c7" />

Linear Regression (Tenure Prediction)
- Used to understand factors affecting customer loyalty
- Showed that:
o	Higher watch time increases tenure
o	Premium subscription users tend to stay longer
o	Promotions positively impact customer longevity

### 📷 Add residual plot or predicted vs actual plot here
<img width="894" height="645" alt="Screenshot 2025-10-21 080504" src="https://github.com/user-attachments/assets/38c55df2-32a2-40ba-a552-ae395664cefc" />

### 📌 Interpretation of Results
The analysis shows that customer engagement is the strongest driver of retention. Users who watch more content and remain active longer are significantly less likely to churn.
Promotions and referrals act as effective retention tools, especially for new users. Mobile-heavy users show slightly higher churn risk, suggesting potential experience or usability challenges.

### 🧠 Key Takeaways 
- Demonstrates end-to-end data analysis workflow
- Combines statistics, machine learning, and business reasoning
- Focuses on real-world subscription and retention challenges
- Translates technical outputs into business actions
- Communicates insights clearly to non-technical stakeholders

