# 🍽 Food Recipe Rating Prediction using Machine Learning

A machine learning project that predicts recipe ratings based on ingredients, preparation time, cuisine type, and other features. Two models are compared — Linear Regression and Random Forest Regressor.

## 📊 Results

| Model | R² Score | RMSE | MAE |
|-------|----------|------|-----|
| Linear Regression | baseline | higher | higher |
| **Random Forest** | **~18–23% better** | lower | lower |

✅ **Random Forest Regressor** achieved the best performance.

## 🛠 Tech Stack
- Python, Jupyter Notebook
- scikit-learn (LinearRegression, RandomForestRegressor)
- Pandas, NumPy
- Matplotlib, Seaborn

## 📋 Features Used
- Cuisine type, Meal type, Difficulty level
- Number of ingredients, Prep time, Cook time
- Calories, Number of reviews
- Vegetarian / Gluten-free flags
- Engineered: Total time, Ingredient density, Calorie level

## ⚙️ Setup & Run

```bash
# Clone the repo
git clone https://github.com/sanaishrath7860-dotcom/food-recipe-rating-prediction.git
cd food-recipe-rating-prediction

# Install dependencies
pip install numpy pandas scikit-learn matplotlib seaborn jupyter

# Open the notebook
jupyter notebook food_recipe_rating_prediction.ipynb
```

## 📁 Files
```
food-recipe-rating-prediction/
├── food_recipe_rating_prediction.ipynb   # Main notebook
├── eda_plots.png                         # Generated EDA plots
├── model_evaluation.png                  # Model comparison charts
└── README.md
```

## 🔍 Key Findings
- `num_reviews` is the strongest predictor of recipe rating
- Random Forest captures non-linear relationships that Linear Regression misses
- Easy recipes tend to receive higher ratings than complex ones
- Feature engineering (total time, ingredient density) improved model accuracy
