#EA-Sports-player-analysics-project
## Predicting Football Player Market Value Using Machine Learning

## Project Overview

This project explores the relationship between football player characteristics and their market value using the EA SPORTS FC 24 Complete Player Dataset.

The primary objective is to develop regression models capable of predicting a player's market value based on demographic, physical, and technical attributes. The project follows a complete data science workflow including data cleaning, exploratory data analysis (EDA), feature selection, machine learning, model evaluation, and hyperparameter tuning.

## Business Problem

Football clubs invest millions of euros in player transfers every year. Accurately estimating a player's market value is essential for recruitment, contract negotiations, scouting, and financial planning.

This project investigates whether machine learning models can accurately estimate player market value using player characteristics available in the EA SPORTS FC 24 dataset.

## Dataset

**Dataset Name**

EA SPORTS FC 24 Complete Player Dataset

**Source**

https://www.kaggle.com/datasets/stefanoleone992/ea-sports-fc-24-complete-player-dataset

The original dataset contains historical player records from FIFA 15 through EA SPORTS FC 24.

For this project, only **EA SPORTS FC 24 players** (`fifa_version = 24`) were analyzed.

Final dataset:

- 18,350 players
- 109 original features
- Selected numerical features used for modeling

Target Variable

- value_eur

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- GitHub
- OpenAI ChatGPT (project planning and documentation assistance)

## Exploratory Data Analysis

The exploratory analysis included:

- Distribution of player market values
- Age distribution
- Overall rating distribution
- Scatter plots
- Correlation heatmap
- Outlier analysis

These analyses identified the strongest relationships between player characteristics and market value.

## Machine Learning Models

The following regression models were developed and compared:

- Single Variable Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Ridge Regression

Model performance was evaluated using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Coefficient of Determination (R²)

GridSearchCV was used to determine the optimal regularization parameter for Ridge Regression.

## Results

Among the evaluated models, **Multiple Linear Regression** achieved the best overall predictive performance.

Key findings include:

- Overall Rating is strongly associated with market value.
- Potential is an important predictor of player valuation.
- Combining multiple player characteristics significantly improves prediction accuracy.
- Ridge Regression produced results very similar to Multiple Linear Regression, indicating limited overfitting.
- Polynomial Regression did not significantly improve performance compared with the multiple linear model.

## Repository Structure

EA-FC24-Player-Value-Prediction/

│── analysis.ipynb
│── data.csv
│── chat.txt
│── README.md
 
## 📚 References

- Stefano Leone. EA SPORTS FC 24 Complete Player Dataset.
- https://www.kaggle.com/datasets/stefanoleone992/ea-sports-fc-24-complete-player-dataset

- OpenAI. ChatGPT (GPT-5.5).
- https://chat.openai.com/

- Scikit-learn Documentation
- https://scikit-learn.org/stable/

- Pandas Documentation
- https://pandas.pydata.org/

- Matplotlib Documentation
- https://matplotlib.org/

- Seaborn Documentation
- https://seaborn.pydata.org/
