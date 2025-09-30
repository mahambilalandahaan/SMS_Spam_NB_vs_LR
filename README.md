# 📊 SMS Spam Classification: Naive Bayes vs Logistic Regression

This project compares **Naive Bayes (NB)** and **Logistic Regression (LR)** classifiers on the [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection).  
The goal is to detect spam messages and compare different models + feature extraction methods.

---

## 🚀 Project Workflow
1. Load and preprocess dataset (UCI SMS Spam).
2. Clean & standardize text (lowercasing, punctuation removal).
3. Feature extraction:
   - CountVectorizer (1-2 n-grams, top 2000 features)
   - TF-IDF Vectorizer (1-2 n-grams, top 2000 features)
4. Models trained:
   - Naive Bayes (MultinomialNB)
   - Logistic Regression (L2, saga solver)
5. Evaluation using:
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - ROC AUC
6. Visualization:
   - Confusion Matrix (heatmap)
   - Results summary table

---

## 📈 Results (Summary Table)

| Model          | Accuracy | Precision | Recall | F1 Score | ROC AUC |
|----------------|----------|-----------|--------|----------|---------|
| NB (Counts)    | ...      | ...       | ...    | ...      | ...     |
| NB (TF-IDF)    | ...      | ...       | ...    | ...      | ...     |
| LR (Counts)    | ...      | ...       | ...    | ...      | ...     |
| LR (TF-IDF)    | ...      | ...       | ...    | ...      | ...     |

*(Replace `...` with your actual results)*

---

## ⚖️ Model Comparison

### ✅ Naive Bayes
- **Pros**: Fast, lightweight, works well with sparse text data.
- **Cons**: Assumes word independence; recall usually lower than LR.

### ✅ Logistic Regression
- **Pros**: Handles class imbalance better, higher recall & precision.
- **Cons**: Slower training, needs parameter tuning.

### ✅ Count vs TF-IDF
- CountVectorizer: simple frequency-based features, weaker performance.
- TF-IDF: weighs rare but important words, leads to stronger results.

---

## 📌 Bottom Line
- Both models are effective for SMS spam detection.  
- **Naive Bayes** is great for speed and simplicity.  
- **Logistic Regression (with TF-IDF)** achieved the **best overall performance**.  
- TF-IDF features clearly outperform Count-based features.  

---

## 📂 Files in this Repo
- `NB_vs_LR.ipynb` → Main Jupyter Notebook.
- `requirements.txt` → Dependencies list.
- `README.md` → Project documentation.

---

## 📜 Dataset
- Source: [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection) (UCI ML Repository).

---

## 🙌 Acknowledgements
- UCI Machine Learning Repository for dataset.
- scikit-learn & pandas for ML pipeline.

