# streamlit-ml-nlp-review-app

An end-to-end Machine Learning and Natural Language Processing (NLP) intelligence platform built with **Scikit-Learn**, **HuggingFace Transformers**, and **Streamlit**. This dashboard ingests raw customer reviews, performs advanced sentiment analysis, extracts text-based feature metrics, and predicts customer recommendation intent.

---

## 🎯 Project Overview & Business Value
In e-commerce, customer retention hinges on understanding feedback at scale. This project provides businesses with a dual-purpose tool:
1. **Interactive Analytics Dashboard:** Aggregates and visualizes customer sentiments, rating distributions, and text metrics to pinpoint customer friction points.
2. **AI-Powered Review Simulator:** A real-time diagnostic playground where developers or business analysts can input raw review text and instantly run it through a multi-stage NLP and Machine Learning classification pipeline to predict customer churn/recommendation status.

---

## 🛠️ Tech Stack & Key Libraries
* **Frontend UI:** Streamlit (clean, interactive, and responsive)
* **Natural Language Processing (NLP):** HuggingFace `transformers` (`distilbert-base-uncased-finetuned-sst-2-english`)
* **Machine Learning:** Scikit-Learn (`RandomForestClassifier` for predictive modeling)
* **Data Engineering & Visualization:** Pandas, NumPy, Plotly
* **Model Serialization:** Joblib

---

## 📁 Repository Structure
Code output
SUCCESS

```text
streamlit-ml-nlp-review-app/
│
├── data/                          # Organized dataset storage
│   ├── raw/                       # Original, untouched Kaggle CSV
│   └── processed/                 # Engineered datasets (git-ignored)
│
├── models/                        # Serialized model artifacts
│   └── review_model.pkl           # Trained Random Forest Model (git-ignored)
│
├── notebooks/                     # Exploratory Phase
│   └── exploratory_analysis.ipynb # Data cleaning & visual prototyping
│
├── src/                           # Production Source Code
│   ├── __init__.py                
│   ├── data_preprocessing.py      # Feature engineering and data cleaning
│   ├── sentiment_engine.py        # HuggingFace Sentiment Pipeline
│   └── train_model.py             # Model training and metric evaluations
│
├── app.py                         # Streamlit Application Entrypoint
├── requirements.txt               # Dependencies
└── .gitignore                     # Tidy repository exclusions
