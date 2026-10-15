# 🏠 House Price Prediction Using Machine Learning

## 📌 Project Overview
House Price Prediction is a Machine Learning project that predicts house prices based on various property features. This project uses regression algorithms to estimate house prices and evaluate model performance.

The project implements **Linear Regression** and **Decision Tree Regression** to predict house prices in lakhs.

## 🎯 Objectives
- Predict house prices using Machine Learning.
- Perform Exploratory Data Analysis (EDA).
- Clean and preprocess the dataset.
- Encode categorical features into numerical values.
- Train and evaluate regression models.
- Save the trained model for future use.

## 🛠️ Technologies Used
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Development Environment:** Jupyter Notebook
- **Model Saving:** Pickle

## 📂 Project Structure

```text
House-Price-Prediction/
│
├── E06_House_Price_Prediction.ipynb
├── E06_house price data less.csv
├── house_price_model.pkl
├── vectorizer.pkl
├── encoder.pkl
├── features.pkl
└── README.md
```

## 📊 Dataset Description
The project uses a house price dataset containing property-related information.

The target variable is:
- `Price_in_Lakhs` — the price of the house in lakhs.

The notebook processes features such as:
- Property Type
- Furnished Status
- Public Transport Accessibility
- Facing
- Security
- Other available numerical and categorical property features

**Note:** The CSV dataset must be available in the project directory to run the notebook.

## ⚙️ Project Workflow

### 1. Data Loading
Load the dataset using Pandas and inspect the records, columns, data types, and dataset dimensions.

### 2. Exploratory Data Analysis (EDA)
- Check the dataset structure.
- Identify missing values.
- Generate descriptive statistics.
- Analyze numerical and categorical features.
- Visualize correlations using a heatmap.

### 3. Data Preprocessing
- Drop the irrelevant `ID` column.
- Remove the `Locality` column.
- Encode ordinal categorical features using `OrdinalEncoder`.
- Convert categorical text to lowercase.
- Separate categorical and numerical columns.

### 4. Feature Engineering
Use `DictVectorizer` to convert the feature dictionaries into a numerical representation suitable for Machine Learning models.

### 5. Model Training
Train the following regression algorithms:

**Linear Regression:** Predicts house prices by learning linear relationships between input features and the target.

**Decision Tree Regression:** Predicts house prices by learning decision rules from the input features.

### 6. Model Evaluation
Evaluate model performance using:
- **MAE:** Mean Absolute Error
- **MSE:** Mean Squared Error
- **RMSE:** Root Mean Squared Error
- **R² Score:** Measures how well the model explains variations in house prices.

### 7. Model Saving
Save the trained Decision Tree model and preprocessing-related objects using Pickle for potential reuse.

## 📈 Results
The notebook evaluates both Linear Regression and Decision Tree Regression.

The final performance should be assessed using the calculated MAE, MSE, RMSE, and R² Score values. The notebook does not establish a verified numerical result in this README, so actual scores should be added after running the experiment.

## 🚀 How to Run the Project

**Step 1: Clone the repository**
```bash
git clone <your-github-repository-url>
```

**Step 2: Open the project folder**
```bash
cd House-Price-Prediction
```

**Step 3: Install the required libraries**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**Step 4: Start Jupyter Notebook**
```bash
jupyter notebook
```

**Step 5:** Open `E06_House_Price_Prediction.ipynb` and run the cells in order.

Make sure the dataset CSV file is in the correct directory before running the notebook.

## 💡 Applications
- Real estate price estimation
- Property market analysis
- Preliminary property valuation
- Understanding factors affecting house prices

## 🔮 Future Enhancements
- Develop a web application using Streamlit.
- Add an interactive interface for entering property details.
- Compare additional regression algorithms.
- Improve model performance through hyperparameter tuning.
- Display predicted prices and model evaluation results visually.

## 🏁 Conclusion
This project demonstrates how Machine Learning can be used to predict house prices. It includes data exploration, preprocessing, feature encoding, regression model training, performance evaluation, and model saving. It provides practical experience in applying Python and Scikit-learn to a real-world regression problem.

