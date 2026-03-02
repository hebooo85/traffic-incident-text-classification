# Smart Traffic Alert System – NLP Text Classification

## 📌 Overview
This project builds a Natural Language Processing (NLP) pipeline to automatically classify traffic accident reports into:
- Collision
- Other incidents

The goal is to support intelligent traffic management systems by enabling faster incident prioritization.

---

## 🎯 Problem Statement
Traffic accident reports are often submitted manually or through text systems.  
Manual review is slow and can delay emergency response.

This project uses machine learning to automatically classify accident reports in real time.

---

## 📊 Dataset
- Source: DSTI Traffic Accident Reports (Hugging Face)
- Original size: 800 reports
- Filtered size: 629 reports
- Binary labels:
  - 1 = Collision
  - 0 = Other

---

## 🧹 Text Preprocessing
- Lowercasing
- Removing punctuation
- Cleaning special characters
- Extracting accident category from text

---

## 🔢 Feature Engineering
- TF-IDF Vectorization
- ngram_range = (1,2)
- max_features = 5000

---

## 🤖 Model
Multinomial Naive Bayes

---

## 📈 Results
- Test Accuracy: **73.8%**
- Balanced Precision & Recall across classes
- Confusion Matrix visualization included
- Top predictive words analyzed using log probabilities

---

## 🔍 Key Insights
The model learned meaningful traffic-related indicators:

Collision indicators:
- "collision"
- "rear-end"
- "intersection"

Other indicators:
- "rollover"
- "pedestrian"
- "lane"

---

## 🛠 Tools & Libraries
- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Hugging Face Datasets

---

## 🚀 Future Improvements
- Compare with Logistic Regression & SVM
- Implement LSTM or Transformer-based model
- Deploy as real-time traffic alert API
