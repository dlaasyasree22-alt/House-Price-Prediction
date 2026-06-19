# House-Price-Prediction
Week 1 Internship Project — House Price Prediction using Linear Regression and Random Forest
# House Price Prediction

This is my Week 1 project from my data science internship. The goal was to 
figure out what actually drives house prices — is it the size of the house? 
The number of bathrooms? Whether it has air conditioning? I used a real-world 
housing dataset to find out.

# What I Did

I started by loading and exploring the dataset, then cleaned it up by handling 
missing values, removing duplicates, and converting yes/no text columns into 
numbers the model could actually use. After that, I trained two different 
models — Linear Regression and Random Forest — and compared how well each 
one predicted house prices. Finally, I created charts to visualize the findings 
and wrote up what I learned.

# How the Models Performed

Interestingly, the simpler model won here:

| Model | MAE | R² Score |
|-------|-----|----------|
| Linear Regression | ₹9,91,074 | 0.63 |
| Random Forest | ₹10,64,471 | 0.59 |

Linear Regression explained 63% of the variation in house prices with an 
average prediction error of around ₹9.9 lakhs — and actually outperformed 
the more complex Random Forest model, which tells me the relationships in 
this dataset are fairly straightforward and linear.

## What I Found

- **Area is everything** — it alone accounted for 50.8% of feature importance 
  and had the strongest correlation with price (0.54)
- **Bathrooms matter more than bedrooms** — bathrooms ranked 2nd in importance 
  while bedrooms ranked 6th, which surprised me
- **Air conditioning adds real value** — it ranked 4th in feature importance, 
  above stories and parking
- **Price distribution is right-skewed** — most houses are in a lower price 
  range with a few expensive outliers pulling the average up


## 🛠️ Tools & Libraries

Python, Jupyter Notebook, Pandas, Scikit-learn, Matplotlib, Seaborn

## 📌 Dataset Source

[Housing Prices Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset)
