# Multi-Class Sentiment Analysis (Traditional Models vs. BERT)

This project is entirely my own work, developed from scratch with careful attention to detail and learning at every stage. It explores multi-class sentiment classification using both traditional machine learning models and a lightweight BERT-based model. The classification covers three sentiment classes: Negative, Neutral, and Positive.

---

## 🔁 First Attempt – Traditional Machine Learning

In the first version of this project, I dedicated a significant amount of time to preprocessing and balancing the data to give classical models a fair chance. Here are the key steps:

### 🧹 Data Cleaning:
- Removed empty and extremely short or long sentences.
- Filtered out emojis-only texts and noisy patterns.
- Balanced the sentiment classes as best as possible.
- Carefully removed or kept certain stop words to avoid biasing the Neutral class toward Positive or Negative.

### 🧠 Models Used:
- Support Vector Machine (SVM)
- Logistic Regression (LogReg)
- Random Forest (RF)
- LSA + Random Forest

📉 Best result achieved: 66.78% accuracy

---

## 🔁 Second Attempt – Lightweight BERT

After realizing that classic preprocessing doesn't suit transformer models, I restarted the entire pipeline from scratch with BERT in mind. For this version:

### 🧹 BERT-Specific Cleaning:
- Avoided over-cleaning (BERT can handle emojis, URLs, etc.).
- Preserved text richness that helps contextual embedding.

### ⚙️ Model:
- A lightweight BERT variant was used due to hardware limitations.
- Trained with only 1 epoch.

📈 Achieved Accuracy: 75.23%

---

## ⚠️ Hardware Limitation

Although I wanted to further improve the results using more epochs, larger models, and better tuning, my personal computer is not powerful enough to handle full-scale training for longer durations (some runs exceeded 8 hours). Despite that, I managed to get competitive results with optimized resources.

---

## 📁 Project Structure
/ multi_sentiment_analysis
│
├── multi_sentiment_classification.ipynb # Traditional models
├── multi_sentiment_classifiction_bert_vertion.ipynb # Lightweight BERT version
├── README.md
--

## ✅ Conclusion

This project demonstrates how:
- Traditional models can give decent results with heavy preprocessing.
- BERT models, even lightweight ones, can outperform classical models with minimal cleaning, thanks to their contextual power.

---

## 📌 Notes
- Dataset contained noisy and imbalanced classes initially.
- Final results are impressive considering hardware constraints and single-epoch training.
- This work was completed independently as part of my learning journey in NLP.
  by:heitham bendjamaa
