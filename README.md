# Flipkart-Sentiment-Analysis

🛒 Sentiment Analysis for E-Commerce Product Reviews

A complete End-to-End NLP System that scrapes Flipkart product reviews, 
analyzes customer sentiment using VADER, 
and visualizes trends via an interactive Flask web interface.

🎯 Objective

This project aims to bridge the gap between raw customer feedback and actionable insights. By automating the extraction and analysis of reviews, we help:
Customers make faster, informed purchasing decisions.
Businesses understand product strengths and areas for improvement.

🧩 Key Features

✅ Automated Web Scraping: Uses Playwright to fetch real-time reviews (User, Rating, Comment, Timestamp) from Flipkart.
✅ NLP Sentiment Analysis: Cleans text and calculates sentiment polarity (Positive, Negative, Neutral) using NLTK VADER.
✅ Star Rating Prediction: Predicts 1–5 star ratings based on sentiment compound scores using a custom rule-based algorithm.
✅ Interactive Dashboard: Visualizes data using Plotly & Matplotlib:
Sentiment Distribution (Pie Charts)
Actual vs. Predicted Ratings (Bar Graphs)
Confusion Matrix for Accuracy
Word Clouds for frequent positive/negative terms.
✅ Flask Web Interface: A user-friendly web app to input product links, trigger scraping, and view reports.

🛠️ Tech Stack

Component,Technology Used
Language,Python 3.x
Web Scraping,"Playwright, BeautifulSoup"
Data Processing,"Pandas, NumPy"
NLP & Sentiment,NLTK (VADER)
Visualization,"Plotly, Matplotlib, WordCloud"
Web Framework,Flask (HTML/CSS/Bootstrap)

📥 How It Works

Web Scraping: The app extracts multiple pages of reviews from a given Flipkart product URL using Playwright.
Sentiment Processing: Text is preprocessed (tokenization, cleaning) and passed through VADER to generate a Compound Score.
Rating Prediction: We map sentiment scores to stars:
Score < -0.3 ➔ ⭐ (1 Star)
Score > 0.6 ➔ ⭐⭐⭐⭐⭐ (5 Stars)
Visualization: The processed data is rendered into interactive charts and word clouds.
User Interface: Results are displayed on the Flask dashboard with options to download the analysis.

🚀 Installation & Usage

Clone the Repository:

git clone https://github.com/mehulchavan11/Sentiment-Analysis-Flipkart.git
cd Sentiment-Analysis-Flipkart
Install Dependencies:
pip install -r requirements.txt
Install Playwright Browsers:
playwright install
Run the Flask App:
python app.py
Access the Dashboard: Open your browser and go to http://127.0.0.1:5000/.

🌟 Applications

👤 For Customers,🏢 For Companies
Quick overview of pros & cons,Track user satisfaction trends
Reduces decision-making time,Identify product defects early
Unbiased sentiment summary,Competitor analysis

👥 Team Members

This project was developed collaboratively by:
Ajinkya Bondge
Atharva Patil
Mehul Chavan
Pratik Chinchawadkar

📜 License

This project is for educational purposes. Data is scraped from public sources.
