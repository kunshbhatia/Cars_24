### 🚗 Car Price Prediction Using Machine Learning
This project predicts the selling price of used cars based on key features like brand, model name, year, fuel type, kilometers driven, and more. It uses Random Forest Regressor with log transformation, hyperparameter tuning, and label encoding for accurate results.

### 📂 Project Structure

1) Cars_24.ipynb      # Jupyter notebook with full workflow
2) README.md          # Project documentation
3) cars_24.csv        # Project CSV File 

### 📈 Features Used
1) Name (Model name of the car)
2) Brand
3) Year
4) Distance Driven
5) Owner Count
6) Fuel Type
7) Location
8) Drive Type (Manual/Automatic)
9) Car Type (SUV, Sedan, etc.)

### 🧠 Model Details
Model: RandomForestRegressor

R² Score: ~83.6%

MAE: ~₹64,000

Log Transformation applied to target variable for better handling of price distribution

Hyperparameter Tuning done via RandomsearchCV

### 🚀 How to Use
Install dependencies
pip install pandas numpy scikit-learn
Run the notebook
Open Cars_24.ipynb in Jupyter Notebook or any compatible IDE.

### 🔄 Data Preprocessing
All categorical features (Name, Brand, Fuel, etc.) are label encoded using OrdinalEncoder.

Target variable Price is transformed using np.log1p() and predictions are reversed with np.expm1().
