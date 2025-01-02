# Churn Prediction Report

## Objective:
The aim of this project is to predict user churn based on user event data, utilizing concepts from a research paper and implementing robust machine learning models.

## Process Overview:
1. **Data Inspection & Preprocessing:**
   - Loaded data and inspected its structure.
   - Handled missing, duplicate, and inconsistent entries.
   - Parsed timestamps and ensured correct data types.

2. **Exploratory Data Analysis (EDA):**
   - Analyzed event distributions over time.
   - Examined brand and category popularity.
   - Summarized user-level data such as total spend, visit frequency, and time between visits.

3. **Defining Churn:**
   - Churn was defined as no activity or purchase over a threshold period.

4. **Feature Engineering:**
   - Created features capturing user behavior patterns, such as frequency of specific events (views, carts, purchases).
   - Extracted categorical insights from popular categories and brands.
   - Used aggregation methods to summarize user activity over time.

5. **Modeling:**
   - Applied Logistic Regression and Random Forest models.
   - Used OneHotEncoding for categorical variables.
   - Split the data into training and testing sets (80-20 split).
   - Evaluated models using metrics like Precision, Recall, F1 score, and ROC-AUC.

## Results:
- The Random Forest model achieved the best performance with high Recall and Precision.
- Feature importance analysis highlighted that 'frequency of purchases' and 'time since last purchase' were key indicators of churn.

## Recommendations:
- Users identified at high risk of churn should be targeted with personalized offers or engagement strategies.
- Implement time-sensitive reminders for users inactive for extended periods.

## Final Metrics:
- **Precision:** 0.89  
- **Recall:** 0.83  
- **F1-Score:** 0.86  
- **ROC-AUC:** 0.92
