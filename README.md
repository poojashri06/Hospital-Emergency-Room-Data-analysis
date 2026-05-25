# ER Wait Times & Patient Satisfaction Analysis System

An analytical data framework built in Power BI (`Hospital ER_Data_analysis.pbix`) designed to evaluate, validate, and measure the operational dynamics of a Hospital Emergency Room (ER).

---

## 📋 Executive Summary
Historically, hospital leadership operates under the assumption that patient throughput speed is the definitive driver of patient satisfaction. This framework bridges operational timelines with post-discharge satisfaction metrics to move the organization from an anecdotal management style to an evidence-based, data-driven paradigm.

The primary objective is to investigate the unverified correlation between ER wait times and patient satisfaction, isolating operational bottlenecks, departmental variations, and demographic experience disparities.

---

## ⚠️ Core Problem Statement
> **"Hospital leadership assumes that longer Emergency Room (ER) wait times are the sole driver of declining patient satisfaction scores. However, because operational wait-time metrics (door-to-doctor, rooming delays) have never been programmatically joined with post-discharge satisfaction data, this correlation remains unverified."**

### Strategic Business Risk
Without an analytics framework to validate this assumption, the hospital risks misallocating capital toward accelerating patient throughput (e.g., hiring more triage staff) while potentially ignoring the actual root causes of patient dissatisfaction—such as poor communication during departmental referrals, inequitable care distribution across demographics, or specific facility bottlenecks.

---

## 🗺️ Dashboard Architecture
The Power BI application is structured into four targeted reporting layers to execute this analysis seamlessly:

1. **Page 1: Executive Overview Dashboard** * *Purpose:* High-level KPI monitoring layer for overall throughput and sentiment baselines.
2. **Page 2: Maintaining Patient Satisfaction Dashboard**
   * *Purpose:* Deep-dive statistical analysis looking exclusively at the relationship between wait windows and scores.
3. **Page 3: Admission & Department Referral Analysis**
   * *Purpose:* Granular operational mapping tracking the handoff from the ER to specialized units.
4. **Page 4: Demographic & Equity Overview**
   * *Purpose:* Compliance and equity analysis tracking uniformity of care and experience across all patient populations.

---

## ⚙️ Detailed Analytical Use Cases

### Use Case 1: Testing the Core Wait-Time Correlation
* **Dashboard Mapping:** `Page 1: Overview` & `Page 2: Maintaining Patient Satisfaction`
* **Objective:** To statistically verify whether a direct mathematical relationship exists between how long an ER patient waits and the satisfaction score they submit post-discharge.
* **Primary Actor:** ER Quality Assurance (QA) Director / Healthcare Data Analyst.
* **Data Interaction & Drill-Down:** The user checks baseline high-level KPIs (*Average Total Wait Time* vs *Average Satisfaction Score*), then navigates to the Patient Satisfaction Page to analyze a scatter plot comparing *Wait Time (Minutes)* on the X-axis against *Satisfaction Score (1-10)* on the Y-axis.
* **Analytical Insights:** The system calculates a correlation coefficient. The analyst can filter by low-satisfaction scores to see if those patients actually experienced longer-than-average door-to-doctor times, or if high-wait-time patients still scored the hospital highly due to other hidden factors (e.g., exceptional nursing care or clear communication).

### Use Case 2: Identifying Operational Delays during Departmental Transfers
* **Dashboard Mapping:** `Page 3: Admission & Department Referral Analysis`
* **Objective:** To isolate whether the breakdown in patient satisfaction happens during initial ER triage, or later when a patient is being referred/transferred to a specific specialized department (e.g., Cardiology, Radiology, ICU).
* **Primary Actor:** ER Operations Manager / Chief Medical Officer (CMO).
* **Data Interaction & Drill-Down:** The user interacts with a matrix visual or horizontal funnel chart showing the **"Average Transfer Window"** (the time elapsed between an ER doctor checking a patient and the destination department admitting them).
* **Analytical Insights:** By filtering by specific receiving departments, users can see if certain units (like Radiology Referrals) have low satisfaction scores but short wait times. This proves that the dissatisfaction is likely tied to *quality of care or communication* within that department, rather than a throughput speed issue.

### Use Case 3: Evaluating Demographic Equity and Experience Disparities
* **Dashboard Mapping:** `Page 4: Demographic & Equity Overview`
* **Objective:** To ensure that wait times and corresponding satisfaction trends are uniform across all patient populations, identifying potential biases or structural inequities in ER care delivery.
* **Primary Actor:** Hospital Equity & Compliance Officer / Hospital Administrator.
* **Data Interaction & Drill-Down:** The user segments the ER wait-time and satisfaction data using interactive demographic slicers, specifically: *Age Group, Ethnicity, Gender,* and *Insurance Status* (acting as a socioeconomic indicator).
* **Analytical Insights:** The user cross-references whether specific marginalized demographics systematically experience longer wait times or report lower satisfaction scores compared to the hospital baseline, allowing administrators to deploy targeted cultural competency training or adjust triage protocols.

---

## 📊 Implementation Summary Matrix

| Use Case ID | Target Dashboard Page(s) | Primary User Role | Primary Visual Mechanism | Strategic Goal |
| :--- | :--- | :--- | :--- | :--- |
| **UC-01** | Overview / Satisfaction | QA Director / Analyst | Scatter Plot & R-Value | Prove/disprove wait time assumption |
| **UC-02** | Admission & Referral | Operations Manager / CMO | Matrix / Funnel Breakdowns | Isolate clinical handoff bottlenecks |
| **UC-03** | Demographic & Equity | Equity Officer / Admin | Demographic Slicers & Bar Charts | Ensure uniform, bias-free care delivery |

---

## 🚀 How to Use the Repository
1. Clone this repository to your local machine.
2. Ensure you have **Power BI Desktop** installed.
3. Open `Hospital ER_Data_analysis.pbix` to view the dashboards and interact with the data models.

Created By : Poojashri K
