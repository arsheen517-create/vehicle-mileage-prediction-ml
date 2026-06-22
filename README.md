# vehicle-mileage-prediction-ml
A Machine Learning project focused on predicting vehicle mileage (MPG) using regression analysis. The model evaluates key features such as cylinders, displacement, horsepower, weight, acceleration, and model year from the Auto MPG dataset. Built using scikit-learn, it achieves an R-squared score of 84.75% and includes clean data visualizations.

**Aim of the project:** To forecast the future mileage or usage of a vehicle, typically based on its past behavior & various factors.

## 1. Objective
To predict the mileage (mpg) of cars based on various features such as cylinders, displacement, horsepower, weight, acceleration, model year, and origin using regression analysis.

## 2. Data Source
We used a dataset resembling the Auto MPG dataset sourced from the UCI Machine Learning Repository, containing information about various car attributes and their mileage.

## 3. Tech Stack & Libraries
**Language:** Python
**Libraries:** `pandas`, `numpy`, `matplotlib`, `scikit-learn`

## 4. Project Workflow

### 1. Data Preprocessing
Handled missing values in the `horsepower` column by replacing invalid `'?'` characters with `NaN`.
Imputed missing values using the median horsepower value (**93.5**).

### 2. Feature & Target Selection
**Features ($X$):** `cylinders`, `displacement`, `horsepower`, `weight`, `acceleration`, `model year`, `origin`
**Target ($y$):** `mpg`

### 3. Model Training
**Train-Test Split:** 80% Training, 20% Testing (`random_state=42`).
**Model:** Linear Regression.

### 4. Model Evaluation
**Mean Squared Error (MSE):** `8.1977`
**R-squared ($R^2$ Score):** `0.8475` (84.75% of the variance explained by the model)

## 5. Visualizations

### Weight vs MPG
Shows the negative correlation between a vehicle's weight and its fuel efficiency.
![Weight vs MPG](plots/weight_vs_mpg.png)

### Actual vs Predicted MPG
Displays model predictions against actual values. The red line represents perfect predictions.
![Actual vs Predicted MPG](plots/actual_vs_predicted_mpg.png)

## 6. How to Run

### Run Locally:
1. Clone this repository.
2. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the analysis script:
   ```bash
   python mileage_prediction.py
   ```

### Run on Google Colab:
You can also open a new notebook in Google Colab, copy the cells from `mileage_prediction.py`, and run them directly in your browser.

