# Nashville Meetup Network Analysis

This repository explores **Nashville’s Meetup community** using network analysis, clustering, and machine learning.  
The goal is to uncover community interests, recommend groups to users, and predict event participation, helping strengthen connections between residents, entrepreneurs, and local businesses.  

---

## 📂 Project Structure

- `Code_Nashville_analysis` → Main analysis scripts (network building, clustering, recommendation, prediction).  
- `Datasets` → Meetup data (groups, members, events, participation).  
- `Project_Nashville_analysis.pdf` → Final report with methodology, results, and insights.   

---

## 📊 Dataset

The dataset contains **real Meetup data from Nashville** from **Kaggle**, including:  
- **Groups** → categories, descriptions, and activity levels.  
- **Members** → user profiles and group memberships.  
- **Events** → details of hosted meetups.  
- **Participation** → member attendance records.  

This combination enables analysis of **community structure**, **interest clusters**, and **engagement behaviors**.

---

## ⚙️ Workflow

### 1. Network Analysis
- Constructed a **member–group bipartite network**.  
- Projected into a **group–group network** to identify overlapping communities.  
- Applied **modularity-based clustering** to detect natural interest groups.  

### 2. Recommendation System
- Built a **content + collaborative filtering hybrid system**:  
  - Suggests groups to members based on **shared participation patterns** and **topic similarity**.  

### 3. Predictive Modeling
- Framed event participation as a **binary classification problem**.  
- Trained multiple models, including **Logistic Regression**, **Random Forest**, and **XGBoost**.  
- Best performance: **XGBoost with AUC ≈ 0.82**, indicating strong predictive power.  

---

## 📈 Results & Insights

- Nashville Meetup groups naturally clustered into communities like **Tech & Startups**, **Music & Arts**, **Outdoors & Fitness**, and **Food & Socializing**.  
- Members are more likely to attend events when:  
  - They belong to multiple overlapping groups.  
  - Events align with **popular community clusters**.  
- The recommendation system highlights **niche groups** that members may overlook but fit their interests.  

---

## 🛠️ Tech Stack

- **Language:** Python  
- **Libraries:** pandas, scikit-learn, networkx, matplotlib, xgboost  
- **Techniques:** Graph analysis, modularity clustering, hybrid recommendations, classification (XGBoost, Random Forest, Logistic Regression)  

---

## 📘 References

This project was developed as part of a group project on **social network analysis** and applied machine learning for community insights.  

