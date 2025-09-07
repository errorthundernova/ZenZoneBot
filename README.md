
# ZenZone Bot

**ZenZone Bot** is an AI-powered mental health chatbot designed to promote emotional well-being. It leverages Natural Language Processing (NLP) and Machine Learning (ML) techniques to provide personalized mindfulness exercises, stress-relief tips, and mental health resources, helping users manage stress effectively.

---

## Features

- **Keyword Recognition**: Identifies important keywords in user input using NLTK to respond more accurately to user concerns.
- **Sentiment Analysis**: Analyzes the emotional tone of user messages with TF-IDF vectorization and Random Forest classifiers, detecting emotions like joy, fear, anger, sadness, distress, and shame.
- **Text Summarization**: Uses LSA (Latent Semantic Analysis) summarizer to condense longer user inputs into concise summaries for better understanding.
- **Intent Recognition**: Employs Support Vector Classifier (SVC) to accurately detect user intent, ensuring relevant and helpful responses.
- **Mental Health Support**: Offers personalized suggestions, coping strategies, and resource guidance based on sentiment, keywords, and intent.

---

## Installation

1. **Clone the repository**
```bash
git clone <your-repo-link>
cd ZenZoneBot
````

2. **Create a virtual environment**

```bash
python -m venv venv
```

3. **Activate the virtual environment**

* **Windows**

```bash
venv\Scripts\activate
```

* **Linux / Mac**

```bash
source venv/bin/activate
```

4. **Install dependencies**

```bash
pip install -r requirements.txt
```

5. **Download NLTK data**

```python
python
>>> import nltk
>>> nltk.download('punkt')
>>> nltk.download('stopwords')
>>> exit()
```

---

## Usage

1. Run the Flask application:

```bash
python app.py
```

2. Open your browser and navigate to:

```
http://127.0.0.1:5000/
```

3. Start chatting with ZenZone Bot through the web interface.

---

## Project Structure

```
ZenZoneBot/
│
├─ app.py                  # Main Flask application
├─ text_sum1.py            # Text summarization and evaluation using LSA & ROUGE
├─ sent.py                 # Sentiment analysis using TF-IDF and Random Forest
├─ keyword1.py             # Keyword matching module
├─ int.py                  # Intent recognition module
├─ templates/              # HTML templates for web interface
├─ static/                 # Static files (CSS, JS, images)
├─ Sent_Analy_classifier_model.joblib   # Pre-trained sentiment model
├─ tfidf_vectorizer_1.joblib            # Pre-trained TF-IDF vectorizer
└─ requirements.txt        # Python dependencies
```

---

## Dependencies

* Flask
* NLTK
* scikit-learn
* pandas
* joblib
* sumy
* rouge

Install all dependencies with:

```bash
pip install -r requirements.txt
```

---

## Future Enhancements

* Integration with IoT wearable devices for emotion tracking.
* Gamification and rewards to improve engagement.
* Advanced emotion recognition beyond basic sentiment analysis.
* Role-playing and peer connection features for better support.

---
## Author

**Samragee Chopra**




