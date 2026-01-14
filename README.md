Task 2: House Price Prediction

🎯 Objective

The objective of this task is to predict house prices using property-related features by applying a Linear Regression model. This task demonstrates the complete machine learning workflow including data loading, preprocessing, model training, evaluation, and visualization.

📊 Dataset Used

File Name: house_prices.csv

Location: Same folder (Internship_new)

Target Variable: price

Features: Numeric and optional categorical features (e.g., location, area, rooms, etc.)

⚠️ The dataset must include a price column for model training.

🛠️ Libraries Used

pandas – data loading and manipulation

matplotlib – visualization

seaborn – correlation heatmap

scikit-learn – model training and evaluation

numpy – numerical computations

🔍 Steps Performed
1️⃣ Import Libraries

All required Python libraries are imported for data analysis, visualization, and machine learning.

2️⃣ Load Dataset

The dataset is loaded using:

pd.read_csv("house_prices.csv")


Initial exploration includes:

First 5 rows preview

Dataset shape

Column names

3️⃣ Explore Dataset

Summary statistics using describe()

Missing values detection

Correlation heatmap to understand relationships between features

Heatmap saved as: correlation_heatmap.png

4️⃣ Data Preprocessing

Categorical features (such as location) are converted using one-hot encoding

Missing values are removed for simplicity

Dataset is prepared for model training

5️⃣ Feature & Target Selection

Features (X): All columns except price

Target (y): price

Data split into training and testing sets (80% / 20%)

6️⃣ Model Training

Linear Regression model is trained using training data

Predictions are made on the test set

7️⃣ Model Evaluation

Model performance is evaluated using:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

These metrics measure how close the predicted prices are to actual prices.

8️⃣ Visualization

Scatter plot of Actual vs Predicted Prices

Helps visually assess model accuracy

Saved as: actual_vs_predicted.png

📌 Key Insights

Linear Regression can effectively model house prices using numeric features

MAE and RMSE provide useful error measurements

Correlation heatmap helps in understanding influential features

Prediction plot shows how closely the model follows actual prices

📂 Generated Files

After execution, the following files are saved:

correlation_heatmap.png

actual_vs_predicted.png

✅ Conclusion

This task demonstrates a complete regression-based machine learning pipeline, including preprocessing, modeling, evaluation, and visualization. It provides a solid foundation for more advanced models such as Random Forest or Gradient Boosting.