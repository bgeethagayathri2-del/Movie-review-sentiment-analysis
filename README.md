# Movie Review Sentiment Analysis

Classifies movie reviews as positive or negative using NLP and machine learning.

- **Dataset:** NLTK Movie Reviews (2,000 reviews: 1,000 positive and 1,000 negative)
- **Method:** TF-IDF features using single words and two-word phrases, then two models
- **Results:**

| Model | Accuracy |
|---|---|
| Logistic Regression | 0.812 |
| Linear SVM | 0.833 |

- **Cross-validation accuracy (Logistic Regression):** 0.829
- **Most positive words:** great, life, war, family, best, excellent, truman, world, perfect, mulan
- **Most negative words:** bad, worst, plot, movie, boring, supposed, script, harry, stupid, waste
- **Conclusion:** Linear SVM was slightly better than Logistic Regression (83.3% vs 81.2%). The cross-validation score of 82.9% shows the result is stable across different splits. Words like "worst", "boring", "stupid" and "waste" clearly signal negative reviews, and "great", "best", "excellent" and "perfect" signal positive ones. Some words, such as "harry", "truman" and "mulan", are movie names rather than opinions. This shows the model also learns quirks of this particular dataset, so it may do worse on reviews of other movies.

## How to run
Open `Sentiment_analysis.ipynb` in Google Colab and click Run all.
