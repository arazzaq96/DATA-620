# Project 3: Name Gender Classification using NLTK

**Course**: DATA 620  
**Student**: Ariba Mandavia  

## 📌 Objective

The goal of this project is to classify the gender (male or female) of a person based on their first name using the NLTK Names Corpus. We apply various NLP classification techniques to analyze linguistic features of names and evaluate different models.

## 🧾 Dataset

We use the `names` corpus from the Natural Language Toolkit (NLTK), which includes:

- 2,948 male names
- 5,094 female names

The data is randomly shuffled and split as follows:
- **Training set**: ~6,400 names
- **Dev-test set**: 500 names
- **Test set**: 500 names

## ⚙️ Feature Engineering

We extract the following features from each name:
- First letter
- Last letter
- Last 2 and 3 characters (suffixes)
- Number of vowels
- Name length

These features capture known linguistic patterns associated with name gender classification.

## 🧠 Models Used

We trained and compared the following classifiers:
- **Naive Bayes**: Probabilistic model assuming feature independence
- **Decision Tree**: Rule-based classifier using decision paths
- **Maximum Entropy (MaxEnt)**: Logistic regression-based model
- **Ensemble Classifier**: Majority voting among all three models

We also performed 5-fold cross-validation on the Naive Bayes classifier to assess generalizability.

## 📊 Results

| Classifier           | Dev-Test Accuracy | Test Accuracy |
|----------------------|-------------------|---------------|
| Naive Bayes          | 78.2%             | 81.0%         |
| Decision Tree        | 73.4%             | 73.0%         |
| MaxEnt               | 79.6%             | 82.2%         |
| **Ensemble**         | 79.6%             | 81.4%         |

**Cross-Validated Naive Bayes Accuracy**: 79.8%

## ✅ Conclusion

- MaxEnt performed best, achieving over 82% accuracy.
- Ensemble slightly improved stability.
- Most informative features (e.g., suffix "na", "ia", "us") aligned with expected gender patterns.
- Even simple models can extract powerful insights from text-based features.

## 🔮 Future Work

- Expand to multilingual or culturally diverse name sets
- Apply deep learning or sequence models (e.g., LSTM, transformers)
- Create an interactive app or API for real-time predictions

