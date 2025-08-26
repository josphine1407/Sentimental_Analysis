# Sentimental Analysis   

A **Flask-powered web application** that performs **sentiment analysis** on user-input text.  
The app uses **Machine Learning (scikit-learn)** and **Natural Language Processing (NLTK)** to classify text as **Positive, Negative, or Neutral**.  

## Project Structure  
```
Sentimental_Analysis/
│
├── app.py # Flask application (main entry point)
├── clf.pkl # Trained ML classifier (pickle file)
├── tfidf.pkl # TF-IDF vectorizer (pickle file)
├── requirements.txt # Python dependencies
├── templates/
│ └── index.html # Frontend template (user interface)
├── static/ # (Optional) CSS / images for styling
└── Sentiment Analysis.ipynb # Jupyter Notebook (model training)

---

## Features  

✅ Simple web-based interface to analyze text sentiment  
✅ Preprocessing with **NLTK** (stopword removal, stemming, cleaning)  
✅ Machine Learning model trained on TF-IDF features  
✅ Real-time predictions with Flask backend  
✅ Easily extensible for new datasets or UI improvements  

---

## Tech Stack  

- **Python 3.8+**  
- **Flask** (backend web framework)  
- **NLTK** (text preprocessing & stopwords)  
- **scikit-learn** (model training & inference)  
- **HTML + CSS (Jinja2)** (frontend template rendering)  

---

## Clone the Repository  

To get a copy of this project locally:  

```bash
git clone https://github.com/josphine1407/Sentimental_Analysis.git
cd Sentimental_Analysis

## Installation & Setup
pip install -r requirements.txt
**Run the App**
python App.py
➡ Open your browser and go to: http://127.0.0.1:5000/

---

## How It Works

Input: User submits a comment through the web form.

Preprocessing:

Lowercasing & cleaning

Stopword removal (using NLTK)

Word stemming (PorterStemmer)

Vectorization: Text is converted into numerical features using TF-IDF.

Prediction: Pre-trained classifier (clf.pkl) predicts sentiment label.

Output: Sentiment result is displayed back on the webpage.

📊 Model Training (Notebook)

The Jupyter notebook includes:

Dataset loading & exploration

Text preprocessing pipeline

TF-IDF feature engineering

Model training (Logistic Regression / Naive Bayes)

Performance evaluation (Accuracy, Precision, Recall, F1)

Saving model (clf.pkl) & vectorizer (tfidf.pkl)

🌱 Future Enhancements

📌 Add sentiment confidence score (e.g., probability output)

🌍 Extend to multilingual sentiment analysis

🎨 Improve UI with Bootstrap / TailwindCSS

☁️ Deploy on Heroku / Render / Railway for public access

🤖 Add deep learning model (LSTM / BERT) for better accuracy

📸 Example Output

Input:

"I really love this product, it's amazing!"

Output:

✅ Sentiment: Positive
