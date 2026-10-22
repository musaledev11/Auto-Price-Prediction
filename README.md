# Automobile Price Prediction

A machine learning project that estimates the selling price of a vehicle based on details such as its brand, model, year, mileage, fuel type, transmission, and other available features.

## Project Overview

The purpose of this project is to use historical vehicle data to train a regression model that predicts an estimated car price from its attributes.

## Objectives

- Explore and understand the vehicle dataset.
- Clean the data and handle missing or inconsistent values.
- Perform exploratory data analysis (EDA).
- Prepare numerical and categorical features for machine learning.
- Train and evaluate regression models.
- Predict an estimated price for a vehicle.

## Technologies Used

- **Python** — programming language
- **Pandas** — data manipulation
- **NumPy** — numerical operations
- **Matplotlib / Seaborn** — data visualization
- **Scikit-learn** — preprocessing, model training, and evaluation
- **Jupyter Notebook** — experimentation and analysis

## Dataset

Use a vehicle dataset in CSV format. The available columns depend on the dataset. Common features include:

| Feature | Description |
|---|---|
| `brand` / `name` | Vehicle manufacturer or model name |
| `year` | Manufacturing year |
| `km_driven` / `mileage` | Distance driven or mileage, depending on the dataset |
| `fuel` | Fuel type, such as petrol, diesel, or CNG |
| `transmission` | Manual or automatic |
| `owner` | Previous-owner category, if available |
| `selling_price` / `price` | Target value to predict |

**Important:** Dataset column names vary. Update the code and this README to match the dataset you actually use. Do not treat mileage and kilometres driven as the same feature.

## Project Workflow

1. Load the vehicle dataset.
2. Inspect data types, summary statistics, duplicates, and missing values.
3. Clean the data and investigate unusual prices or values.
4. Explore how vehicle attributes relate to selling price.
5. Separate input features (`X`) and the target price (`y`).
6. Encode categorical features and split the data into training and testing sets.
7. Train one or more regression models, such as Linear Regression, Random Forest Regressor, or Gradient Boosting.
8. Evaluate the model using MAE, RMSE, and R².
9. Use the trained model to estimate prices for new vehicle details.

## Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

### 2. Create a virtual environment (optional)

```bash
python -m venv .venv
```

On Windows:

```bash
.venv\Scripts\activate
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

If your project uses a `requirements.txt` file, install dependencies with:

```bash
pip install -r requirements.txt
```

### 4. Add the dataset

Place the CSV dataset in the project directory or update the file path in your notebook or Python script.

### 5. Run the project

For a Jupyter Notebook:

```bash
jupyter notebook
```

Open the automobile price prediction notebook and run the cells in order.

For a Python script, if your entry-point file is named `main.py`:

```bash
python main.py
```

## Model Evaluation

- **MAE (Mean Absolute Error):** Average absolute difference between actual and predicted prices.
- **RMSE (Root Mean Squared Error):** Penalizes larger prediction errors more strongly.
- **R² Score:** Measures the proportion of target-price variation explained by the model on the evaluation data.

Record your actual evaluation results here after running the project. Do not report an accuracy or score unless you have measured it on your dataset.

## Suggested Repository Structure

```text
automobile-price-prediction/
├── dataset/
│   └── vehicles.csv
├── notebooks/
│   └── automobile_price_prediction.ipynb
├── main.py
├── requirements.txt
└── README.md
```

This is a suggested structure. Keep only the folders and files that exist in your repository, and update the filenames as needed.

## Future Improvements

- Compare several regression algorithms and tune their hyperparameters.
- Improve handling of vehicle brands and models.
- Build a prediction interface using Streamlit or Flask.
- Save the preprocessing steps and trained model in a reusable pipeline.
- Add more recent data to help reflect changing market prices.

## Limitations

Predictions depend on the quality, size, and recency of the dataset. Vehicle condition, accident history, regional demand, and other factors may not be represented. The output is an estimate, not a guaranteed market valuation.

## Author

**Musale Devendra**  

