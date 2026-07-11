<p align="center">
  <img src="images/banner_profile.png" width="100%" alt="Rohit Bhowmick - Data Scientist">
</p>

<h1 align="center">Hi, I'm Rohit Bhowmick 👋</h1>
<h3 align="center">Data Scientist | ML Engineer | Analytics & Financial Crime Intelligence</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/XGBoost-006ACC?style=for-the-badge" />
  <img src="https://img.shields.io/badge/LightGBM-00A0DC?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
</p>

<p align="center">
  <a href="mailto:rohitbhowmick817@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/rohit-bhowmick"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/rohit-bhowmick2002"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

---

## 👨‍💻 About Me

I build **end-to-end data science systems** — from synthetic and real-world data pipelines, through SQL analytics and machine learning, to interactive dashboards that non-technical stakeholders can actually use. My work spans **financial crime detection (fraud & AML)**, **retail demand forecasting**, **e-commerce customer analytics**, and **subscription churn modeling**.

Across my projects I consistently focus on four things:

- 📐 **Rigorous data foundations** — normalized schemas, partitioned warehouses, reproducible ETL
- 🧠 **Production-style ML** — calibrated gradient-boosted models (XGBoost/LightGBM), SHAP explainability, proper train/test discipline
- 📊 **SQL-first analytics** — hundreds of hand-written, business-intent-documented queries across my repos
- 🖥️ **Decision-ready delivery** — Streamlit apps, executive dashboards, and API endpoints, not just notebooks

Below are four projects that showcase this approach across different domains.

---

## 🚀 Featured Projects

### 🕵️ 1. [Fraud Detection & AML Analytics Platform](https://github.com/rohit-bhowmick2002/Fraud-Detection-AML-Analytics-Platform)
**A simulated retail bank, built to be investigated.**

<p align="center">
  <img src="images/banner_fraud.png" width="100%" alt="Fraud Detection and AML Analytics Platform Banner">
</p>

A synthetic financial-crime platform generating **1,000,000 deterministic transactions** across 50,000 customers, then hunting fraud and money laundering inside that data.

<p align="center">
  <img src="images/fraud_01_executive_dashboard.png" width="100%" alt="SentinelFlow Executive Dashboard">
</p>

<p align="center">
  <img src="images/fraud_02_roc_pr_curve.png" width="49%" alt="Fraud Model ROC and PR Curve">
  <img src="images/fraud_04_mule_network.png" width="49%" alt="AML Mule Network Graph">
</p>

<details>
<summary>📊 View fraud typology breakdown</summary>
<p align="center"><img src="images/fraud_03_typology_breakdown.png" width="85%" alt="Fraud Typology Breakdown"></p>
</details>

- 🎯 **14 fraud typologies** (account takeover, synthetic ID, bust-out, bin attacks…) and **9 AML typologies** (structuring, layering, smurfing, mule accounts…)
- 🧮 **62 production SQL analyses** across fraud, AML, KPI, risk, network, and regulatory categories
- 🤖 XGBoost fraud model — **0.941 ROC-AUC**, isotonic calibration, SHAP explainability
- 🕸️ NetworkX mule-network detection — PageRank scoring + Louvain community detection (12 mule communities found)
- 🖥️ 5-tab Streamlit investigator console + FastAPI scoring service (`/score`, `/aml/evaluate`) + Power BI star schema
- 🏛️ Governance built in: model cards, SAR/CTR templates, audit logging, CI with a live Postgres service

**Stack:** PostgreSQL 16 · Python 3.11 · XGBoost · FastAPI · Streamlit · NetworkX · Docker · GitHub Actions

---

### 🛒 2. [Retail Sales Forecasting](https://github.com/rohit-bhowmick2002/retail-sales-forecasting)
**Forecasting demand for a national retail chain on real Kaggle data.**

<p align="center">
  <img src="images/banner_retail.png" width="100%" alt="Retail Sales Forecasting Banner">
</p>

Built on the Corporación Favorita dataset (**3M+ transactions**, 54 stores), this project forecasts retail sales and quantifies the ROI of promotions.

<p align="center">
  <img src="images/retail_01_forecast.png" width="100%" alt="Retail Sales Actual vs Forecast">
</p>

<p align="center">
  <img src="images/retail_02_model_comparison.png" width="32%" alt="Model Comparison MAE">
  <img src="images/retail_03_feature_importance.png" width="32%" alt="Feature Importance">
  <img src="images/retail_04_promotion_lift.png" width="32%" alt="Promotion Lift">
</p>

- 📈 XGBoost forecasting model — **MAE of $1,850**, a **42% improvement over Prophet**
- 🎯 R² of **0.78** on holdout data
- 🎁 Quantified **+68% promotional lift**, giving a clear read on campaign ROI
- 🧮 50+ ready-to-run SQL business-intelligence queries
- 🖥️ Real-time Streamlit dashboard, fully containerized with Docker

**Stack:** Python · XGBoost · Prophet · Streamlit · Plotly · Docker

---

### 📦 3. [Olist E-Commerce Analytics & ML Platform](https://github.com/rohit-bhowmick2002/Olist-E-Commerce-Analytics-ML-Platform)
**Turning 1.55M rows of real Brazilian marketplace data into a decision-making platform.**

<p align="center">
  <img src="images/banner_olist.png" width="100%" alt="Olist E-Commerce Analytics Platform Banner">
</p>

An end-to-end analytics platform on the Olist Brazilian e-commerce dataset (99K orders, 96K customers, R$15.8M GMV), combining SQL, ML, and dashboards to answer concrete revenue, churn, and satisfaction questions.

<p align="center">
  <img src="images/olist_01_kpi_dashboard.png" width="100%" alt="Olist Executive KPI Dashboard">
</p>

<p align="center">
  <img src="images/olist_02_churn_roc.png" width="49%" alt="Olist Churn ROC Curve">
  <img src="images/olist_03_cohort_retention.png" width="49%" alt="Olist Cohort Retention Heatmap">
</p>

- 🧮 **55 hand-written SQL queries** across 8 business sections — all validated by an automated smoke test (55/55 passing)
- 🤖 **3 ML models:** XGBoost churn classifier (**0.8945 ROC-AUC**), gradient-boosting review-score regressor (0.90★ MAE), and KMeans RFM segmentation (top 3% of customers → 24% of GMV)
- 💰 Six impact initiatives mapped directly to SQL/ML signals, totaling an estimated **R$2.3M+** in annual value
- 🖥️ Two dashboards ship in the repo: a 9-page Streamlit app with live model scoring, and a self-contained static HTML dashboard

**Stack:** SQLite · Python · XGBoost · scikit-learn · Streamlit · Plotly

---

### 🎵 4. [KKBox Churn Prediction](https://github.com/rohit-bhowmick2002/kkbox-churn-prediction)
**Predicting subscriber churn for a music streaming service (WSDM Cup 2018).**

<p align="center">
  <img src="images/banner_kkbox.png" width="100%" alt="KKBox Churn Prediction Banner">
</p>

A churn-prediction pipeline built on KKBox's dataset of **30M+ records**, engineering 87 features from member, transaction, and listening-behavior data.

<p align="center">
  <img src="images/kkbox_01_executive_dashboard.png" width="100%" alt="KKBox Executive Dashboard">
</p>

<p align="center">
  <img src="images/kkbox_03_roc_all_models.png" width="49%" alt="KKBox ROC Curve All Models">
  <img src="images/kkbox_02_feature_importance.png" width="49%" alt="KKBox Feature Importance">
</p>

- 🏆 Best model (LightGBM) achieved **0.8923 ROC-AUC**, beating the 0.85 target
- 🔑 Auto-renewal status emerged as the single strongest churn signal — churn risk is **5.8x higher** when disabled
- 🧪 87 engineered features, 5 models compared (LightGBM, XGBoost, CatBoost, Random Forest, Logistic Regression), 21 passing unit tests
- 🔍 SHAP-based explainability distinguishing risk-increasing vs. risk-decreasing behaviors
- 💼 Business recommendations translated into a **5.1x projected ROI** across four retention initiatives
- 🖥️ Streamlit app for live scoring, backed by a documented SQL analysis layer

**Stack:** Python · LightGBM · XGBoost · CatBoost · scikit-learn · SHAP · Streamlit · pytest

---

## 🧰 Tech Stack

| Category | Tools |
|---|---|
| **Languages** | Python, SQL |
| **ML / Modeling** | XGBoost, LightGBM, CatBoost, scikit-learn, SHAP |
| **Data Engineering** | pandas, NumPy, PostgreSQL, SQLite, ETL pipelines |
| **Visualization** | Streamlit, Plotly, matplotlib, seaborn, Power BI |
| **APIs & Serving** | FastAPI |
| **Graph / Network Analytics** | NetworkX |
| **DevOps** | Docker, GitHub Actions (CI/CD) |

---

## 📫 Get in Touch

- 📧 **Email:** rohitbhowmick817@gmail.com
- 💼 **LinkedIn:** [linkedin.com/in/rohit-bhowmick](https://www.linkedin.com/in/rohit-bhowmick)
- 🐙 **GitHub:** [github.com/rohit-bhowmick2002](https://github.com/rohit-bhowmick2002)

<p align="center"><i>⭐ If any of these projects are useful to you, a star is always appreciated.</i></p>
