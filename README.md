# 📺 Streaming Service Churn Prediction

A machine learning web app that predicts whether a streaming service user is likely to cancel their subscription (churn), built with Python, scikit-learn, and Streamlit.

## 🎯 Business Problem

Customer churn is one of the biggest cost drivers for subscription businesses. Losing a customer costs 5–7× more than retaining one. This app helps customer success teams identify **high-risk users before they leave**, so the business can act early — offer discounts, improve recommendations, or reach out proactively.

## 🚀 Live Demo

> Run locally with: `streamlit run churnapp.py`

## 📊 Dataset

- Source: [Kaggle – Streaming Service Churn Dataset](https://www.kaggle.com/)
- Domain: Video streaming platform (similar to Netflix)
- Features include: user demographics, watch behavior, subscription plan, device type, IMDb ratings of watched content

## 🔧 Features Used

| Feature | Description |
|---|---|
| `age` | User age |
| `monthly_spend` | Monthly subscription spend ($) |
| `tenure_days` | Days since first subscription |
| `total_watch_events` | Total number of viewing sessions |
| `total_watch_minutes` | Total minutes watched |
| `avg_watch_minutes` | Average session length |
| `unique_movies_watched` | Content variety |
| `avg_imdb_watched` | Average IMDb rating of watched content |
| `share_high_imdb` | Share of high-quality content watched |
| `gender`, `country` | User demographics |
| `subscription_plan` | Standard / Premium / Premium+ |
| `primary_device` | Laptop / Mobile / Smart TV / Tablet / Gaming Console |

## 🤖 Model

- **Algorithm:** K-Nearest Neighbors (KNN) Classifier
- **Library:** scikit-learn
- **Output:** Probability of churn (0–100%)
- **Risk levels:**
  - 🔴 High risk: ≥ 60%
  - 🟡 Medium risk: 30–59%
  - 🟢 Low risk: < 30%

## 📁 Project Structure

```
churn-prediction/
├── churnapp.py           # Streamlit web app
├── knn_model.pkl         # Trained KNN model
├── feature_columns.json  # Feature schema for prediction
├── requirements.txt      # Python dependencies
└── README.md
```

## ⚙️ How to Run

```bash
# 1. Clone the repo
git clone https://github.com/mikimetov-mba/churn-prediction.git
cd churn-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the app
streamlit run churnapp.py
```

## 💡 Key Insights

- Users with **low watch time** and **short tenure** show the highest churn risk
- **Premium+ subscribers** churn less than Standard plan users
- **Mobile-first users** tend to have higher churn rates than Smart TV users
- Content quality (avg IMDb score) is a strong retention signal

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)

## 👤 Author

**Mukhammedjan Ikmetov** — MBA candidate | Data Scientist | Business Consultant  
[GitHub](https://github.com/mikimetov-mba) · [LinkedIn](#)

---

*Part of a portfolio combining business consulting expertise with data science.*
