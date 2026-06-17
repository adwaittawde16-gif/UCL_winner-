# 🏆 UEFA Champions League Winner Predictor

A machine learning pipeline that predicts the UEFA Champions League winner using historical UCL season data (2000–2024), team statistics, and knockout-stage performance metrics.

---

## 🚀 Demo

> *[Live App](https://github.com/adwaittawde16-gif/UCL_winner-)* · Built with Streamlit

---

## 📌 Features

- Predicts UCL winner from group-stage + knockout-round stats
- Users input club statistics → receive ranked winner probability per team
- Handles severe class imbalance (1 winner per 32+ clubs per season)
- Interactive Streamlit UI for live predictions

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| XGBoost | Classification model |
| scikit-learn | Preprocessing, cross-validation |
| SMOTE | Class imbalance handling |
| Pandas / NumPy | Data processing |
| Streamlit | Web app |
| Web Scraping + Football APIs | Data ingestion |

---

## 📂 Project Structure

```
UCL_winner/
├── data/
│   ├── raw/           # Scraped / API data
│   └── processed/     # Cleaned feature sets
├── notebooks/
│   └── eda.ipynb      # Exploratory analysis
├── src/
│   ├── features.py    # Feature engineering
│   ├── model.py       # Training & evaluation
│   └── predict.py     # Inference logic
├── app.py             # Streamlit app
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup & Run

```bash
git clone https://github.com/adwaittawde16-gif/UCL_winner-.git
cd UCL_winner-
pip install -r requirements.txt
streamlit run app.py
```

---

## 📊 Features Used

- Goals scored / conceded (group + knockout stages)
- Squad market value
- Historical UCL win rate per club
- Knockout-stage form and progression stats
- Head-to-head records
- Home / away performance differential

---

## 🧠 ML Pipeline

- **Model:** XGBoost classifier
- **Baseline:** Random Forest
- **Class imbalance:** SMOTE + stratified cross-validation
- **Feature selection:** Iterative selection to reduce leakage
- **Evaluation:** Winner recall, ROC-AUC, F1

---

## 🔮 Future Work

- [ ] Add player-level stats (injuries, top scorers)
- [ ] Real-time data pipeline
- [ ] Bracket simulation mode
- [ ] Probabilistic output per team across full draw

---

## 📄 License

MIT License
