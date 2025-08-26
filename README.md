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

## 🔍 How It Works  

The application workflow is divided into the following steps:  

### 📝 1. Input  
- User submits a comment or text through the web form.  

### 🧹 2. Preprocessing  
- Convert text to lowercase and remove unwanted characters  
- Remove stopwords (using **NLTK**)  
- Apply stemming (**PorterStemmer**)  

### 🔡 3. Vectorization  
- Convert cleaned text into numerical features using **TF-IDF vectorizer** (`tfidf.pkl`)  

### 🤖 4. Prediction  
- Pre-trained classifier (`clf.pkl`) predicts the sentiment label (Positive / Negative / Neutral)  

### 📤 5. Output  
- Predicted sentiment is displayed back on the webpage in real time  


## 📊 Model Training (Notebook)  

The Jupyter Notebook covers the following stages:  

### 📂 1. Data Preparation  
- Load dataset  
- Explore text samples and labels  

### 🧹 2. Preprocessing  
- Tokenization & stopword removal  
- Stemming / normalization  

### 🔡 3. Feature Engineering  
- Convert text into vectors using **TF-IDF**  

### 🏋️ 4. Model Training  
- Train models such as **Logistic Regression** or **Naive Bayes**  

### 📈 5. Evaluation  
- Measure **Accuracy, Precision, Recall, and F1-score**  

### 💾 6. Saving Artifacts  
- Save trained model → `clf.pkl`  
- Save TF-IDF vectorizer → `tfidf.pkl`  

## 📸 Example Output  

### Input:  
"I really love this product, it's amazing!"

### Output:  
✅ Sentiment: Positive
