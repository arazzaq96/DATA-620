
# 📧 Spam Classification using UCI Spambase Dataset

This project is part of the DATA 620 course and focuses on building a spam detection model using the [UCI Spambase dataset](https://archive.ics.uci.edu/dataset/94/spambase). The goal is to classify emails as spam or ham (not spam) based on word and character frequency features.

## 📁 Dataset

- **Source**: UCI Machine Learning Repository
- **Records**: 4,601 emails
- **Features**: 57 numeric features (word & character frequencies) + 1 target label (`is_spam`)
- **Target**: `is_spam` (1 = spam, 0 = not spam)

## 🔍 Project Steps

1. **Data Loading & Cleaning**
   - Loaded `spambase.data` and assigned correct feature names from `spambase.names`.
   - Confirmed no missing values or duplicates.

2. **Exploratory Data Analysis**
   - Visualized class distribution.
   - Used descriptive statistics and a correlation heatmap to understand feature behavior.

3. **Train-Test Split**
   - 70/30 split with stratification to preserve spam-ham ratio.

4. **Model Building**
   - Trained two models: Naive Bayes and Random Forest.
   - Evaluated performance using accuracy, precision, recall, F1-score, and ROC-AUC.

5. **Feature Importance**
   - Extracted and visualized most predictive features from the Random Forest model.

## 📈 Results

- **Random Forest** achieved the best performance, particularly in minimizing false positives.
- Most predictive features:
  - `capital_run_length_total`
  - `char_freq_$`
  - `word_freq_free`
  - `char_freq_!`
  - `word_freq_remove`

## ✅ Conclusion

The project shows that Random Forest is highly effective for spam detection using engineered word and character frequency features. Future improvements could include experimenting with more models (e.g., XGBoost) or using raw email text with NLP techniques.

## 🛠️ Tools Used

- Python, Jupyter Notebook
- pandas, matplotlib, seaborn
- scikit-learn

---

**Author**: Ariba Razzak  
**Course**: DATA 620 — Natural Language Processing  
