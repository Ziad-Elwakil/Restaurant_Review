
# 🧠 Sentiment Analysis Web App

## 🔍 Project Overview

This project is a **Sentiment Analysis** tool built using **Natural Language Processing (NLP)** techniques. It analyzes **restaurant reviews** and classifies them as **Positive** or **Negative** using a **Multinomial Naive Bayes classifier**.

The model is trained on the `Restaurant_Reviews.tsv` dataset and includes an interactive **Gradio-based web interface** for user-friendly review classification.

---

## 📊 Features

- Visualizations:
  - Label distribution (bar and pie charts)
  - Review length distribution
  - Word clouds for all, positive, and negative reviews
  - Sentiment polarity histogram
- NLP Preprocessing:
  - Emoji removal
  - Lowercasing, punctuation removal, stopwords removal
  - Lemmatization and stemming
  - Spell correction using TextBlob
- Model:
  - Bag of Words (CountVectorizer)
  - Multinomial Naive Bayes
  - Hyperparameter tuning for alpha
- Evaluation:
  - Accuracy, precision, recall
  - Confusion matrix with heatmap
- Deployment:
  - Interactive Gradio app to test new reviews

---

## 🛠️ Installation

```bash
pip install numpy pandas matplotlib seaborn wordcloud nltk textblob scikit-learn gradio emoji
```

---

## 📁 Dataset

- **Filename**: `Restaurant_Reviews.tsv`
- **Columns**:
  - `Review`: Text of the review
  - `Liked`: Label (0 for Negative, 1 for Positive)

---

## 🚀 Usage

1. Clone the repo or run the notebook in Google Colab.
2. Mount Google Drive and place `Restaurant_Reviews.tsv` in the correct path.
3. Run all cells to:
   - Visualize the data
   - Clean and process reviews
   - Train and evaluate the model
4. Launch the Gradio app:
   ```python
   interface.launch()
   ```
5. Enter any customer review in the textbox to classify it.

---

## 🧪 Example Inputs

```text
"The food was absolutely wonderful, from preparation to presentation."
🔁 Output: 🟢 POSITIVE Review

"The meat was undercooked and the service was slow."
🔁 Output: 🔴 NEGATIVE Review
```

---

## 📈 Model Performance

After hyperparameter tuning, the best accuracy achieved was around **86-89%** with `alpha=0.5`.

Metrics:
- ✅ Accuracy: ~87%
- 🎯 Precision: ~0.88
- 🔁 Recall: ~0.85

---

## 🧰 Tools & Libraries

- Python 🐍
- NLTK
- TextBlob
- Scikit-learn
- Matplotlib & Seaborn
- WordCloud
- Gradio
- Emoji

---

## 🧠 Author

- 👨‍💻 **Ziad Elwakeel**
- 📧 zm655092@gmail.com
- 🏫 Menoufia University – Artificial Intelligence

---

## 📌 Notes

- Optional steps like **spell correction** and **stemming** can be enabled or disabled as needed.
- Works best with short to medium-length reviews.
- You can expand this by using TF-IDF, deep learning models, or multi-language support.
