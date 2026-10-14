<h1 align="center">Seifeddine Ghozzi</h1>
<p align="center">
  <b>AI & Machine Learning Engineer</b> · ENSTA Paris (Institut Polytechnique de Paris)<br>
  LLM applications · RAG & agents · trustworthy, privacy-aware AI<br>
  Paris, France · open to new opportunities
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/seifeddine-ghozzi/"><img src="https://img.shields.io/badge/-LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:seifeddine.ghozzi@ensta.fr"><img src="https://img.shields.io/badge/-Email-333?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

---

## 👋 About

I'm an engineer from ENSTA Paris specialised in AI and machine learning, with experience in **research**
(Inria, ICML co-author) and in the **telecom industry** (SFR). I like building LLM systems where
correctness can be *checked*: deterministic code around the model, evidence for every claim, and measured
results rather than demos.

---

## 💼 Experience

**AI & Data Engineering Intern — SFR** · Paris · *Apr – Oct 2026*
- Built the **RAG pipeline** behind a fully local, engineer-facing chatbot over technical documentation:
  parent-child chunking, hybrid search (dense + BM25), reranking, query decomposition and VLM-based
  ingestion of diagrams, on a Qdrant vector store.
- Designed an **agentic troubleshooting system** for network captures: the LLM proposes filters,
  deterministic code executes them, and the agent identifies the first anomaly and the component responsible.
- Automated the **generation of verification criteria** from a test-scenario description alone, with every
  generated check verified against the data.
- Built data-processing pipelines that structure raw network-capture data for automated anomaly detection.

**AI Research Intern — Inria, PETSCraft team** · Saclay · *May – Sep 2025*
- Developed invisible **text watermarking** to protect sensitive documents and audit unauthorised use in LLMs.
- Fine-tuned open-source LLMs (Mistral, LLaMA, Qwen) with **LoRA** on watermarked data and evaluated
  traceability and provenance, with a methodology for watermark retention, leakage and robustness.

## 📄 Publication

**Data Provenance Auditing of Fine-Tuned LLMs with a Text-Preserving Technique** — *ICML 2026* (co-author)

---

## 🚀 Projects

### 🩺 [Clinical Text-to-SQL Agent](https://github.com/S4IF-TP/Clinical-text-to-SQL-agent)
*Personal project · Python, LangGraph, PostgreSQL, FastAPI, Streamlit, Docker*
- Plain-English questions about patient records → **validated, read-only SQL**, the result and a short
  answer, with the SQL always shown. Runs over 2,000 synthetic patients ([Synthea](https://github.com/synthetichealth/synthea)).
- **Two independent safety layers:** a `sqlglot` validator and a read-only database role with a timeout;
  a guard refuses diagnosis / treatment requests; errors and empty results trigger self-correction.
- **Measured, not claimed:** 90-question benchmark with hand-written gold SQL (60 dev / 30 held-out),
  execution accuracy for 3 open-weight models. Baselines were already ~88–92% on the dev split, so I report
  the gain from self-correction as modest and single-run differences as noise.

### 🧪 [Synthetic Data Generation for RAG Systems](https://github.com/Aziz-Benamira/Synthetic-Data-Generation-for-RAG-Systems)
*Team project · ENSTA Paris, Agentic AI course 2025 · multi-agent LLM pipeline*
- A team pipeline that generates high-quality **question–answer pairs from scientific PDFs**, with a
  multi-agent critic (retry loop, hard rules) and a RAG evaluation suite (Hit@k, MRR, ROUGE-L, BERTScore,
  LLM-as-judge).
- **My contribution:** worked across the whole project (pipeline, critic, evaluation) and owned the
  **multimodal and difficulty** module: image extraction and vision-language captioning for figures, plus a
  question **difficulty estimator**, question-type classifier and diversity manager to annotate datasets.

### 🔌 [OpAmp Component Similarity](https://github.com/S4IF-TP/stmicro-component-similarity)
*Machine learning & deep learning · scikit-learn, LightGBM, PyTorch*
- Predicts similarity between **operational-amplifier components** from STMicroelectronics
  cross-reference data, to support component cross-referencing and finding alternative parts.
- Compared **Random Forest** and **LightGBM Ranker** against an **MLP with categorical embeddings**
  (supplier-package features) and custom distance metrics; produces similarity matrices and a demo UI.

### 🏦 [Bank Customer Churn Prediction](https://github.com/S4IF-TP/ML-Bank-customer-churn-prediction)
*Machine learning · scikit-learn, XGBoost, LightGBM, imbalanced-learn*
- End-to-end pipeline with statistical feature selection (chi-square), **SMOTE** for class imbalance,
  hyper-parameter tuning and cross-validation across 7 classifiers, including a voting ensemble.
- Best model reaches **78% recall** on churners; age, number of products, activity status and geography
  were the main drivers, translated into retention recommendations.

---

## 🛠️ Skills

**LLM & RAG** &nbsp;
![RAG](https://img.shields.io/badge/-RAG-FF9F1C?style=flat-square)
![Hybrid search](https://img.shields.io/badge/-Hybrid%20search%20%26%20reranking-555?style=flat-square)
![Qdrant](https://img.shields.io/badge/-Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)
![LangGraph](https://img.shields.io/badge/-LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Hugging Face](https://img.shields.io/badge/-Hugging%20Face-F9A03C?style=flat-square&logo=huggingface&logoColor=white)
![LoRA](https://img.shields.io/badge/-LoRA%20fine--tuning-555?style=flat-square)

**Serving & deployment** &nbsp;
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![vLLM](https://img.shields.io/badge/-vLLM-555?style=flat-square)
![Ollama](https://img.shields.io/badge/-Ollama-000?style=flat-square&logo=ollama&logoColor=white)
![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**ML & data** &nbsp;
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/-XGBoost-189AB4?style=flat-square)
![Pandas](https://img.shields.io/badge/-Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/-NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MLflow](https://img.shields.io/badge/-MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)
![C/C++](https://img.shields.io/badge/-C%2FC%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)

**Certifications** · Machine Learning Specialization (Stanford) · Neural Networks and Deep Learning ·
Exploratory Data Analysis in Python
**Languages** · Arabic (native) · French (bilingual) · English (B2)

---

## 🔭 Currently

- Looking for opportunities in **AI / ML engineering**, especially LLM systems, RAG and trustworthy AI.

📫 Reach me on [LinkedIn](https://www.linkedin.com/in/seifeddine-ghozzi/) or at
[seifeddine.ghozzi@ensta.fr](mailto:seifeddine.ghozzi@ensta.fr).
