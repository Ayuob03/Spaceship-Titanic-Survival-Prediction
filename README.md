# Spaceship Titanic Survival Prediction

## Project Overview
This project aims to predict whether passengers were transported to another dimension on the Spaceship Titanic. The dataset includes passenger demographics, cabin information, spending habits, and travel details.

## Dataset
- Source: [Kaggle Spaceship Titanic](https://www.kaggle.com/competitions/spaceship-titanic/data)
- Features include:
  - PassengerId, HomePlanet, CryoSleep, Cabin, Destination, Age, VIP
  - Spending data: RoomService, FoodCourt, ShoppingMall, Spa, VRDeck
  - Target: Transported

## Data Cleaning & Feature Engineering
- Filled missing values using group information (passengers traveling together).  
- Split Cabin into Deck, Number, and Side.  
- Converted VIP and CryoSleep to boolean types.  
- Created group-based features like Group_Size.  
- Encoded categorical variables and scaled numeric features.

## Modeling
- Baseline models: Logistic Regression, Random Forest, Gradient Boosting (XGBoost/LightGBM).  
- Hyperparameter tuning using RandomizedSearchCV.  
- Evaluation metrics: Accuracy, F1-score, ROC-AUC.  
- Feature importance and interpretation using SHAP.

## Results
- Best model: [Your best model name]  
- Key predictive features: Deck, Side, Age, Spending features, Group_Size.

## How to Run
1. Clone this repository.  
2. Install dependencies: `pip install -r requirements.txt`  
3. Run `main.ipynb` to reproduce preprocessing, modeling, and evaluation.  
4. Predictions can be generated on `test.csv` and submitted to Kaggle.

## Author
- Ayuob Mubedein
