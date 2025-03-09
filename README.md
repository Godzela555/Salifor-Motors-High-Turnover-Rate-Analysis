# Salifort Motors Employee Turnover Analysis & Predictive Modeling Project: Unveiling Root Causes and Driving Actionable Retention Strategies

**Project Goal:**  To conduct a rigorous analysis of employee attrition at Salifort Motors, not just to predict turnover, but to **identify the *root causes* driving employee departures** and to develop a predictive model that can be used thoughtfully by HR to enable truly effective, proactive interventions.

**Business Problem:**  Salifort Motors faces a significant and costly problem: **high employee turnover**.  The need is urgent to understand **"What's *really* making our employees leave?"** to move beyond surface-level observations and implement impactful solutions.  The traditional approach to hiring and replacing departing staff is proving inefficient and expensive.

**Project Objective:**  This project goes beyond simple prediction. The key objectives are:

*   **Deep Root Cause Analysis:** To move beyond surface-level correlations and uncover the underlying drivers of employee turnover at Salifort Motors.
*   **Predictive Model Development & Strategic Model Selection:** To build predictive models with high accuracy, but also to critically evaluate models based on their ability to inform *actionable* insights – even considering models that may have slightly lower scores but offer more robust root cause interpretability.
*   **Actionable & Targeted Recommendations:** To deliver a comprehensive set of HR strategies, grounded in data and predictive insights, designed to directly address the root causes of turnover and dramatically improve employee retention.

## Project Overview & Methodology: From Data to Deep Understanding

This project employed a rigorous, multi-stage methodology combining exploratory analysis with advanced predictive modeling and a focus on actionable business implications:

1.  **Comprehensive Exploratory Data Analysis (EDA):**  Went beyond simple visualization to conduct a detailed investigation of the dataset, seeking to uncover not just *patterns*, but the *stories* behind the data. EDA focused on features such as:
    * **Employee Experience Metrics:** Satisfaction Level, Last Evaluation, Time Spent at Company, Average Monthly Hours
    * **Work & Performance Factors:** Number of Projects, Work Accidents
    * **Compensation & Career Factors:** Salary, Promotion Last 5 Years
    * **Organizational Context:** Department

2.  **Root Cause Hypothesis Development (Data-Driven):**  EDA was not just descriptive. It was used to develop specific hypotheses about the *chronological flow* of factors leading to turnover, specifically linking workload, evaluation, satisfaction, and compensation perceptions over employee tenure.

3.  **Predictive Modeling - A Strategic Choice:**  Multiple machine learning models were developed, including Logistic Regression, Random Forest, and XGBoost. However, the project critically considered **model selection beyond just top scores.**  The analysis explicitly addressed the trade-off:

    *   **"Champion Model" (e.g., tuned XGBoost with Satisfaction):**  Highest predictive accuracy but includes 'Satisfaction Level' as a feature –  acknowledged as potentially a *result* rather than a direct root cause, making it best for *predictive accuracy when satisfaction data is available*.
    *   **"Root Cause Focused Model" (e.g., Random Forest or Logistic Regression without Satisfaction):**  Potentially slightly lower scores but deliberately excluded Satisfaction Level to focus on **predicting turnover from *upstream factors***, enabling interventions at the root cause. Feature importance analysis was crucial here.

4.  **Feature Importance Interpretation - Unveiling the Strategic Compass:**  Feature importance analysis wasn't just for model understanding, but served as a **strategic compass for HR action.** It was used to quantify the influence of various factors and directly prioritize areas for HR intervention, ensuring recommendations were data-validated and targeted at the most impactful levers.

5.  **Actionable & Prioritized Recommendations – Data-Driven HR Strategy:** Recommendations weren't generic HR advice. They were meticulously crafted and prioritized **directly from the EDA insights, feature importance findings, and the root cause hypotheses.** The recommendations form a cohesive, data-driven strategy for Salifort Motors to tackle its turnover problem at its source.

## Key Insights & Findings: Beyond the Symptoms to the Root of the Problem

This project delved deeper than surface-level correlations, uncovering key insights about the underlying drivers of turnover:

*   **Number of Projects: The Crucial Root Cause Driver:** The analysis points to **Number of Projects** as a pivotal, and potentially manageable, root cause factor.
    *   **Overwork Cycle:** Increased Projects -> Increased Average Monthly Hours -> Higher Last Evaluation -> *Perception of Insufficient Reward/Growth for Effort* -> Lower Satisfaction -> Turnover
    *   **Under-Engagement Cycle:** Decreased Projects -> Decreased Average Monthly Hours -> Lower Last Evaluation -> *Perceived Lack of Challenge/Engagement* -> Lower Satisfaction -> Turnover
*   **Employee Satisfaction: The Barometer, Not the Root:**  Confirmed that **Satisfaction Level** is the strongest *predictor*, but crucially, recognized it as often a *result* or a symptom of underlying workload imbalances, compensation concerns, and limited growth opportunities (as outlined in the Project Cycle hypotheses).
*   **The Critical Mid-Tenure Dip (Years 3-5):** Reinforces the distinct turnover lifecycle, emphasizing the urgent need to address employee experience and progression during these critical years.
*   **(Further insights on Workload Imbalance, Compensation Concerns, Attrition at Both Performance Extremes, Limited Promotions, Departmental Variations, and Work Accident Paradox - as previously detailed, but now framed within the Root Cause narrative).**

## Strategic Model Selection: Accuracy vs. Actionability – Choosing the Right Tool for HR

A key element of this project is the explicit consideration of **strategic model selection.** While a "Champion Model" (with Satisfaction) offered peak prediction accuracy, the project recognized that **a "Root Cause Focused Model" (without Satisfaction)**, despite potentially slightly lower scores, offers greater *actionability* for Salifort Motors HR.

**Model Recommendation Rationale:**

*   **For Immediate Prediction & Risk Monitoring (if Satisfaction Data is available in advance):** The **"Champion Model" (XGBoost with Satisfaction)** is recommended for deployment. It will provide the most accurate near-term prediction of employee attrition *when* satisfaction level data is available and up-to-date. This model can be invaluable for proactive risk identification and triggering timely interventions.

*   **For Long-Term Strategic HR Planning & Root Cause Intervention (even without immediate Satisfaction data):**  The **"Root Cause Focused Model" (Random Forest or Logistic Regression *without* Satisfaction)** is strategically more valuable for understanding and addressing the *underlying causes* of turnover. By focusing on upstream features (Project Load, Work Hours, Evaluation, Tenure, Compensation), this model informs long-term HR strategies designed to *prevent* dissatisfaction in the first place.  Feature importances from this model are particularly crucial for guiding HR strategy.

**This project emphasizes that the "best" model is not solely defined by its score, but by its strategic fit for the specific business objective and its ability to drive meaningful and sustainable HR action.**

## Key Recommendations for Salifort Motors HR: A Data-Driven Retention Strategy

Based on the analysis, Salifort Motors HR should prioritize the following recommendations:

*   **Prioritize Proactive Satisfaction Measurement and Actionable Feedback Loops**
*   **Re-Engineer Workload Distribution & Implement Project Portfolio Management for Balance**
*   **Revamp Compensation Structures for Market Competitiveness & Transparent Progression**
*   **Expand Promotion Pathways and Implement Fair & Transparent Processes**
*   **Elevate Employee Well-being, Safety & Reduce Workload-Related Pressures**
*   **Tailor Departmental Retention Strategies to Address Unique Contexts**
*   **Conduct Qualitative Research to Deepen Understanding of Satisfaction Drivers & Work Accident Paradox**
*   **Focus Mid-Tenure Retention Programs for Years 3-5**

_(Refer to full project notebook and detailed documentation for comprehensive recommendation descriptions)._

## Model Performance Highlights
*   **Top Performing Models:**  XGBoost and Random Forest (tuned and upsampled).
*   **High Accuracy:**  ~98.5% - 98.7%
*   **F1-Score:** ~0.95 - 0.96
*   **AUC:** ~0.96 - 0.97

## Potential Next Steps & Model Utilization (Real-World Implementation)

For real-world application, the developed predictive models could be integrated into Salifort Motors' HR systems to:

*   **Enable real-time attrition risk monitoring of current employees.**
*   **Trigger automated alerts for proactive HR interventions.**
*   **Support data-driven decision-making in retention strategy development and resource allocation.**

## Limitations & Further Considerations
*   This analysis is based on a specific dataset and its timeframe.
*   The model is limited by the features available in the dataset (external factors and more nuanced workplace dynamics are not directly captured).
*   Employee Satisfaction, while a strong predictor, acts as a proxy for underlying root causes (workload, compensation, career opportunities). Further qualitative research is recommended.
*   The paradoxical finding related to work accidents requires further investigation to understand the underlying dynamics.

Further research could explore longitudinal data, incorporate qualitative data, integrate external economic indicators, and refine dynamic predictive models for continuous improvement in employee retention strategies.

## Skills Demonstrated

This project showcases skills in:

*   **Data Exploration and Visualization (Python - Pandas, Matplotlib, Seaborn)**
*   **Statistical Analysis and Hypothesis Testing**
*   **Feature Engineering and Data Preprocessing**
*   **Predictive Modeling (Machine Learning - Scikit-learn, XGBoost)**
*   **Model Evaluation and Hyperparameter Tuning**
*   **Feature Importance Interpretation**
*   **Business Insight Generation from Data Analysis**
*   **Formulating Actionable Recommendations for Business Problems**
*   **Communicating Technical Findings to a Business Audience**

## Repository Contents

*   `[Project Notebook Name(s)].ipynb`:  Jupyter Notebook(s) containing the complete end-to-end analysis, including EDA, modeling, and insight generation.
*   `data/`: Directory containing the dataset used for analysis (e.g., `employee_turnover.csv`).
*   `[Presentation File (Optional) e.g., Salifort_Motors_Turnover_Analysis.pdf]`: (Optional) Presentation slides summarizing key findings and recommendations.
*   `README.md`:  This file, providing an overview of the project.

## How to Run the Project

1.  Clone this repository to your local machine.
2.  Ensure you have Python 3.x installed along with the necessary libraries (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost). You can install them using `pip install -r requirements.txt` (if you include a `requirements.txt` file listing dependencies).
3.  Open and run the Jupyter Notebook(s) (`[Project Notebook Name(s)].ipynb`) to reproduce the analysis.
4.  The dataset (`employee_turnover.csv`) is included in the `data/` directory.

## Contact

Ratthana Tongtan - ratthana_tongtan@hotmail.com or https://www.linkedin.com/in/ratthana-t/

---
