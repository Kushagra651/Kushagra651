<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24c6dc&height=200&section=header&text=Kushagra%20Bhargava&fontSize=46&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=ML%20%7C%20MLOps%20%7C%20Retrieval%20%26%20LLM%20Systems&descSize=18&descAlignY=58" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=18&pause=1000&color=24C6DC&center=true&vCenter=true&width=640&lines=Final-year+ISE+%40+DSCE+Bengaluru+%7C+2027+batch;I+build+ML+systems+end+to+end%2C+and+measure+them+honestly.;Monitoring+%7C+Retrieval+%7C+Evals+%7C+MLOps;Learning+in+public.+Shipping+side+projects+weekly." alt="Typing SVG" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kushagrabhargava651)
[![Gmail](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kushagrabhargava93@gmail.com)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/aapnakaamkar)
[![Substack](https://img.shields.io/badge/Substack-FF6719?style=for-the-badge&logo=substack&logoColor=white)](https://substack.com/@kushagrabhargava)
[![Phone](https://img.shields.io/badge/Call-+91_6350655535-24c6dc?style=for-the-badge&logo=googlemessages&logoColor=white)](tel:+916350655535)

</div>

---

## 👋 About

I like the full arc of an ML system: data, model, serving, monitoring, and the measurement that tells you whether any of it worked. My projects are personal builds, and I write down what failed as readily as what worked (a loss that beat my architecture, a gate set below the majority baseline, a leaky test I had to rebuild).

- 🎓 Final-year B.E. Information Science, Dayananda Sagar College of Engineering, Bengaluru | 2027 batch | CGPA 8.58
- 🔧 Contributed to open source: **Giskard AI** (PR #2440, Bias LLM Judge evaluation check) and a **pgmpy** PR on composable regressors for structure scoring
- 🏆 Kaggle **Top 16%** (350 / 2,247, Spaceship Titanic) with stacked XGBoost, LightGBM and Random Forest
- 🧪 Worked on a churn model (ROC-AUC 0.91 vs 0.73 baseline) during an ML internship at Fitin, Jan to Mar 2026
- ✍️ Writing about ML systems and RAG on [Substack](https://substack.com/@kushagrabhargava)
- 📍 Bengaluru | Open to remote and relocation

---

## 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🛡️ SentinelML
**ML monitoring and auto-retraining**

3 Airflow DAGs (6-hour drift check, gated retrain with 12-hour cooldown, train-evaluate-register), FastAPI hot-reload serving, PostgreSQL prediction logging, MLflow registry, Docker Compose.

- False drift alarms cut **44% → 1.5%** with a Bonferroni-corrected p-value gate plus PSI 0.1 over a KS / chi-square / PSI detector
- Load-tested to a 50 req/s ceiling, p95 298 ms, 0% errors at 10 concurrent users
- Found my own accuracy gate sat below the majority baseline and fixed it

`Airflow` `MLflow` `Prometheus` `Grafana` `FastAPI` `Docker`

[→ Repo](https://github.com/kushagra651/SentinelML)

</td>
<td width="50%" valign="top">

### 🔍 FintelRAG
**Financial document intelligence**

Hybrid retrieval over 4,737 SEC 10-K chunks: vocabulary-level BM25 sparse vectors (30,800 tokens) fused with 768-dim Qdrant dense embeddings via RRF, orchestrated in LangGraph.

- DeepEval faithfulness **0.48 → 0.89**, context precision **0.51 → 1.00** (20 QA pairs)
- Cold start **200 s → under 1 s** by persisting the BM25 corpus
- Regex pre-routing skips LLM decomposition for single-company queries

`Qdrant` `BM25` `LangGraph` `DeepEval` `Groq`

[→ Repo](https://github.com/kushagra651/FintelRAG)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎯 RecTower
**Two-tower retrieval recommender**

PyTorch two-tower model with in-batch InfoNCE on MovieLens-1M (575K interactions). Diagnosed popularity bias and added logQ correction.

- Full-catalog NDCG@10 **0.016 → 0.0347** (3 seeds), about 10% above tuned BPR-MF and ItemKNN
- Replaced inflated sampled metrics with full-catalog ranking, rebuilt a leaky cold-start test
- FAISS + FastAPI + Docker, 24 pytest tests, retrieval p99 3.3 ms

`PyTorch` `FAISS` `FastAPI` `Docker`

[→ Repo](https://github.com/kushagra651/RecTower)

</td>
<td width="50%" valign="top">

### 🧱 Also built

- **LexRA**: QLoRA fine-tune of TinyLlama 1.1B on Indian legal text ([HuggingFace](https://huggingface.co/aapnakaamkar))
- **MediFlow**: hospital demand forecasting with SHAP explainability
- **VC AI Agents**: multi-agent due-diligence loops with Pydantic-validated outputs

[→ All repositories](https://github.com/kushagra651?tab=repositories)

</td>
</tr>
</table>

---

## 🧰 Toolkit

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-EA4335?style=flat-square)
![HuggingFace](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square)

![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apache-airflow&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

</div>

| Area | What I work with |
|---|---|
| 🧮 **Problem solving** | Data structures and algorithms in Python and C++; thinking in complexity, trade-offs and edge cases before writing code |
| 🗄️ **SQL and data** | PostgreSQL, MySQL, MongoDB; schema design, prediction logging, analytical queries over model outputs |
| ⚙️ **MLOps** | Drift detection, gated retraining, model registry and promotion gates, CI/CD, load testing, Prometheus and Grafana metrics |
| 🧠 **LLMs and retrieval** | Hybrid BM25 + dense search, RRF fusion, LoRA/PEFT, 4-bit quantization, LLM evals with DeepEval |

---

## 📡 Currently Learning

- **Serving and scale**: distributed model serving, batching and latency budgets
- **Evals**: LLM-as-judge reliability, regression gates for RAG and agent pipelines
- **ML platform habits**: experiment tracking, reproducibility, monitoring that stays quiet unless something is actually wrong
- **Cloud ML**: SageMaker and Vertex AI workflows

I write up what I learn on [Substack](https://substack.com/@kushagrabhargava).

---

## 🐍 Contribution Snake

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/kushagra651/kushagra651/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/kushagra651/kushagra651/output/github-snake.svg" />
    <img alt="Contribution snake" src="https://raw.githubusercontent.com/kushagra651/kushagra651/output/github-snake-dark.svg" />
  </picture>
</div>

---

## 📊 GitHub Snapshot

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=kushagra651&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&bg_color=0f0c29" height="170"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kushagra651&layout=compact&theme=tokyonight&hide_border=true&bg_color=0f0c29" height="170"/>
</div>

---

## 📬 Let's Talk

I'm looking for an ML / AI engineering internship with a path to full-time. If you're building retrieval, evals, or ML infrastructure and want someone who measures before claiming, I'd like to hear from you.

| | |
|---|---|
| 📧 Email | [kushagrabhargava93@gmail.com](mailto:kushagrabhargava93@gmail.com) |
| 💼 LinkedIn | [linkedin.com/in/kushagrabhargava651](https://www.linkedin.com/in/kushagrabhargava651) |
| 📞 Phone | [+91 6350655535](tel:+916350655535) |
| 🤗 HuggingFace | [aapnakaamkar](https://huggingface.co/aapnakaamkar) |
| ✍️ Substack | [@kushagrabhargava](https://substack.com/@kushagrabhargava) |

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:24c6dc,50:302b63,100:0f0c29&height=90&section=footer" width="100%"/>
