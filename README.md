# Cognifyz Machine Learning Internship

Projects completed during the Cognifyz Technologies Machine Learning internship,
using a restaurant dataset of 9,551 restaurants across 15 countries.

## Tasks completed

### Task 1: Predict Restaurant Ratings (Regression)
- Cleaned the data, encoded categorical features, and removed leakage columns (Rating color / Rating text).
- Trained Linear Regression, Decision Tree and Random Forest.
- Compared results with and without unrated restaurants (rating 0), since unrated places inflate the score.
- Best model on rated restaurants: Random Forest, R² = 0.59, RMSE = 0.36.
- Most influential features: votes, city (outside the top 10 cities), number of cuisines, price range.

### Task 3: Cuisine Classification
- Predicted the primary cuisine for 18 cuisines with at least 100 restaurants.
- Used restaurant-name TF-IDF plus price, votes, booking and delivery features.
- Best model: Logistic Regression, accuracy 66.2% vs a baseline of 35.8%, macro F1 0.595.
- Analysed per-cuisine performance, class imbalance, and common misclassifications.

### Task 2: Restaurant Recommendation (Content-based)
- Encoded cuisines with TF-IDF and scored restaurants by cuisine similarity, price match and rating.
- Supports filtering by city, minimum rating and minimum votes.
- Evaluated with 5 sample users: 100% cuisine match, price match 40% to 100%.

## Tech stack
Python, pandas, NumPy, scikit-learn, matplotlib, seaborn

## How to run
1. `pip install -r requirements.txt`
2. Keep `Dataset.csv` in the same folder as the notebooks
3. Open any notebook in Jupyter, VS Code or Colab and run all cells

## Author
[sahil] | https://www.linkedin.com/in/sahil-rangi/ ]
