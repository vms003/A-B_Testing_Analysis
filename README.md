# A/B Testing Case Study

## 📋 Overview
This project analyzes the effectiveness of marketing campaigns using A/B testing methodology. The primary focus is to evaluate whether the campaign succeeded and quantify the impact of advertisements on conversions.

### Objectives:
- **Determine Campaign Success:** Evaluate the overall performance of the marketing campaign.
- **Quantify Ad Impact:** Understand how much success can be attributed to advertisements.
- **Provide Actionable Insights:** Derive meaningful conclusions for business decisions.

---

## 🗂️ Project Structure

### Main Files:
- **`A_B_testing_dashboard.pbix`**: Interactive Power BI dashboard with campaign insights.
- **`ab_analysis.ipynb`**: Python notebook for data analysis, hypothesis testing, and modeling.
- **`A_B_Testing_ppt.pptx`**: Presentation summarizing findings and recommendations.
- **`marketing_AB.csv`**: Dataset used for analysis.

### Folders:
- **Dashboard/**: Contains the Power BI dashboard.
- **Plots/**: Stores visualizations generated during analysis.
- **Slides/**: Includes the presentation slides summarizing findings.

---

## 📊 Dataset Description

### Data Fields:
| Field Name      | Description                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| `Index`         | Row index.                                                                |
| `user id`       | Unique identifier for each user.                                           |
| `test group`    | Group assignment (`ad` for experimental group, `psa` for control group).   |
| `converted`     | Conversion status (1 = Purchased, 0 = Not Purchased).                      |
| `total ads`     | Number of ads seen by the user.                                            |
| `most ads day`  | Day of the week when the user saw the most ads.                            |
| `most ads hour` | Hour of the day when the user saw the most ads.                            |

---

## 🛠️ Methodology

### 1. Data Preprocessing
- Converted `converted` to binary format.
- Categorized `most ads day` for easier analysis.

### 2. Exploratory Data Analysis (EDA)
- **Conversion Rates:** Analyzed and visualized conversion rates by test groups.
- **Ad Effectiveness:** Explored the distribution of ads and their influence on conversions.

### 3. Hypothesis Testing
- **Chi-Square Test:** Tested statistical significance of conversion rate differences.
- **T-Test:** Compared total ads between groups.

### 4. Segmentation Analysis
- **Day-Based Insights:** Analyzed conversion rates by the day of the week.
- **Hour-Based Insights:** Explored conversion rates by the hour of the day.

### 5. Predictive Modeling
- **Model Used:** Random Forest Classifier.
- **Goal:** Predict likelihood of user conversion based on ads data.
- **Evaluation Metrics:** Classification report and ROC AUC score.

### 6. Interaction Effects
- Explored interaction between `total ads` and `most ads hour` using logistic regression.

### 7. Incrementality Testing
- **Incremental Lift:** Measured the added benefit of ads over the control group.

---

## 🔍 Key Insights

1. **Conversion Rates:** Experimental group (`ad`) achieved higher conversion rates compared to the control group (`psa`).
2. **Ad Impact:** Incremental lift highlights the direct contribution of ads to conversions.
3. **Optimal Segments:** Certain days and hours drive significantly higher conversions, offering targeting opportunities.
4. **Predictive Power:** Random Forest model provides reliable predictions for user conversions.
5. **Interaction Effects:** Ads shown at specific times have a higher likelihood of driving conversions.

---

## ⚙️ Tools & Requirements

### Python Libraries:
- `numpy`, `pandas`, `matplotlib`, `seaborn`, `scipy`, `sklearn`, `statsmodels`

### Additional Tools:
- Power BI

---

## 🚀 How to Use

### Steps to Explore:
1. **Data Analysis**:
   - Open `ab_analysis.ipynb` to review data cleaning, EDA, hypothesis testing, and predictive modeling.
2. **Dashboard**:
   - Open `A_B_testing_dashboard.pbix` in Power BI to view interactive visualizations.
3. **Presentation**:
   - Use `A_B_Testing_ppt.pptx` for a summarized view of the project.

---

## 🌟 Conclusion
This A/B testing project showcases the value of data-driven decision-making in marketing. By analyzing conversion rates, testing hypotheses, and building predictive models, we deliver actionable insights to improve campaign strategies and optimize advertising efforts.

---

## 👤 Author
**Viraj Suthar**

📧 [Email Me](mailto:virajsuthar2003@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/viraj-suthar-517445333/)

---

### 📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

