
# Sephora Skincare Recommender

<div align="center">

<img src="https://img.shields.io/badge/Python-3.9+-blue?style=for-the-badge&logo=python"/>
<img src="https://img.shields.io/badge/Flask-API-black?style=for-the-badge&logo=flask"/>
<img src="https://img.shields.io/badge/Streamlit-WebApp-red?style=for-the-badge&logo=streamlit"/>
<img src="https://img.shields.io/badge/Machine%20Learning-Recommender-green?style=for-the-badge"/>
<img src="https://img.shields.io/badge/NLP-Content%20Based-orange?style=for-the-badge"/>

</div>

---

<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?size=22&duration=3000&color=36BCF7&center=true&vCenter=true&lines=Hybrid+Skincare+Recommendation+System;Built+with+Machine+Learning+and+NLP;Fast+%7C+Scalable+%7C+Personalized"/>

</div>

---

## Overview

A **Hybrid Recommendation System** for **Sephora skincare products**, combining:

- **Item-Based Collaborative Filtering** – based on user ratings  
- **Content-Based Filtering** – based on ingredients, categories, and product metadata  

This system delivers **accurate and personalized skincare recommendations** using machine learning and NLP techniques.

---

## Purpose

- Help users discover skincare products tailored to their **preferences and needs**
- Provide **intelligent recommendations** using hybrid ML models
- Enhance product discovery using **data-driven insights**

---

## Features

- Hybrid Recommendation Model (Collaborative + Content-Based)
- Flask API for real-time recommendations
- Streamlit Web App for interactive UI
- Precomputed similarity matrix for performance optimization
- Scalable architecture for large datasets

---

## Architecture

```mermaid
flowchart LR
	A[User Input] --> B[Streamlit UI]
	B --> C[Flask API]
	C --> D[Hybrid Recommendation Engine]
	D --> E[Similarity Matrix]
	E --> F[Recommended Products]
	F --> B
Project Structure
.
├── data/
│   ├── product_info.csv
│   ├── reviews_0-250.csv
│   ├── reviews_250-500.csv
│   ├── reviews_500-750.csv
│   ├── reviews_750-1250.csv
│   ├── reviews_1250-end.csv
│
├── metadata/
│   ├── products.csv
│   ├── hybrid_similarity.pkl
│
├── skincare/              # Virtual environment (ignored)
├── api.py                 # Flask API
├── app.py                 # Streamlit App
├── model.ipynb            # Model development
├── requirements.txt
├── .gitignore
└── README.md
Dataset
Source

https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews/data

Setup Instructions

Download and extract the dataset

Place files inside the data/ directory:

data/
├── product_info.csv
├── reviews_0-250.csv
├── reviews_250-500.csv
├── reviews_500-750.csv
├── reviews_750-1250.csv
├── reviews_1250-end.csv
Installation

Install dependencies:

pip install -r requirements.txt
Running the Application
Run Flask API
python api.py

Access endpoint:

http://127.0.0.1:5000/recommend?product_id=P12345&num_recommendations=5
Run Streamlit Web App
streamlit run app.py

Open in browser:

http://localhost:8501
How It Works

User selects a skincare product

System analyzes:

User ratings (Collaborative Filtering)

Product metadata (Content-Based Filtering)

Hybrid model computes similarity scores

Top recommendations are returned

Results displayed with product details

Tech Stack
Layer	Technology
Backend API	Flask
Frontend	Streamlit
ML Models	Scikit-learn
Data Processing	Pandas, NumPy
NLP	TF-IDF / Vectorization
Future Improvements

Sentiment analysis on user reviews

Skin-type and concern-based personalization

Deep learning embeddings for better similarity

Cloud deployment (AWS / GCP / Azure)

Real-time recommendation updates

Contribution

Contributions are welcome.

Fork the repository

Create a new branch

Make your changes

Submit a pull request

License

This project is intended for educational and research purposes.










 








