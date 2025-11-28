# NLP Customer Review Insight System (NDA-Protected Project)
### Topic Modelling • Emotion Analysis • LLM Insight Generation

---

## 🔒 NDA Notice

This project was originally developed for a **large UK-based fitness chain** as part of a commercial engagement.  
The real client name, proprietary datasets, internal identifiers and operational details are all **protected under NDA** and therefore **not included** in this repository.

To demonstrate the methodology, a **synthetic dataset** is provided.  
The modelling pipeline, topic modelling structure, insight generation workflow, and analytical logic **mirror the real client implementation**.

---

## 📌 Project Overview

This repository presents a full **end-to-end NLP system** for analysing thousands of customer reviews collected across multiple fitness club locations in the UK.  
The system supports business teams by:

- identifying recurring **customer concerns**  
- detecting **operational issues** across branches  
- quantifying **emotions & sentiment** from user-generated content  
- summarising findings via **LLM-driven insights**  
- enabling **location-level benchmarking**  

Originally, the solution was used by the client to enhance decision-making in customer experience, retention, staffing, and service quality.

---

## 🧠 Core Capabilities

### ✔ **Topic Modelling (BERTopic)**  
Using transformer-based embeddings, UMAP dimensionality reduction and HDBSCAN clustering, the system extracts meaningful customer themes from both structured and unstructured text.

### ✔ **Emotion & Sentiment Analysis**  
The pipeline includes multi-label emotion modelling (anger, joy, frustration, sadness, trust) and polarity detection.

### ✔ **Multi-source Review Integration**  
Synthetic versions of the original data reflect the structure of:

- Google Reviews  
- Trustpilot Reviews  

### ✔ **LLM-based Insight Generation**  
Falcon-7B (instruction-tuned) is used to transform raw topics and reviews into:

- actionable operational recommendations  
- management-level summaries  
- location-level insights  
- comparative analysis across branches

---

## 🏗 Architecture Overview

The system follows a modular, enterprise-style NLP architecture designed for
scalability, interpretability and extensibility.

            ┌────────────────────────────────────────┐
            │          Data Sources (Synthetic)      │
            │────────────────────────────────────────│
            │  • Google Reviews (synthetic mirror)   │
            │  • Trustpilot Reviews (synthetic mirror│
            └────────────────────────────────────────┘
                               │
                               ▼
            ┌────────────────────────────────────────┐
            │        Data Preprocessing Layer        │
            │────────────────────────────────────────│
            │  • Cleaning & deduplication            │
            │  • Language filtering                  │
            │  • Custom domain stopwords             │
            │  • Tokenisation & normalisation        │
            └────────────────────────────────────────┘
                               │
                               ▼
            ┌────────────────────────────────────────┐
            │      Embedding & Topic Modelling       │
            │────────────────────────────────────────│
            │  • SentenceTransformers embeddings     │
            │  • UMAP dimensionality reduction       │
            │  • HDBSCAN clustering                  │
            │  • BERTopic topic extraction           │
            └────────────────────────────────────────┘
                               │
                               ▼
            ┌────────────────────────────────────────┐
            │   Emotion & Sentiment Classification   │
            │────────────────────────────────────────│
            │  • Polarity detection                  │
            │  • Emotion modelling (anger, joy, etc.)│
            └────────────────────────────────────────┘
                               │
                               ▼
            ┌────────────────────────────────────────┐
            │       LLM Insight Generation Layer     │
            │────────────────────────────────────────│
            │  • Falcon-7B summarisation             │
            │  • Actionable CX recommendations       │
            │  • Location-level reporting            │
            └────────────────────────────────────────┘
                               │
                               ▼
            ┌────────────────────────────────────────┐
            │            Final Outputs               │
            │────────────────────────────────────────│
            │  • Topic summaries                     │
            │  • CX insights per branch              │
            │  • Emotion patterns                    │
            │  • Management-ready LLM summaries      │
            └────────────────────────────────────────┘
---

## 📊 Example Insights (Synthetic Demonstration)

Even with synthetic data, the system demonstrates:

- overcrowding issues in several peak-hour locations  
- recurrent equipment maintenance complaints  
- dissatisfaction with response times of support teams  
- consistent praise for new facilities and updated machines  
- mismatches between high ratings and negative comments (sentiment drift)  

These patterns mirror typical multi-location service businesses and illustrate the system’s business impact.

---

## 🚀 Business Impact

The real client used this solution to:

- measure **operational consistency** across 50+ locations  
- identify **branches with declining customer satisfaction**  
- prioritise **maintenance & staffing needs**  
- support **CX improvement initiatives**  
- produce weekly reports for regional managers via LLM  
- inform retention strategy and membership engagement actions  

This project demonstrates the value of combining **advanced NLP** with **domain-specific insight generation** in a real business context.

---

## 🛠 Tech Stack

- Python  
- BERTopic  
- SentenceTransformers  
- Falcon-7B (HuggingFace)  
- spaCy  
- NLTK  
- Matplotlib / Seaborn  
- Pandas  
- UMAP / HDBSCAN  

---

## 🧩 Future Extensions

- Deploy as an interactive dashboard (Streamlit / Dash)  
- Build an n8n-based agent workflow (agentic AI)  
- Add automated anomaly detection for location-level trends  

---

## ✨ Author

Developed as part of an NDA-protected client engagement and refined for public demonstration.  
For collaboration or consulting inquiries, please contact via LinkedIn or GitHub.
