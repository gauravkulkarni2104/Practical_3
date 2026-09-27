# House Price Prediction using Linear Regression (Gradient Descent vs Scikit-learn)

## Aim
To build a regression model that predicts house prices from house area, implementing Linear Regression from scratch using Gradient Descent, and comparing it with Scikit-learn's Linear Regression model.

## Project Structure
```
house-price-prediction-gd/
├── house_price_prediction.py   # Main source code
├── requirements.txt            # Python dependencies
├── results/                    # Output screenshots / plots go here
└── README.md
```

## Dataset
The dataset is a small synthetic dataset of house area (sq. ft.) and price (lakhs), defined directly inside the script. No external file is required.

## How to Run
1. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
2. Run the script:
   ```
   python house_price_prediction.py
   ```
3. Console output will show the slope, intercept, and evaluation metrics (MAE, MSE, RMSE, R²) for both models. Three plots will also be generated and saved automatically into the `results/` folder:
   - `actual_vs_predicted.png`
   - `gradient_descent_cost.png`
   - `regression_line.png`

## Sample Output
```
SCIKIT-LEARN LINEAR REGRESSION
Slope: 0.0258...
Intercept: 4.32...

GRADIENT DESCENT
Slope: 0.0257...
Intercept: 4.30...
Final Training MSE: 0.85...

 Scikit-learn Model
MAE: 0.42
MSE: 0.25
RMSE: 0.50
R2 Score: 0.998

 Gradient Descent Model
MAE: 0.44
MSE: 0.27
RMSE: 0.52
R2 Score: 0.997

HOUSE PRICE PREDICTION
Area: 1500 sq. ft.
Scikit-learn Prediction: 43.11 lakhs
Gradient Descent Prediction: 43.08 lakhs
```

## Results
See the `results/` folder for the actual output screenshots and plots generated after running the script.

## Conclusion
Both models produce very similar slope, intercept, and evaluation metric values, confirming that the manually implemented Gradient Descent algorithm converges close to the direct least-squares solution computed by Scikit-learn.
