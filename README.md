# 🎬 Anime Recommendation System

## 🚀 Project Overview

This project builds a **content-based and collaborative filtering recommendation system** for anime, generating personalized recommendations for users and visualizing insights in **Power BI** for business and stakeholder analysis.

---

## 📈 Workflow

### 1️⃣ Data Loading & Preprocessing

- Load `` and ``.
- Clean missing values and correct data types.
- Extract **genre columns**.
- Encode categorical columns for modeling.

---

### 2️⃣ Content-Based Filtering

- Use **one-hot encoding** on genre features.
- Calculate **cosine similarity** between anime based on genre.
- Generate **top-N similar anime recommendations** for any given anime.

---

### 3️⃣ Collaborative Filtering

- Create a **user-item rating matrix** using `scipy.sparse`.
- Apply **TruncatedSVD** for dimensionality reduction.
- Generate **personalized top-N recommendations per user**.
- Evaluate using **RMSE, Precision\@K, Recall\@K**.

---

### 4️⃣ Saving Outputs

- Save **recommendations for 100 users** in `recommendations_all_users.csv`.
- Save **recommendation frequency** in `recommendation_frequency.csv`.
- Save **model evaluation metrics** in `model_metrics.csv` for Power BI analysis.

---

### 5️⃣ Power BI Dashboard

- Load `recommendations_all_users.csv`, `recommendation_frequency.csv`, and `model_metrics.csv`.
- Create:
  - User-specific and global recommendations table.
  - Genre distribution charts for recommended anime.
  - Cards for RMSE, Precision\@K, Recall\@K.
  - Recommendation frequency graphs.
  - (Optional) Heatmaps for user-item rating distributions.
- Add a **professional anime-themed background**.

---

## 🛠️ Tools & Libraries

- **Python**: pandas, numpy, sklearn, scipy, seaborn, matplotlib
- **Power BI Desktop** for dashboards
- **Jupyter Notebook** for iterative development

---

## 📂 Directory Structure

```
project/
│
├── data/
│   ├── anime.csv
│   ├── rating.csv
│   ├── recommendations_all_users.csv
│   ├── recommendation_frequency.csv
│   └── model_metrics.csv
│
├── notebooks/
│   └── 04_Modeling.ipynb
│
├── models/
│   └── truncated_svd_model.joblib
│
└── README.md
```

---

## 📌 Key Points for Stakeholders

- **Personalized Recommendations** to increase user engagement.
- **Genre Insights** to track trending genres in recommendations.
- **Performance Metrics** for iterative improvement.
- **Interactive Power BI Dashboard** for stakeholder presentation.

---

## ⚡ Future Extensions

- Add hybrid models combining content-based and collaborative filtering.
- Explore deep learning embeddings for improved recommendations.
- Incorporate time-based analysis for trending anime.

---

## 🖥️ Usage

Run the **Jupyter Notebook** `04_Modeling.ipynb` to generate:

- Recommendations for Power BI.
- Evaluation metrics for performance monitoring.
- Saved models for reproducibility.

Then, **open Power BI Desktop** to load the CSV outputs and create your interactive dashboard.

---

If you need a Power BI guide, model architecture diagram, or background image generation prompt for your dashboard, please let me know!
