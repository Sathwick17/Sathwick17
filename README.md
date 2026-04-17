<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:7c3aed&height=140&section=header&text=Sathwick%20Kiran%20M%20S&fontSize=38&fontColor=ffffff&fontAlignY=55&desc=Data%20Professional%20%7C%20Python%20%C2%B7%20SQL%20%C2%B7%20ETL%20%C2%B7%20ML%20%C2%B7%20Power%20BI%20%7C%20Ex-Sony%20%7C%20MS%20Data%20Science%2C%20UB&descAlignY=78&descSize=13" width="100%"/>

</div>

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-0ea5e9?style=for-the-badge&logo=vercel&logoColor=white)](https://sathwick17.github.io/sathwick-portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-7c3aed?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sathwick-kiran-m-s-708b43193/)
[![Email](https://img.shields.io/badge/Email-0f172a?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sathwick@buffalo.edu)

</div>

---

### 👋 About Me

Data professional with 2 years of experience at Sony and an MS in Data Science from the University at Buffalo. My work spans data engineering, analytics, and applied machine learning — building ETL pipelines, Power BI dashboards, and reporting solutions that cross-functional teams use to make decisions.

At Sony, I worked on Python and SQL data workflows across 5+ internal teams, automated reporting pipelines, and implemented data quality checks that improved consistency and reduced manual effort by 15%. Outside of work I have built a LangGraph multi-agent AI system using LLMs and generative AI, processed 3.3M+ records using PySpark and NLP on Hadoop, and built a containerized DataOps observability platform with Kafka, Airflow, dbt, and Tableau.

**Open to full-time roles in:** Data Analytics · Data Engineering · Analytics Engineering · Data Science · Machine Learning Engineering

---

### 🚀 Featured Projects

---

**01 — DataOps Change Impact & Pipeline Failure Observability Platform**

> *End-to-end DataOps platform for real-time pipeline monitoring, schema drift detection, SLA tracking, and AI-assisted root cause analysis*

Modern data teams lack centralized visibility into pipeline health. This platform addresses that — tracking every pipeline run, detecting failures and SLA breaches in real time, tracing downstream schema change impact, and surfacing root causes via a RAG-powered API backed by a local LLaMA model.

```
Kafka Topics → Airflow Orchestration → PostgreSQL Raw Layer
                                              │
                                          dbt Core
                                              │
                                    Analytics Mart Layer
                                    ┌─────────┴──────────┐
                                 Grafana             FastAPI + RAG
                               Dashboards          (Ollama + LLaMA)
```

| Component | Tool |
|-----------|------|
| Streaming | Apache Kafka |
| Orchestration | Apache Airflow |
| Storage | PostgreSQL |
| Transformation | dbt Core |
| Dashboards | Grafana |
| RCA / AI Layer | RAG · Ollama · LLaMA · FastAPI |
| Infrastructure | Docker Compose |

| Phase | Description | Status |
|-------|-------------|--------|
| 0 | Project Setup | ✅ Done |
| 1 | Base Data Layer | ✅ Done |
| 2 | Historical Data Generation & Batch ETL | ✅ Done |
| 3 | SQL Modeling and dbt Layer | ✅ Done |
| 4 | Grafana Dashboard Layer | ✅ Done |
| 5 | Kafka Streaming Layer | ✅ Done |
| 6 | Airflow Orchestration | ✅ Done |
| 7 | Change Impact Logic | 🔄 In Progress |
| 8 | RAG Layer (Ollama + FastAPI) | ⬜ Pending |
| 9 | Final Polish | ⬜ Pending |

![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0ea5e9?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

**[View Repository →](https://github.com/Sathwick17/dataops-observability-platform)**

---

**02 — Osteoporosis Risk Prediction**

> *Multi-model classification pipeline for early-stage osteoporosis detection from patient medical records*

Built on 1,958 patient records, this project applies four ML classifiers — Logistic Regression, Random Forest, Decision Tree, and SVC — to predict osteoporosis risk from clinical features including age, hormonal changes, calcium intake, and physical activity. The Decision Tree Classifier achieved **90.6% accuracy** after hyperparameter tuning, up from a 73% baseline, and was selected for its clinical interpretability.

| Model | Accuracy |
|-------|----------|
| Logistic Regression | 83.1% |
| Random Forest | 85.3% |
| **Decision Tree (Tuned)** | **90.6%** |
| Support Vector Classifier | 57.8% |

![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![RMarkdown](https://img.shields.io/badge/RMarkdown-276DC3?style=flat-square&logo=r&logoColor=white)
![caret](https://img.shields.io/badge/caret-7c3aed?style=flat-square&logoColor=white)
![ggplot2](https://img.shields.io/badge/ggplot2-a855f7?style=flat-square&logoColor=white)

**[View Repository →](https://github.com/Sathwick17/osteoporosis_detection)**

---

**03 — Amazon Book Review Analytics**

> *Full-scale big data pipeline processing 3.3M+ reviews using Hadoop, PySpark, and Spark MLlib*

An end-to-end distributed ML pipeline covering the complete data lifecycle — HDFS ingestion via a custom Java ingestion script, PySpark EDA, TF-IDF feature extraction, and multi-model training for sentiment classification, rating prediction, and helpfulness prediction. Post hyperparameter tuning with GridSearchCV, Logistic Regression achieved **95.01% accuracy** and **93.45% F1-score** as the best-performing model.

| Model | Accuracy (Tuned) | F1-Score (Tuned) |
|-------|-----------------|-----------------|
| **Logistic Regression** | **95.01%** | **93.45%** |
| SVM | 88.64% | 86.81% |
| Random Forest | 60.86% | 46.97% |

```
books.csv + rating.csv → HDFS → PySpark EDA → TF-IDF Feature Extraction
        → Spark MLlib (LR · SVM · RF) → GridSearchCV Tuning → Results → HDFS
```

![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Hadoop](https://img.shields.io/badge/Hadoop_HDFS-FFCE00?style=flat-square&logo=apachehadoop&logoColor=black)
![Spark MLlib](https://img.shields.io/badge/Spark_MLlib-E25A1C?style=flat-square&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0ea5e9?style=flat-square&logo=docker&logoColor=white)

**[View Repository →](https://github.com/Sathwick17/amazon-bigdata-review-analytics)**

---

**04 — Synapse Street · AI Multi-Agent Short Selling Detection**

> *Multi-agent LLM system for detecting short-selling opportunities in U.S. equities — built in 15 hours at UB Hackers 2024*

Three coordinated LangGraph agents — Analyst, Model, and Risk — share a Qdrant vector memory and collaboratively evaluate short-selling signals across a ~5GB historical U.S. stock dataset processed on a two-node HDFS cluster (Vultr Cloud). A Logistic Regression model computes per-ticker short probabilities, with the top candidate **CMAX** reaching a 94.5% short probability. Results surface via Streamlit and Tableau dashboards.

| Metric | Result |
|--------|--------|
| AUROC | 0.642 |
| Precision@10 | 0.60 |
| Top Short Candidate | CMAX — 94.5% probability |
| Build Time | 15 hours |

![LangGraph](https://img.shields.io/badge/LangGraph-7c3aed?style=flat-square&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-0ea5e9?style=flat-square&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-f97316?style=flat-square&logo=scikitlearn&logoColor=white)
![Hadoop](https://img.shields.io/badge/Hadoop_HDFS-FFCE00?style=flat-square&logo=apachehadoop&logoColor=black)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**[View Repository →](https://github.com/Sathwick17/ub_hackers)**

---

### 🛠️ Skills & Stack

**Languages**

![Python](https://img.shields.io/badge/Python-0ea5e9?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-7c3aed?style=flat-square&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-1e2440?style=flat-square&logo=gnubash&logoColor=white)

**ML & AI**

![Scikit-learn](https://img.shields.io/badge/Scikit--learn-f97316?style=flat-square&logo=scikitlearn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-7c3aed?style=flat-square&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-0ea5e9?style=flat-square&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-34d399?style=flat-square&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)

**Data Engineering**

![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Hadoop](https://img.shields.io/badge/Hadoop_HDFS-FFCE00?style=flat-square&logo=apachehadoop&logoColor=black)

**Analytics & BI**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

**Cloud & Tools**

![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0ea5e9?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

---

<div align="center">

📍 New York, United States &nbsp;·&nbsp; 💼 Open to Data Analyst · Data Engineer · Data Scientist · Analytics Engineer · ML Engineer roles

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3aed,100:0ea5e9&height=80&section=footer" width="100%"/>

</div>
