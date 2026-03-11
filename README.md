# Spam SMS Detection using Machine Learning

## Project Overview

This project builds a **Machine Learning model that classifies SMS messages as Spam or Ham (Not Spam)**.

The system uses **Natural Language Processing (NLP)** techniques to convert SMS text messages into numerical features and applies a **Multinomial Naive Bayes classifier** to detect spam messages automatically.

---

## Dataset

The dataset used for this project is the **SMS Spam Collection Dataset**.

Dataset details:

* **Total Messages:** 5572
* **Classes:** Spam and Ham (Not Spam)

Original dataset columns:

| Column     | Description         |
| ---------- | ------------------- |
| v1         | Label (spam or ham) |
| v2         | SMS message text    |
| Unnamed: 2 | Empty column        |
| Unnamed: 3 | Empty column        |
| Unnamed: 4 | Empty column        |

During preprocessing, only the relevant columns were used and renamed to:

* **label**
* **message**

---

## Technologies Used

* Python
* Pandas
* Scikit-learn
* Natural Language Processing (NLP)
* TF-IDF Vectorization

---

## Machine Learning Workflow

1. **Data Loading**

   * Load the dataset using pandas.

2. **Data Preprocessing**

   * Rename dataset columns
   * Remove unused columns
   * Prepare text data for modeling

3. **Feature Extraction**

   * Convert SMS messages into numerical vectors using **TF-IDF Vectorizer**.

4. **Train-Test Split**

   * Split dataset into **80% training data** and **20% testing data**.

5. **Model Training**

   * Train a **Multinomial Naive Bayes classifier**.

6. **Model Evaluation**

   * Evaluate model performance using:

     * Accuracy
     * Precision
     * Recall
     * F1 Score

7. **Prediction**

   * The model predicts whether a new SMS message is **Spam or Ham**.

---

## Example Prediction

Spam Message:
Congratulations! You've won a free gift card. Call now.

Prediction: **Spam**

Normal Message:
Hey, are we meeting at 6 PM today?

Prediction: **Not Spam**

---

## Project Structure

```
Spam-SMS-Detection-ML
│
├── Spam_Detection.ipynb
├── spam.csv
├── spam_detection_demo.mp4
└── README.md
```

---
## Author

**Navya Saravanan**

AIML Student

LinkedIn:
https://www.linkedin.com/in/navya-saravanan-8aa481311/
