# Asset-Trade-In-Probability
# ⏳ Predicting Asset Trade-In Probability with Survival Analysis

**Author:** Brandy Horne  
**Tags:** Survival Analysis, Cox Proportional Hazards, Kaplan-Meier, Tableau, Predictive Modeling, CRISP-DM

---

## 🎯 The Business Problem

In industries where assets have long operational lifespans, predicting *when* a customer is likely to return or trade in a product can drive powerful logistics and pricing strategies. This project focused on forecasting **the probability of commercial asset trade-ins** over a 24-month period using survival analysis.

The objective was to support **planning and pricing teams** with visibility into expected return timelines—reducing idle inventory, improving resale strategy, and aligning operations with customer behavior.

---

## 🔍 Business & Domain Understanding

To begin, I investigated key factors influencing asset trade-in behavior:

- **Operational cycles:** mileage thresholds, wear-and-tear expectations
- **Contractual triggers:** lease ends, incentives, service renewals
- **Customer segments:** regional usage, company size, historical trade behavior

The outcome needed to be explainable, actionable, and integrated into strategic forecasting discussions.

---

## 🧠 Data Understanding

I aggregated data across several internal sources, including:

- **Asset attributes:** age, mileage, service history, model type
- **Customer profiles:** industry, usage patterns, geographic distribution
- **Historical trade-ins:** event timing, frequency, and return conditions

Key metrics included asset age at return, usage intensity, and external economic indicators tied to replacement cycles.

---

## 🧹 Data Preparation

I transformed the dataset into a **time-to-event structure**, labeling trade-in events as binary outcomes and censored records where applicable.

- Cleaned and normalized features
- Removed anomalies and inconsistent return dates
- Created derived variables (e.g., mileage per year, service frequency)
- Encoded categorical variables for modeling inputs

---

## 🔬 Modeling

### Kaplan-Meier Estimator
Used as an exploratory tool to visualize survival curves across customer and asset segments.

- Estimated overall survival function (i.e., probability of not trading in)
- Compared survival rates across asset types and usage groups

### Cox Proportional Hazards Model
Selected for its interpretability and ability to handle censored data.

- Modeled hazard ratios to quantify the influence of features on trade-in likelihood
- Validated proportional hazards assumptions
- Optimized for simplicity and business relevance

---

## 📊 Evaluation

- Evaluated model fit using log-likelihood and concordance index (C-index)
- Conducted stratified visual validation with KM overlays
- Sensitivity tested variable inclusion and cohort consistency

---

## 📈 Deployment

I deployed the insights into a **Tableau dashboard** for executive leadership and planners:

- Interactive filters by asset class, geography, and customer profile
- Quarterly updates with trade-in probability curves and segment summaries
- Integrated alerts for assets entering high-risk return windows

Monthly insights were presented to leadership, driving actionable pricing and logistics interventions.

---

## ✅ Results

- Improved visibility into expected asset return timing
- Enabled proactive pricing strategy adjustments based on churn risk
- Informed logistics resource planning with high-risk return cohorts

---

## 🛠️ Tools Used

- **Languages:** Python, SQL  
- **Libraries:** Lifelines, pandas, NumPy, Seaborn, Matplotlib  
- **Visualization:** Tableau  
- **Techniques:** Kaplan-Meier, Cox PH, censoring, hazard modeling

---

## 💡 Key Takeaways

1. Survival analysis offers interpretable, business-aligned predictions for time-based events.
2. Proper data structuring and variable engineering are crucial for event modeling.
3. Executive dashboards can translate statistical models into strategic foresight.

---

**Contact:**  
[GitHub](https://github.com/brandyanalytics) | [LinkedIn](https://linkedin.com/in/brandyhorne01) | Brandyhorne01@gmail.com  
