# Emotion Detection from Text using Natural Language Processing (NLP)

## Project Overview

This project implements an **Emotion Detection System** using Natural Language Processing (NLP) and Machine Learning. The objective is to classify textual data into different emotion categories by applying text preprocessing, feature extraction techniques, and supervised learning algorithms.

The project compares the performance of multiple machine learning models and identifies the most accurate approach for emotion classification.

---

## Objectives

* Perform text preprocessing and cleaning.
* Convert text into numerical features.
* Train multiple machine learning models.
* Compare model performance.
* Predict emotions from unseen text.

---

## Dataset

**Dataset File:** `train.txt`

The dataset contains two columns:

* **Text:** Input sentence or statement.
* **Emotion:** Corresponding emotion label.

The emotion labels are converted into numerical values before training the models.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* NLTK
* Scikit-learn
* Jupyter Notebook

---

## Data Preprocessing

The following preprocessing techniques were applied:

* Converted text to lowercase.
* Removed punctuation.
* Removed numerical values.
* Removed emojis and non-ASCII characters.
* Removed English stop words using NLTK.
* Converted categorical emotion labels into numerical labels.

---

## Feature Extraction

Two feature extraction techniques were used:

### Bag of Words (CountVectorizer)

Converts text into vectors based on word frequency.

### TF-IDF (Term Frequency–Inverse Document Frequency)

Represents text by assigning weights to words according to their importance in the dataset.

---

## Machine Learning Models

### 1. Multinomial Naive Bayes (Bag of Words)

**Accuracy:** 76.81%

### 2. Multinomial Naive Bayes (TF-IDF)

**Accuracy:** 66.09%

### 3. Logistic Regression (TF-IDF)

**Accuracy:** 86.28%

Logistic Regression achieved the highest accuracy and was selected as the best-performing model.

---

## Model Comparison

| Model                   | Feature Extraction | Accuracy   |
| ----------------------- | ------------------ | ---------- |
| Multinomial Naive Bayes | Bag of Words       | 76.81%     |
| Multinomial Naive Bayes | TF-IDF             | 66.09%     |
| Logistic Regression     | TF-IDF             | **86.28%** |

---

## Project Workflow

1. Load the dataset.
2. Clean and preprocess the text.
3. Encode emotion labels.
4. Split the dataset into training and testing sets.
5. Extract text features using Bag of Words and TF-IDF.
6. Train machine learning models.
7. Evaluate model performance using accuracy.
8. Compare the results and select the best model.

---

## Results

* Successfully classified text into multiple emotion categories.
* Compared Bag of Words and TF-IDF feature extraction techniques.
* Logistic Regression with TF-IDF achieved the highest accuracy of **86.28%**.

---

## Future Improvements

* Apply stemming and lemmatization.
* Use Word2Vec or GloVe embeddings.
* Train deep learning models such as LSTM and GRU.
* Fine-tune transformer-based models such as BERT or RoBERTa.
* Deploy the model using Streamlit or Flask for real-time predictions.

---

## Project Structure

```text
Emotion-Detection/
│
├── train.txt
├── Emotion_Detection.ipynb
├── README.md
└── requirements.txt
```

---

## Author

**Jannat**

This project was developed to demonstrate the complete NLP pipeline, including text preprocessing, feature extraction, machine learning model training, and emotion classification using supervised learning techniques.
