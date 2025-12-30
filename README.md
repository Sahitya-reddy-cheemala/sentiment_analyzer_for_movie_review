# 🎬 Movie Review Sentiment Analysis (BoW vs TF-IDF)

This project demonstrates a **basic Natural Language Processing (NLP) sentiment analysis pipeline** using **scikit-learn**.  
It classifies movie reviews as **positive** or **negative** using traditional machine learning techniques.

---
## ⚙️ Project Workflow

1. **Data Collection**
   - A small dataset of movie reviews is manually created.
   - Each review is labeled as:
     - `1` → Positive
     - `0` → Negative

2. **Text Preprocessing**
   - Convert all text to lowercase.
   - Remove stop words (e.g., *the, is, and*).
   - Tokenize text into individual words.
   - This is handled internally by `CountVectorizer` and `TfidfVectorizer`.

3. **Feature Extraction**
   - **Bag of Words (BoW)**:
     - Converts text into word frequency vectors.
     - Ignores word order.
   - **TF-IDF**:
     - Weighs words based on importance.
     - Penalizes common words and highlights informative ones.

4. **Train-Test Split**
   - Dataset is split into:
     - 70% training data
     - 30% testing data
   - Stratified splitting ensures balanced class distribution.

5. **Model Training**
   - A **Logistic Regression** classifier is trained using:
     - BoW features
     - TF-IDF features
   - The model learns patterns associated with positive and negative sentiment.

6. **Model Evaluation**
   - Predictions are made on test data.
   - Performance is measured using:
     - Precision
     - Recall
     - F1-score
     - Accuracy
   - Confusion matrices are used to visualize prediction results.

7. **Sentiment Prediction**
   - New, unseen movie reviews are processed using the trained TF-IDF model.
   - The model predicts:
     - Sentiment label (positive or negative)
     - Probability/confidence score

8. **Result Comparison**
   - Performance of BoW and TF-IDF models is compared.
   - TF-IDF typically provides better generalization on text data.

- 


