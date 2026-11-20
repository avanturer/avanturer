<p align="center">
  <img src="./assets/profile-header.svg" alt="Rodion Orkin — Senior Machine Learning Engineer / ML Lead" width="100%" />
</p>

<p align="center">
  <a href="https://t.me/bizarreman"><img src="https://img.shields.io/badge/Telegram-@bizarreman-229ED9?style=flat-square&logo=telegram&logoColor=white" alt="Telegram" /></a>
  <a href="mailto:rodion.ork@yandex.ru"><img src="https://img.shields.io/badge/Email-Contact-64748B?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://fuddy.team"><img src="https://img.shields.io/badge/Product-Fuddy-0F766E?style=flat-square&logo=googlechrome&logoColor=white" alt="Fuddy" /></a>
</p>

<p align="center">
  Building production ML systems — from data and modeling to experimentation, serving, and monitoring.
</p>

---

## 🎯 Selected impact

<table>
  <tr>
    <td width="50%" align="center" valign="middle">
      <h2>−20–25%</h2>
      <strong>CPA reduction</strong><br />
      <sub>100+ advertisers · online A/B tests</sub>
    </td>
    <td width="50%" align="center" valign="middle">
      <h2>+9%</h2>
      <strong>Recommendation CTR</strong><br />
      <sub>+2.3% revenue per session</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center" valign="middle">
      <h2>611K</h2>
      <strong>Products relabeled</strong><br />
      <sub>Fine-tuned LLM · production catalog</sub>
    </td>
    <td width="50%" align="center" valign="middle">
      <h2>10K+</h2>
      <strong>Fuddy downloads</strong><br />
      <sub>Independent product · paid subscriptions</sub>
    </td>
  </tr>
</table>

## 🧭 What I build

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>🎯 AdTech</h3>
      Purchase propensity · conversion modeling · bid optimization · calibration · offline conversions
      <br /><br />
      <sub><strong>Impact:</strong> CPA −20–25% across 100+ advertisers</sub>
    </td>
    <td width="33%" valign="top">
      <h3>🧠 RecSys</h3>
      Candidate generation · ranking · personalization · cold start · low-latency serving
      <br /><br />
      <sub><strong>Impact:</strong> CTR +9% in an online A/B test</sub>
    </td>
    <td width="33%" valign="top">
      <h3>🤖 LLM Engineering</h3>
      SFT / QLoRA · evaluation · distillation · inference · acceptance gates
      <br /><br />
      <sub><strong>Impact:</strong> fine-tuned models shipped to production</sub>
    </td>
  </tr>
</table>

## 🏢 Experience

### RivoxAI · Machine Learning Engineer / ML function owner

<sub>Mar 2025 — Present · AdTech · AI bid optimization for Yandex Direct</sub>

- Built the ML function from scratch and owned its lifecycle: hypothesis backlog, data and training pipelines, deployment, online experiments, and monitoring. Coordinated a junior MLE and a senior data analyst.
- Developed purchase-propensity models for **100+ advertisers**. Reduced **CPA by 20–25% without reducing lead volume** in 4–6-week online A/B tests; designed a cold-start path for clients with fewer than 30 conversions.
- Engineered **~600 features** from **~5M clickstream events/day**. Improved CatBoost PR-AUC from **0.35 to 0.42** at ~1% purchase prevalence (ROC-AUC 0.90); increased auto-bidding signals **2–5×** through calibrated virtual conversions and offline-conversion uploads.
- Introduced weekly retraining and production monitoring, detecting **10+ tracking failures** before they wasted advertising spend.

<sub>Python · SQL · Polars · CatBoost · PyTorch · Optuna · MLflow · Docker · GCP · Yandex Metrica API</sub>

### CognitiveWave · Data Scientist / Recommender Systems

<sub>Sep 2023 — Feb 2025 · B2B e-commerce · catalogs up to ~500K SKUs</sub>

- Built a multi-tenant, two-stage recommender: ALS and two-tower candidate generation with Faiss HNSW retrieval, followed by LightGBM ranking. Improved NDCG@10 **0.21 → 0.24** and Recall@100 **0.34 → 0.40**; SASRec signals raised NDCG@10 to **0.26** for active users.
- Delivered **+9% CTR** and **+2.3% revenue per session** (*p* < 0.01) in a four-week online A/B test for a fashion retailer with ~2M MAU.
- Improved new-item cold start with multilingual-e5 embeddings (**Recall@100 0.06 → 0.17**) and served recommendations at **P99 < 50 ms** using Redis precomputation and FastAPI re-ranking.

<sub>Python · PyTorch · implicit · LightGBM · Faiss · Redis · FastAPI · Docker</sub>

## 🚀 Founder project · Fuddy

**Founder & ML Engineer · solo project** · [fuddy.team](https://fuddy.team) · <sub>2026 — Present</sub>

A consumer product scanner for food and cosmetics. **10K+ downloads · paid subscriptions.** I lead product and ML engineering end to end.

- Fine-tuned **Qwen3-14B with QLoRA** on 230K labeled products, replacing a Qwen3-235B-A22B API dependency for nutrient and NOVA estimation; relabeled the full **611K-product** catalog and shipped it to production.
- Built acceptance gates across **~20 quality dimensions**. Traced a TRL / bf16 LoRA issue that rounded **74–96% of LoRA updates to zero**; added write-guards, reducing false-zero salt predictions from **309 to 8** in a 9.5K-product shadow evaluation.
- In a separate benchmark, an 8B prototype reached **92.7% NOVA accuracy vs. 70.0%** for Qwen3-235B-A22B (*n* = 327), with valid JSON improving from **90% to 100%**.

<sub>Python · PyTorch · Unsloth · TRL · QLoRA · bitsandbytes · vLLM · OCR · TypeScript · Next.js</sub>

## 🧰 Core technologies

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=py,pytorch,sklearn,cpp,postgres,redis,docker,fastapi,gcp,git&perline=10" alt="Python, PyTorch, scikit-learn, C++, PostgreSQL, Redis, Docker, FastAPI, GCP, Git" />
  </a>
</p>

| Area | Tools & methods |
|---|---|
| **ML & experimentation** | CatBoost, LightGBM, XGBoost, Optuna, feature engineering, probability calibration, A/B testing, bootstrap CIs |
| **Recommender systems** | ALS, two-tower, SASRec, GRU, Faiss, node2vec, candidate generation, ranking, cold start |
| **LLM engineering** | SFT, QLoRA, Unsloth, TRL, bitsandbytes, vLLM, model evaluation, distillation, embeddings, OCR |
| **Data & production** | Polars, pandas, FastAPI, Redis, Docker, Airflow, MLflow, Vertex AI, Cloud SQL, Grafana |

## 🎓 Education & recognition

<table>
  <tr>
    <td width="60%" valign="top">
      <strong>ITMO University · AI Talent Hub</strong><br />
      <sub>MSc in Artificial Intelligence · in progress</sub><br /><br />
      <strong>NUST MISIS</strong><br />
      <sub>BSc in Applied Mathematics</sub>
    </td>
    <td width="40%" valign="top">
      🥇 <strong>1st place</strong> · TechFriend AI Hack<br /><br />
      🥉 <strong>3rd place</strong> · PSB.Hack, HSE University
    </td>
  </tr>
</table>

<sub>Additional training: Yandex School of Data Analysis · NLP | Deep Learning School, MIPT · CV / NLP</sub>

---

<p align="center">
  <strong>Russian</strong> — Native &nbsp;·&nbsp; <strong>English</strong> — C1
  <br /><br />
  <a href="https://t.me/bizarreman">Telegram</a> &nbsp;·&nbsp;
  <a href="mailto:rodion.ork@yandex.ru">Email</a> &nbsp;·&nbsp;
  <a href="https://fuddy.team">Fuddy</a>
</p>
