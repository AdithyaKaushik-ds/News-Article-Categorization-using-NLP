# News-Article-Categorization-using-NLP

This repository presents a natural language processing (NLP) case study focused on classifying news articles into distinct categories such as Politics, Business, Sports, Entertainment, and Technology. The primary objective is to improve content relevance and personalization for users.

## 📂 Dataset Description

The dataset contains:
- **Article**: Full text of the news article.
- **Category**: The target class representing the topic.

There are 2,225 news articles distributed across 5 categories.

## 📊 Exploratory Data Analysis (EDA)

- Assessed category-wise distribution of news.
- Identified dominant categories (e.g., Business, Sports).
- Visualized class balance using count plots.
- Examined common words and vocabulary across articles.

## 🧹 Text Preprocessing

Steps included:
- Removal of non-alphabet characters.
- Conversion to lowercase.
- Tokenization and stopword removal.
- Lemmatization using `WordNetLemmatizer`.

## 🛠️ Feature Engineering

- Transformed articles using **Bag-of-Words** and **TF-IDF**.
- Encoded target labels using `LabelEncoder`.

## 🔍 Model Building and Evaluation

Implemented and evaluated the following models:
- **Naive Bayes**: Achieved highest accuracy (≈ 95.9%)
- **SGD Classifier**: Achieved ≈ 96.8% accuracy
- **Logistic Regression**: ≈ 96.6% accuracy
- **Decision Tree**: ≈ 84.7% accuracy
- **K-Nearest Neighbors**: ≈ 59.3% accuracy
- **Random Forest**: ≈ 85.6% accuracy

Evaluation metrics used:
- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix

## 📈 Key Findings

- **Naive Bayes** performed best across metrics and categories.
- Balanced precision and recall observed, making it suitable for multi-class problems.
- TF-IDF representation improved model performance.

## 🔁 Recommendations

- Address category imbalance with resampling or class weights.
- Experiment with BERT/Transformer-based models for further improvement.
- Integrate user feedback loops for continuous model refinement.
