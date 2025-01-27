# eCommerce Customer Analytics

## Project Overview
This project analyzes an eCommerce dataset to generate actionable business insights, build a Lookalike Model for customer recommendations, and predict customer churn using machine learning techniques. The goal is to showcase advanced data science skills while delivering meaningful results for potential business applications.

---

## Repository Structure

```
ecommerce_customer_analytics/
├── data/                           # Dataset files
│   ├── Customers.csv
│   ├── Products.csv
│   ├── Transactions.csv
├── Jins_Varghese_EDA.ipynb
├── Jins_Varghese_EDA.pdf
├── Jins_Varghese_Lookalike.ipynb
├── Jins_Varghese_Lookalike.csv
├── Jins_Varghese_ChurnPrediction.ipynb
├── Jins_Varghese_ChurnPredictions.csv
├── Jins_Varghese_Clustering.ipynb
├── Jins_Varghese_Clustering.csv
├── README.md
└── requirements.txt
```

---

## Key Features

### 1. **Exploratory Data Analysis (EDA)**
- Performed in-depth analysis of customer transactions, products, and regional behaviors.
- Generated five business insights:
  1. Revenue contribution by category (e.g., Books leads with $192,147.47).
  2. Regional customer behaviors with South America having the highest AOV.
  3. Increasing yearly customer signups, with 79 new customers in 2024.
  4. Seasonal sales trends, with peaks in January and dips in November.
  5. Top 10 products by revenue, led by "ActiveWear Smartwatch."

### 2. **Lookalike Model**
- Developed an ensemble-based recommendation system using:
  - **Collaborative Filtering:** Customer-product interactions (cosine similarity).
  - **Content-Based Filtering:** Customer profile attributes (CountVectorizer).
  - Weighted combination of collaborative and content-based scores.
- Outputs the top 3 most similar customers for the first 20 customers.
- Results saved in `Jins_Varghese_Lookalike.csv`.

### 3. **Customer Churn Prediction**
- Defined churn as customers with no transactions in the last 30 days.
- Aggregated customer-level features (e.g., transaction frequency, average spending).
- Trained a **Random Forest Classifier**:
  - Achieved high accuracy and insights from feature importance.
- Predictions saved in `Jins_Varghese_ChurnPredictions.csv`.

---

## Usage Instructions

### 1. **Setup Environment**
- Install required Python libraries:
  ```bash
  pip install -r requirements.txt
  ```

### 2. **Run Notebooks**
- Open Jupyter Notebooks for each task:
  1. `Jins_Varghese_EDA.ipynb` for exploratory data analysis.
  2. `Jins_Varghese_Lookalike.ipynb` for customer recommendations.
  3. `Jins_Varghese_ChurnPrediction.ipynb` for churn analysis.
  4. `Jins_Varghese_Clustering.ipynb` for clustering.

### 3. **Explore Outputs**
- Key output files:
  - `Jins_Varghese_EDA.pdf`: Business insights report.
  - `Jins_Varghese_Lookalike.csv`: Top 3 similar customers.
  - `Jins_Varghese_ChurnPredictions.csv`: Predicted churn labels.
  - `Jins_Varghese_Clustering.csv`: Done clustering.

---

## Results and Business Impact
- **Lookalike Model:** Helps identify similar customers for targeted marketing.
- **Churn Prediction:** Enables proactive customer retention strategies.
- **Insights:** Guides business decisions like inventory management and regional campaigns.

---

## Future Enhancements
- Implement deep learning-based embeddings for more accurate recommendations.
- Deploy the models as interactive dashboards using Streamlit or Flask.
- Automate feature engineering for real-time churn predictions.

---
