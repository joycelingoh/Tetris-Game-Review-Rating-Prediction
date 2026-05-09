# **Tetris Game Review Rating Prediction**

This project was developed as a midterm project for the Text Mining course, focusing on sentiment and rating prediction using user reviews from the Tetris mobile game on Google Play Store. The objective was to analyze user-generated text reviews and build machine learning models capable of predicting review ratings based on textual patterns and sentiment. 

## **Project Overview**

The dataset consisted of 2,000 English-language Tetris game reviews scraped directly from Google Play Store using the `google-play-scraper` library. The analysis included exploratory text analysis, preprocessing, feature extraction, and comparison of multiple machine learning and deep learning models for multiclass rating prediction.

The project explored how different text representation techniques and classification algorithms perform on imbalanced review data.

**Dataset Features:**

* User Review Text
* Review Rating (1–5 stars)

---

## **Key Insights**

* The dataset was highly imbalanced, with the majority of reviews belonging to the 1-star category.
* Common negative terms such as **“ads”**, **“offline”**, and **“many ads”** frequently appeared in low-rated reviews.
* Positive reviews were generally shorter and contained words such as **“fun”**, **“good”**, and **“great game.”**
* Users often complained about excessive advertisements and offline mode limitations.
* Lower ratings tended to have significantly longer review lengths, indicating detailed complaints from dissatisfied users.

**Best Model Performance:**

* **TF-IDF + Random Forest**

  * Accuracy: **62.5%**
  * Weighted F1-Score: **0.537**
* **Word2Vec + CNN**

  * Accuracy: **61.5%**
  * Weighted F1-Score: **0.553**

The CNN model achieved the highest weighted F1-score among all evaluated models. 

---

## **Tools & Methods**

* Language: Python
* Libraries:

  * pandas
  * NumPy
  * NLTK
  * scikit-learn
  * TensorFlow / Keras
  * gensim
  * matplotlib
  * wordcloud

### Methods:

* Web scraping using Google Play Scraper
* Text preprocessing:

  * Lowercasing
  * Stopword removal
  * Lemmatization
  * Text normalization
* Exploratory Text Analysis (ETA)
* Word frequency analysis
* WordCloud visualization
* Bigram analysis
* TF-IDF vectorization
* Word2Vec embedding
* Machine Learning:

  * Logistic Regression
  * Random Forest
* Deep Learning:

  * LSTM
  * CNN
* Imbalanced data handling:

  * SMOTE
  * Class weighting

---

## **Results**

* Successfully scraped and analyzed 2,000 real-world mobile game reviews.
* Identified dominant user complaints related to advertisements and gameplay limitations.
* Compared traditional machine learning and deep learning approaches for multiclass text classification.
* TF-IDF-based models generally outperformed Word2Vec classical models in accuracy.
* CNN achieved stronger balanced performance compared to LSTM on imbalanced text data.
* SMOTE and class weighting improved minority class recognition but reduced overall accuracy in several models.

This project demonstrates practical experience in text mining, NLP preprocessing, sentiment analysis, feature engineering, and machine learning model evaluation using real-world textual data.

---

## **Future Work**

* Implement transformer-based models such as BERT for improved text understanding.
* Perform sentiment classification instead of direct rating prediction.
* Apply advanced imbalance handling techniques.
* Expand the dataset using reviews from multiple mobile games.
* Deploy the model as a web-based review analytics application.
