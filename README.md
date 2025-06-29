### 🚗 Car Price Prediction Using Machine Learning
This project predicts the selling price of used cars based on key features like brand, model name, year, fuel type, kilometers driven, and more. It uses Random Forest Regressor with log transformation, hyperparameter tuning, and label encoding for accurate results.

### 📂 Project Structure
bash
Copy
Edit
├── Cars_24.ipynb      # Jupyter notebook with full workflow
├── README.md          # Project documentation
├── cars_24.csv        # Project CSV File
📈 Features Used
Name (Model name of the car)

Brand

Year

Distance Driven

Owner Count

Fuel Type

Location

Drive Type (Manual/Automatic)

Car Type (SUV, Sedan, etc.)

### 🧠 Model Details
Model: RandomForestRegressor

R² Score: ~83.6%

MAE: ~₹64,000

Log Transformation applied to target variable for better handling of price distribution

Hyperparameter Tuning done via GridSearchCV

### 🚀 How to Use
Install dependencies

bash
Copy
Edit
pip install pandas numpy scikit-learn
Run the notebook
Open Cars_24.ipynb in Jupyter Notebook or any compatible IDE.

Use the interactive input

python
Copy
Edit
NAME = input("Name")
...
Get the price prediction
Output will be something like:

yaml
Copy
Edit
Predicted Price: ₹6,03,000
### 🔄 Data Preprocessing
All categorical features (Name, Brand, Fuel, etc.) are label encoded using OrdinalEncoder.

Target variable Price is transformed using np.log1p() and predictions are reversed with np.expm1().
