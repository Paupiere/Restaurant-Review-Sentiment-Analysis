# 🍽️ Sentiment Analysis of Google Reviews
### Restaurants in Majitar, East Sikkim (PIN: 737136)

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange?logo=scikit-learn)
![NLP](https://img.shields.io/badge/NLP-Sentiment%20Analysis-green)
![Assignment](https://img.shields.io/badge/B.Tech-NLP%20Assignment-purple)

---

## 📌 Overview

This project performs **Sentiment Analysis** on real Google Reviews from restaurants in **Majitar, East Sikkim, India**.  
Each review is automatically classified as **Positive** or **Negative** using classical Machine Learning techniques.

> **B.Tech NLP Assignment** — Text Analysis and Natural Language Processing

---

## 📁 Project Structure

```
├── Sentiment_Analyzer.ipynb           # Main Python script (fully commented)
├── dataset.csv                        # 40 Google reviews with sentiment labels
├── requirements.txt                   # Python dependencies
└── README.md                          # This file
```

---

## 🧠 Techniques Used

| Component | Details |
|-----------|---------|
| **Preprocessing** | Lowercasing, removing punctuation/numbers, NLTK Stopword removal |
| **Feature Extraction** | TF-IDF (Term Frequency – Inverse Document Frequency) |
| **Model** | Logistic Regression |
| **Evaluation** | Accuracy, Precision, Recall, F1-Score |

---

## 📊 Dataset

- **Location**: Majitar, East Sikkim (PIN: 737136)
- **Total Reviews**: 40 (8 Local Restaurants)
- **Classes**: `positive` (1) · `negative` (0)

| Sentiment | Count | Share |
|-----------|-------|-------|
| Positive  | 24    | 60%   |
| Negative  | 16    | 40%   |

> ⚠️ **Class Imbalance**: The dataset is slightly skewed toward positive reviews, which is typical of real-world dining feedback.

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/your-username/sentiment-majitar.git
cd sentiment-majitar
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the model**
```bash
python Sentiment_Analyzer.ipynb
```

---

## 📈 Sample Output

```text
=========================================
      MODEL PERFORMANCE EVALUATION       
=========================================
Accuracy:  0.67
Precision: 0.67
Recall:    1.00
F1-Score:  0.80
=========================================


Available Restaurants: Punjabi Kitchen, Grill and Chill Majhitar, Coffee Break, Imperfecto Restro, Down Town Restro, Lounge 88, Paddington, Biryani Kitchen

Enter a restaurant name from the list above: Imperfecto Restro

--- Analyzing Reviews for: Imperfecto Restro ---

Review: "Fresh and delicious food with authentic cuisine. Clean and well-maintained."
Predicted Sentiment: Positive

Review: "Very bad experience. The place was dirty and noisy."
Predicted Sentiment: Positive

Review: "Highly recommend this restaurant for a great dining experience."
Predicted Sentiment: Positive

Review: "Overpriced and small portions. Not worth the hype."
Predicted Sentiment: Negative

Review: "The staff was very courteous and the ambiance is superb."
Predicted Sentiment: Positive
```

---

## ⚠️ Limitations

- Small dataset constraint (40 reviews) — results are primarily for academic demonstration.
- The model occasionally struggles with implicitly negative reviews due to the limited training size.
- Classical Logistic Regression used; Transformer-based models (like BERT) would yield higher accuracy on complex sentence structures.

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **pandas** — data manipulation
- **numpy** — array operations
- **scikit-learn** — TF-IDF vectorization, Logistic Regression, evaluation metrics
- **nltk** — stopword removal
- **re** (built-in) — regex text cleaning

---

## 📚 References

- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [NLTK Documentation](https://www.nltk.org/)
- Manning, Raghavan & Schütze — *Introduction to Information Retrieval*

---

## 👩‍💻 Author

**PALAK AGARWAL** · Register No: - 202300292  
B.Tech — CSE(DS)  
Course: Text Analysis and Natural Language Processing | 2023-2027  

Sikkim Manipal Institute of Technology  
Majitar, East Sikkim, India
