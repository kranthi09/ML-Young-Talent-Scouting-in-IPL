# 🏏 Future IPL Stars - A Data-Driven Talent Scouting Model

## 📌 Project Overview

This project aims to identify **future star batsmen** in the **Indian Premier League (IPL)** using a data-driven approach. By leveraging **machine learning (Random Forest)** and performance analytics from IPL ball-by-ball data, the model classifies young elite batsmen into roles such as **Top Order**, **Middle Order**, and **Finisher** based on their phase-wise performance metrics.

---

## 🎯 Objectives

- Identify emerging IPL batsmen who debuted after 2020.
- Filter elite players using:
  - Strike Rate > 130
  - Less than 60 matches played
  - More than 400 career runs
- Engineer features based on **Powerplay**, **Middle**, and **Death overs**.
- Use **Random Forest Classifier** to classify players into tactical roles.
- Support data-driven scouting and auction decisions for IPL franchises.

---

## 📁 Files Included

- `final_code_01.ipynb` – Jupyter notebook with full data preprocessing, feature engineering, and model training.
- `deliveries.csv` & `matches.csv` – IPL datasets used for analysis (source: Kaggle).
- `x23288892_future_ipl_stars.pptx` – Final presentation slides.
- `Domain_Report.pdf` – Project report explaining methodology, findings, and business value.
- `README.md` – Project overview and instructions.

---

## 📊 Dataset

- Source: [Kaggle IPL Complete Dataset](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)
- `matches.csv`: Match-level metadata (teams, venue, result, season)
- `deliveries.csv`: Ball-by-ball data (runs, overs, players, dismissals)

---

## 🔍 Methodology

1. **Data Cleaning & Merging**
   - Merged `matches.csv` and `deliveries.csv` to align player stats with debut years.

2. **Feature Engineering**
   - Calculated **strike rate**, **boundary %**, and **dot ball %** for each player across:
     - Powerplay (1–6 overs)
     - Middle overs (7–15)
     - Death overs (16–20)

3. **Elite Player Filtering**
   - Filtered players who:
     - Played < 60 matches
     - Scored > 400 runs
     - Had SR > 130
     - Debuted in or after 2020

4. **Model Training**
   - Used **Random Forest Classifier**
   - Stratified 80-20 train-test split
   - Evaluated using accuracy, F1-score, and feature importance

---

## ✅ Results

- **Accuracy**: 83%
- Successfully classified young elite players into roles:
  - Top Order
  - Middle Order
  - Finisher
- Identified future stars like **Rinku Singh**, **Tim David**, and **Jitesh Sharma**

---

## 🔒 Ethical Considerations

- **Data Privacy**: Only public IPL data used
- **Fairness**: Model supports human judgment, doesn’t replace it
- **Bias Risk**: Acknowledges possible exclusion of late bloomers
- **Transparency**: Uses interpretable ML techniques (feature importance)
- **Responsible Use**: Encourages human oversight in decision-making

---

## 🚀 Future Improvements

- Integrate match context (venue, opposition)
- Include psychological and pressure metrics
- Deploy as a **Streamlit dashboard** for live scouting insights
- Use more advanced models like XGBoost or SHAP explainability

---

## 📬 Contact

**Author**: Kranthi Kumar Yedla  
**Email**: x23288892@student.ncirl.ie  
**Program**: MSc in Data Analytics, National College of Ireland

---

