# 🌟 Sentimental Analysis   

A **Flask-powered web application** that performs **sentiment analysis** on user-input text.  
The app uses **Machine Learning (scikit-learn)** and **Natural Language Processing (NLTK)** to classify text as **Positive, Negative, or Neutral**.  

---

## 🚀 Demo Output  

<p align="center">
  <img src="./static/interface_sample.png" alt="Sentiment Analysis Web App UI" width="600">
</p>  

*User enters a comment → app preprocesses the text → model predicts sentiment → result is shown instantly on the interface.*

---

## 📂 Project Structure  

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

## 🎯 Features  

✅ Simple web-based interface to analyze text sentiment  
✅ Preprocessing with **NLTK** (stopword removal, stemming, cleaning)  
✅ Machine Learning model trained on TF-IDF features  
✅ Real-time predictions with Flask backend  
✅ Easily extensible for new datasets or UI improvements  

---

## 🛠️ Tech Stack  

- **Python 3.8+**  
- **Flask** (backend web framework)  
- **NLTK** (text preprocessing & stopwords)  
- **scikit-learn** (model training & inference)  
- **HTML + CSS (Jinja2)** (frontend template rendering)  

---

## 📥 Clone the Repository  

To get a copy of this project locally:  

```bash
git clone https://github.com/josphine1407/Sentimental_Analysis.git
cd Sentimental_Analysis

## Installation & Setup
pip install -r requirements.txt
**Run the App**
python App.py
➡ Open your browser and go to: http://127.0.0.1:5000/
