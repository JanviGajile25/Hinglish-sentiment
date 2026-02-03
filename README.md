## 📊 Hinglish Sentiment Analysis

This project demonstrates a **Hinglish (Hindi + English) sentiment analysis system** using **Machine Learning (Logistic Regression)**.
It classifies Hinglish classroom feedback into **Positive**, **Negative**, or **Neutral** sentiments.

---

## 🚀 Project Overview

Hinglish is widely used in India, but most sentiment analysis tools are built for pure English.
This project shows how to:

* preprocess Hinglish text
* convert text into numerical features using **TF-IDF**
* train a **Logistic Regression** classifier
* predict sentiment for new Hinglish sentences
* save and reuse trained models

---

## 🧠 Sentiment Classes

* **Positive** – good feedback (e.g., *“Sir aaj ki class bahut achhi thi”*)
* **Negative** – poor feedback (e.g., *“Lecture boring tha”*)
* **Neutral** – average feedback (e.g., *“Class theek thi”*)

---

## 🗂️ Project Structure

```
Hinglish-sentiment-demo-main/
│
├── experiment.ipynb          # Main notebook (training + testing)
├── feedback.csv              # Generated dataset
├── tfidf_vectorizer.pkl      # Saved TF-IDF vectorizer
├── sentiment_model.pkl       # Trained Logistic Regression model
├── README.md                 # Project documentation
```

---

## ⚙️ Technologies Used

* **Python 3.10**
* **Pandas** – data handling
* **Regex** – text cleaning
* **Scikit-learn**

  * TF-IDF Vectorizer
  * Logistic Regression
  * Train-test split
* **Joblib** – model saving

---

## 🧪 Dataset Creation

The dataset is **manually created** using:

* Hinglish positive sentences
* Hinglish negative sentences
* Hinglish neutral sentences

These are combined into a CSV file (`feedback.csv`) with labels.

---

## 🧹 Text Preprocessing

Steps applied to text:

1. Convert to lowercase
2. Remove numbers and special characters
3. Keep:

   * English characters (`a-z`)
   * Hindi Unicode range (`\u0900-\u097F`)
4. Remove extra spaces

This ensures Hinglish text is preserved correctly.

---

## 📐 Feature Extraction

* **TF-IDF Vectorizer** is used
* Converts cleaned text into numerical vectors
* Helps capture important words while reducing noise

---

## 🤖 Model Training

* **Algorithm:** Logistic Regression
* **Train/Test Split:** 80% / 20%
* **Stratified split** to balance sentiment classes
* Model is trained with `max_iter = 1000`

---

## 📈 Model Evaluation

* Accuracy is calculated on test data
* Model performs well for small demo datasets
* Suitable for educational and demo purposes

---

## 🔮 Sentiment Prediction

You can predict sentiment for new Hinglish sentences:

```python
predict_sentiment("Sir aaj ki class bahut achhi thi")
```

Example outputs:

* Positive
* Negative
* Neutral

---

## 💾 Model Saving

The trained components are saved for reuse:

* `sentiment_model.pkl`
* `tfidf_vectorizer.pkl`

These can be loaded later without retraining.

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone <repo-url>
cd Hinglish-sentiment-demo-main
```

### 2️⃣ Install dependencies

```bash
pip install pandas scikit-learn joblib regex
```

### 3️⃣ Run the notebook

Open `experiment.ipynb` in Jupyter Notebook or VS Code and run all cells.

---

## 🎓 Use Cases

* Classroom feedback analysis
* Student sentiment analysis
* NLP learning project
* Mini / Final year ML project
* Hinglish text processing demo

---

## 📌 Future Improvements

* Larger real-world Hinglish dataset
* Deep learning models (LSTM / BERT)
* Streamlit web interface
* Hindi transliteration support

---

## ✨ Conclusion

This project shows how **Machine Learning + NLP** can be applied to **Indian Hinglish data**, making sentiment analysis more practical and relatable.


