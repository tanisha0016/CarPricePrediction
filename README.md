# CarPricePrediction

---

This project involves predicting the selling price of used cars based on various features using Linear Regression and Lasso Regression models. The dataset used contains details about different cars, including their present price, driven kilometers, fuel type, and other attributes.

## Dataset

The dataset used in this project contains 301 entries with the following columns:
- `Car_Name`: The name of the car.
- `Year`: The year the car was purchased.
- `Selling_Price`: The price at which the car is being sold.
- `Present_Price`: The current ex-showroom price of the car.
- `Driven_kms`: The distance driven by the car in kilometers.
- `Fuel_Type`: The type of fuel used by the car (Petrol, Diesel, CNG).
- `Selling_type`: Whether the seller is a dealer or an individual.
- `Transmission`: The type of transmission (Manual, Automatic).
- `Owner`: The number of previous owners of the car.

## Dependencies

The following Python libraries are required to run the code in this project:
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

You can install these libraries using pip:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## Data Preprocessing

- Replaced categorical values in `Fuel_Type`, `Selling_type`, and `Transmission` columns with numerical values.
- Split the data into features (X) and target (Y) variables. Dropped the `Car_Name` and `Selling_Price` columns from the features.

## Model Training and Evaluation

### Linear Regression

- Split the data into training and test sets with a test size of 10%.
- Trained a Linear Regression model on the training data.
- Evaluated the model using R squared error and plotted the actual vs. predicted prices for both training and test sets.

### Lasso Regression

- Trained a Lasso Regression model on the same training data.
- Evaluated the model using R squared error and plotted the actual vs. predicted prices for both training and test sets.

## Results

### Linear Regression

- R squared error on training data: 0.8796
- R squared error on test data: 0.8366

### Lasso Regression

- R squared error on training data: 0.8424
- R squared error on test data: 0.8710

## Conclusion

Both Linear Regression and Lasso Regression models performed well in predicting the selling price of used cars. The Lasso Regression model showed slightly better performance on the test data.

## Code

You can find the code for this project in the [car_price_prediction.ipynb](car_price_prediction.ipynb) notebook.

## Usage

To run this project, you can use Google Colab. Open the notebook in Colab and follow the instructions to execute the code cells.

## License

This project is licensed under the MIT License.

---

