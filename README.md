## 📌 Week 6: Advanced Analytics, Dashboard Optimization & Cross-Track Integration

### 🎯 Objective
Transition exploratory analysis into advanced segmentation, refine key operational KPIs inside an interactive Power BI dashboard, and execute cross-track data alignment with the Data Science team.

---

### 📊 Dashboard & KPI Suite
* **No-Show Rate:** `48.5%` (Baseline operational drop-off)
* **Attendance Rate:** `46.3%` (Realized clinic capacity)
* **Total Wasted Capacity:** `53.7%` (No-shows + Late Cancellations)
* **Lost Capacity Hours:** `1,210 Hours` (Based on 30-min appointment slots)
* **Top Channel Outcome (SMS):** `45.8%` (vs. 51.4% unreminded slots)

---

### 🔎 Key Analytical Insights
1. **Compounding Friction Cluster:** Patients residing **>15 km** away with booking lead times **>14 days** exhibit non-attendance rates ranging from **44.2% to 57.0%**.
2. **Age & Transit Barriers:** Elderly cohort ($\ge 65$ years) non-attendance at >10 km is driven primarily by transport logistics rather than forgetfulness.
3. **Chronic Non-Attendance:** Patients with $\ge 2$ past missed appointments account for **36.5%** of overall unutilized slots.

---

### 🤝 Cross-Track Integration (Data Science Collaboration)
* **Data Exchanged:** Shared risk-stratified patient bins (`Distance >15km`, `Lead Time >14 days`), interaction matrices, and correlation outputs.
* **Model Validation:** Data Science validated our segment findings by engineering interaction features in their refined **Gradient Boosting** candidate model, successfully reducing classification false positives from 191 to 175.
* **Handoff Alignment:** Data schema and cleaning pipelines (`HealthConnect_Week6_Analytics_Dataset.csv`) are standardized across Analytics reporting and DS model inputs.

---

### 🛠️ Visual Suite Features
* Dynamic risk slicers (Age Group, Risk Status, Reminder Channel).
* Soft red conditional formatting for high-risk compounding matrix visual.
* Operational **High-Risk Unconfirmed Queue** table visual for targeted administrative phone outreach.
