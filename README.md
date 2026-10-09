# House Price Prediction Using Machine Learning

## Project Overview
This project develops and evaluates regression models to predict house prices. The notebook explores the dataset, preprocesses the data, encodes categorical features, trains regression models, and evaluates their performance.

## Objectives
- Explore and understand the house-price dataset.
- Clean and preprocess data for machine learning.
- Encode ordinal and categorical features.
- Train regression models to predict house prices.
- Evaluate predictions using regression metrics.
- Save the trained model and preprocessing objects for reuse.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Pickle

## Models Used
- **Linear Regression**
- **Decision Tree Regressor**

## Workflow
1. Load the house-price dataset.
2. Perform exploratory data analysis (EDA), including checking missing values, data types, summary statistics, and correlations.
3. Remove the `ID` and `Locality` columns as described in the notebook.
4. Encode ordinal features such as property type, furnishing status, public transport accessibility, facing, and security.
5. Normalize the case of categorical text values.
6. Randomly sample 40% of the dataset to reduce training time.
7. Split the sampled data into training and testing sets.
8. Convert categorical features using `DictVectorizer`.
9. Train and evaluate Linear Regression and Decision Tree regression models.
10. Save the trained model and preprocessing objects.

## Evaluation Metrics
The notebook uses the following metrics:
- **MAE (Mean Absolute Error):** Average absolute difference between actual and predicted prices.
- **MSE (Mean Squared Error):** Average squared prediction error.
- **RMSE (Root Mean Squared Error):** Square root of MSE, expressed in the target's units.
- **R² Score:** Indicates how well the model explains variation in house prices.

## Requirements
Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Dataset
The notebook loads a CSV file named `E06_house price data less.csv`. Place this dataset in the same folder as the notebook before running it. The dataset is not included in this README.

## How to Run
1. Clone or download this repository.
2. Place `E06_house price data less.csv` in the same directory as the notebook.
3. Install the required libraries.
4. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open the `.ipynb` notebook and run the cells in order.

## Saved Files
After running the model-saving cell, the notebook saves:
- `house_price_model.pkl` — trained Decision Tree model
- `vectorizer.pkl` — fitted `DictVectorizer`
- `encoder.pkl` — fitted `OrdinalEncoder`
- `features.pkl` — input feature names

## Conclusion
The project demonstrates house-price prediction using Linear Regression and Decision Tree regression. The models are evaluated with standard regression metrics. Actual performance depends on the dataset and the evaluation results generated when the notebook is run.

## Author
Add your name here.
