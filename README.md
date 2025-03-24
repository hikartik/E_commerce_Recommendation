(canvas
# E-commerce Product Recommendation System

## Overview
This project implements a product recommendation system for an e-commerce platform. It uses both content-based and collaborative filtering techniques to deliver personalized product recommendations. The backend is developed using Flask with SQLAlchemy for database interactions, while data processing and machine learning are handled with Pandas, Scikit-learn, and SpaCy.

## Features
- **User Authentication:**  
  Signup and signin functionality with secure storage of user credentials in a MySQL database.
- **Trending Products Display:**  
  Shows trending products with randomly assigned images and pricing.
- **Content-Based Recommendation:**  
  Utilizes TF-IDF vectorization on product tags and cosine similarity to recommend similar items.
- **Collaborative Filtering:**  
  Constructs a user-item rating matrix to find similar users and recommend products based on their interactions.
- **Hybrid Recommendations:**  
  Combines content-based and collaborative approaches for more robust recommendations.

## Technologies & Tools
- **Programming Language:** Python
- **Web Framework:** Flask
- **Database:** MySQL (using SQLAlchemy)
- **Data Processing:** Pandas, NumPy
- **Machine Learning & NLP:** Scikit-learn (TF-IDF, cosine similarity), SpaCy
- **Visualization:** Matplotlib, Seaborn

## Installation & Setup
1. **Clone the Repository:**  
   Clone the project repository to your local machine.
2. **Create a Virtual Environment:**  
   Set up and activate a Python virtual environment.
3. **Install Dependencies:**  
   Run the following command to install required packages:
```bash
pip install -r requirements.txt
```
4. **Database Configuration:**  
Configure the MySQL database as per the settings in `app.py`.
5. **Run the Flask Application:**  
Start the application by executing:
```bash
python app.py
```


6. **Access the Application:**  
Open your web browser and navigate to `http://localhost:5000`.

## Usage

### Running the Application
- **Homepage:** View trending products.
- **User Authentication:** Sign up or sign in using the provided forms.
- **Recommendations:** Access product recommendations via designated routes.

### Project Notebook (Jupyter Notebook)
The `project_notebook.ipynb` contains the following steps:
1. **Data Loading:**  
Load product review data from `product_review.tsv` and CSV files (`trending_products.csv` and `clean_data.csv`).
2. **Data Cleaning & Preprocessing:**  
- Handle missing values and standardize column names.
- Use SpaCy to clean text data and extract relevant product tags.
3. **Exploratory Data Analysis (EDA):**  
- Generate statistics and visualizations to analyze user interactions and product popularity.
4. **Recommendation System Implementation:**  
- **Content-Based Filtering:**  
  Apply TF-IDF on product tags and calculate cosine similarity to find similar items.
- **Collaborative Filtering:**  
  Build a user-item matrix and compute user similarities to recommend new products.
- **Hybrid Recommendations:**  
  Merge content-based and collaborative recommendations to provide a diverse set of suggestions.

