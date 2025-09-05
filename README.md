# 🏏 Virat Kohli Century Match Outcome Prediction

Predicting the result of cricket matches (🏆 Won, ❌ Lost, ⚪ Drawn) based on whether Virat Kohli scored a century, along with match features like Teams, Format, Batting Position, Venue, and Ground (Home/Away/Neutral).

---

## 📖 Project Overview

This project analyzes and predicts cricket match outcomes using historical data of Virat Kohli's centuries. The model predicts whether the match was **🏆 Won, ❌ Lost, or ⚪ Drawn** based on match features.

**Target Variable:** `Match_Result`  
- ⚪ 0 → Draw  
- ❌ 1 → Lost  
- 🏆 2 → Won  

**Features Used:**
- 🏟️ `Format` → Test/ODI/T20  
- 🏏 `Team` → Opponent team  
- 🎯 `Position` → Virat’s batting position  
- 🌍 `Venue` → Stadium or city  
- 🏠/✈️ `Ground` → Home / Away / Neutral  
- 💯 `Virat_Century` → 1 if century scored, 0 otherwise  

---

## 🛠️ Models Used

### 1️⃣ Logistic Regression
- ✅ Train Accuracy: **0.76**  
- ✅ Test Accuracy: **0.72**  
- 👍 Pros: Simple, interpretable, minimal overfitting  
- ⚠ Cons: Struggles with non-linear relationships; lower recall for Draw/Lost

---

## 📊 Feature Importance (Decision Tree)

| Feature   | Importance |
|-----------|------------|
| 🏟️ Format    | 0.411      |
| 🏠 Ground    | 0.165      |
| 🎯 Position  | 0.112      |
| 🏏 Team      | 0.087      |
| 🌍 Venue     | 0.029      |

**Insight:**  
- Format and Ground dominate predictions.  
- Batting position and opponent team moderately affect results.  
- Venue has minimal impact.

---

## 📈 Evaluation Metrics (Logistic Regression)

| Class  | Precision | Recall | F1-score | 
|--------|-----------|--------|----------|
| ⚪ Draw (0) | 1.00     | 0.50   | 0.67     | 
| ❌ Lost (1) | 1.00     | 0.14   | 0.25     | 
| 🏆 Won (2)  | 0.70     | 1.00   | 0.82     | 

- **Accuracy:** 0.72

---

**Interpretation:**  
- Model predicts Wins (🏆) very accurately.  
- Struggles to predict Draws (⚪) and Losses (❌) due to class imbalance.

---

## 💡 Recommendations
- Use `class_weight='balanced'` to handle class imbalance.  
- Include features like opponent strength, recent form, toss outcome, pitch conditions.  
- Try ensemble models (Random Forest, Gradient Boosting) to improve accuracy and recall for minority classes.

---

## ✅ Conclusion
- Baseline models achieved **72% accuracy**.  
- Logistic Regression is stable and interpretable.  
- Decision Tree provides feature importance insights.  
- Further improvements can be made using ensemble methods and additional features.

---

## 👤 Author
**Aldous Dsouza**  
BSc Computer Science | Data Science & Software Development Enthusiast
