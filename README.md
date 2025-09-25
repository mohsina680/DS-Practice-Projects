# DS-Practice-Projects
🧠 AI-Powered Projects Repository

This repository contains two Python-based machine learning projects:

🎬 Netflix Movie Recommendation System – Recommends similar movies and shows based on description similarity.

🔒 ML-Based Phishing URL Detector – Detects malicious or phishing websites using machine learning and feature engineering.

🎬 1. Netflix Movie Recommendation System
📌 Overview

This project uses Natural Language Processing (NLP) and similarity metrics to recommend movies or TV shows from the Netflix dataset (netflix_titles.csv).
When a user enters a title, the system returns a list of top 5 most similar titles based on description similarity.

⚙️ How It Works

The dataset is preprocessed using TF-IDF (Term Frequency–Inverse Document Frequency).

It computes similarity between titles using cosine similarity.

Returns the most similar shows or movies to the user’s input.

🧪 Example Usage
recommend("Breaking Bad")


Output:

1. Narcos
2. Ozark
3. El Chapo
4. Queen of the South
5. Better Call Saul

🔒 2. ML-Based Phishing URL Detector
📌 Overview

This project aims to detect phishing URLs using machine learning. It analyzes multiple features of a given website link and classifies it as legitimate or malicious.

⚙️ Features Extracted

Some of the key features used for classification include:

URL length, presence of @ symbol, and IP usage

SSL certificate status

Number of subdomains and domain age

Redirection patterns, favicon checks, and more

🤖 Workflow

Feature Engineering – Extract key indicators from the URL.

Model Training – Use ML algorithms (e.g., Random Forest, Logistic Regression) on a labeled dataset.

Prediction – Classify new URLs as Phishing or Legitimate.

🧪 Example Usage
url = "http://example-phishing-site.com/login"
result = predict_url(url)
print(result)


Output:

⚠️ Phishing Detected: This URL is potentially malicious.

🧰 Tech Stack

🐍 Python 3.x

📊 Pandas, NumPy – Data handling

📈 Scikit-learn – ML model training

📚 TF-IDF & Cosine Similarity – NLP-based recommendation

🌐 Requests, whois, socket, ssl – URL feature extraction

📂 Project Structure
📁 project/
│
├── 📁 netflix_recommender/
│   ├── recommender.py
│   └── netflix_titles.csv
│
├── 📁 phishing_detector/
│   ├── feature_extractor.py
│   ├── model_training.ipynb
│   └── phishing_dataset.csv
│
└── README.md

🚀 Future Improvements

✅ Deploy both projects as web applications using Flask or Streamlit

✅ Add real-time URL scanning with live website data

✅ Enhance recommendation accuracy using transformer-based NLP models
