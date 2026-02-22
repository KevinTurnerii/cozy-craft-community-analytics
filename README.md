# 🧶 Cozy Craft Community Analytics  
Community Growth • Engagement Modeling • Capacity Forecasting  

Comprehensive event analytics using Python and Power BI.  
Applies dimensional modeling, KPI engineering, and executive dashboard design to evaluate community growth, attendance utilization, and retention behavior.

---

## 📑 Table of Contents

- [Project Overview](#project-overview)
- [Business Objective](#business-objective)
- [Data Architecture](#data-architecture)
- [Methodology](#methodology)
- [Key Metrics & Insights](#key-metrics--insights)
- [Power BI Dashboard](#power-bi-dashboard)
- [Dashboard Preview](#dashboard-preview)
- [Tools & Technologies](#tools--technologies)
- [Skills Demonstrated](#skills-demonstrated)
- [Business Impact](#business-impact)
- [Conclusion](#conclusion)
- [Repository Structure](#repository-structure)
- [Education & Certifications](#education--certifications)
---

## 📘 Project Overview

This project analyzes Cozy Craft’s transition from three 2025 pilot events to expanded 2026 operations, measuring growth sustainability, attendance efficiency, and repeat engagement behavior across six total events.

While 2025 established initial capacity build, 2026 serves as the first statistically reliable operational baseline for forecasting and KPI modeling.

---

## 🎯 Business Objective

To evaluate community expansion, measure attendance efficiency, and design a data-driven ticket release strategy that supports sustainable growth.

---

## 🏗 Data Architecture

Dimensional modeling approach:

**Dimension Table**
- `cozy_dim_event`

**Fact Tables**
- `cozy_fact_orders`
- `cozy_fact_attendance`

Design principles:

- One row per event grain  
- Explicit separation of seats reserved vs verified check-ins  
- No silent filtering or recomputation  
- All Power BI visuals driven from validated notebook outputs  

---

## 🔬 Methodology

The project followed a structured analytics pipeline:

1. Raw data ingestion (Orders, Attendees, Check-ins)  
2. Event-level normalization  
3. Attendance rate calculation  
4. Conversion ratio modeling  
5. Repeat participant identification  
6. Scenario-based forecasting model (ticket release → attendance target)  

All KPI calculations were programmatically validated in the final notebook section against raw check-in exports to ensure reconciliation and metric integrity.

---

## 📊 Key Metrics & Insights

Analysis spans 6 total events (3 in 2025, 3 in 2026), with 2026 treated as the first stable operational baseline.

### 📈 Capacity Growth
- **206% total capacity growth (2025 → 2026)**  
- Event expansion from pilot-scale to large-format meetups  

### 🎟 Attendance Utilization
- **46% average verified attendance rate (2026)**  
- Clear opportunity to optimize ticket release volume  

### 🔁 Engagement Depth
- **44.31% buyer conversion rate**  
- **18.92% repeat core participation rate**  

Indicates early-stage community loyalty formation.

### 📦 Forecast Model
- **152 recommended ticket release**  
  to achieve ~70 verified attendees  
  (Based on historical attendance behavior)

Demonstrates operational forecasting capability.

---

## 📊 Power BI Dashboard

Power BI serves as the executive synthesis layer.

### Page 1 — Growth
- Seats Reserved by Event  
- Growth Rate Over Time  
- Capacity Trend Visualization  

### Page 2 — Utilization
- Verified Check-Ins vs Seats  
- Attendance Rate %  
- Underutilized Capacity Analysis  

### Page 3 — Engagement
- Buyer vs Attendee Conversion  
- Repeat Participant Breakdown  
- Community Depth Indicators  

### Page 4 — Forecast
- Ticket Release Scenario Modeling  
- Attendance Target Planning  
- Capacity Optimization Strategy  

All measures implemented in DAX.  
No Power Query transformations.  
No hidden filters.

---

## 📸 Dashboard Preview

These visuals represent the final executive reporting layer, built exclusively on validated modeling outputs from the Python pipeline.

### Growth Overview
<p align="center">
  <img src="images/cozy%20craft%20growth%201.png" width="80%">
</p>

### Attendance & Utilization
<p align="center">
  <img src="images/cozy%20craft%20attendance%20%26%20utilizaation%202.png" width="80%">
</p>

### Engagement Model
<p align="center">
  <img src="images/cozy%20craft%20engagement%203%20.png" width="80%">
</p>

### Capacity Forecast
<p align="center">
  <img src="images/cozy%20craft%20forecast%204.png" width="80%">
</p>


## 🛠 Tools & Technologies

- Python (pandas, KPI engineering, modeling)  
- Jupyter Notebook  
- Power BI (DAX-based KPI calculations)  
- Dimensional modeling principles  

---

## 💼 Skills Demonstrated

- KPI Engineering  
- Event-Level Fact Table Design  
- Attendance Forecast Modeling  
- Conversion Funnel Analysis  
- Repeat Engagement Segmentation  
- Executive Dashboard Development  
- Data Integrity & Metric Reconciliation  

---

## 🚀 Business Impact

This project demonstrates the ability to:

- Translate event-level operational data into strategic KPIs  
- Identify inefficiencies in ticket utilization  
- Quantify community engagement depth  
- Design actionable growth forecasts  
- Deliver stakeholder-ready dashboards  

The framework can be adapted for:

- Nonprofit event planning  
- Membership communities  
- Subscription growth modeling  
- Conference capacity planning  

---

## 📂 Repository Structure

```
cozy-craft-community-analytics/
│
├── data/
│ ├── raw/
│ └── processed/
│
├── notebooks/
├── powerbi/
├── images/
└── README.md
```

---

## 🔒 Data Integrity & Validation
All executive KPIs were programmatically derived and reconciled against raw check-in exports in the final notebook section.

No manual adjustments were applied to reporting outputs.
All dashboard measures trace directly to validated modeling results.

---

## 🧭 Conclusion

Cozy Craft’s expansion from pilot events to scaled 2026 operations established a measurable attendance baseline and a predictable engagement structure.

By combining dimensional modeling, conversion analysis, and scenario-based forecasting, this project transforms event-level exports into a strategic growth framework.

The resulting analytics system enables sustainable capacity planning, ticket release optimization, and long-term community retention strategy.

 
