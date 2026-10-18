# AI-Based Customer Spending Category Prediction

## Project Overview

This project focuses on predicting customer spending categories using machine learning techniques. It uses customer demographic information, such as age and gender, along with annual income to classify customers into Low, Medium, or High spending categories.

The project was completed as part of an internship task at **Veda Technology** to practice data analysis, visualization, and machine learning.

## Objectives

- Analyze customer data to understand spending patterns.
- Clean and preprocess the dataset.
- Perform Exploratory Data Analysis (EDA).
- Build machine learning classification models.
- Compare model performance using evaluation metrics.
- Predict the spending category of a new customer.
- Identify useful insights for customer segmentation.

## Dataset

The project uses the Mall Customers dataset, which contains information about customers, including:

- Customer ID
- Gender
- Age
- Annual Income
- Spending Score

Dataset source: [Mall Customers Dataset](https://github.com/MahimaSriK/Mall-Customer-Segmentation-Dataset)

The spending categories are created from the existing spending score:

- **Low:** Score from 1 to 33
- **Medium:** Score from 34 to 66
- **High:** Score from 67 to 100

These thresholds are used for this project and are not official business-defined customer categories.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### 1. Data Loading
Loaded the Mall Customers dataset into a Pandas DataFrame.

### 2. Data Cleaning
- Checked and handled missing values.
- Removed duplicate records.
- Converted numeric columns to appropriate data types.
- Validated the age, income, and spending score values.

### 3. Exploratory Data Analysis
Created visualizations to study:
- Customer age distribution
- Annual income distribution
- Spending score distribution
- Spending category counts
- Age versus spending score
- Annual income versus spending score
- Correlations between numeric variables

### 4. Feature Engineering
Created a target column named `Spending Category` using the spending score.

### 5. Model Training
Trained two classification models:

- Logistic Regression
- Random Forest Classifier

The input features used for prediction are gender, age, and annual income.

### 6. Model Evaluation
Evaluated the models using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

The model with the higher weighted F1-score is selected for the sample prediction.

### 7. Customer Prediction
Created a prediction function that accepts a customer's gender, age, and annual income and returns the predicted spending category.

### 8. Business Insights
Compared average age, annual income, and spending score across spending categories to identify customer patterns.

## How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Open the project notebook in Jupyter Notebook.
4. Run the cells sequentially from top to bottom.
5. Review the visualizations, model evaluation results, and sample prediction.

The notebook loads the dataset directly from its public GitHub CSV URL, so a separate local CSV file is not required when internet access is available.

## Results

The notebook compares Logistic Regression and Random Forest using multiple classification metrics. Actual model scores and visualizations are generated when the notebook is executed.

The results should be taken directly from the executed notebook rather than assumed in advance.

## Limitations

The spending categories are derived from the existing spending score, while the model predicts these categories using gender, age, and annual income. Therefore, the model demonstrates a machine learning workflow but does not establish actual future spending behavior or real-world business performance.

## Conclusion

This project provided practical experience in data cleaning, exploratory data analysis, feature engineering, classification, and model evaluation. It also demonstrated how customer data can be analyzed to support basic customer segmentation and business decision-making.

## Author

Completed as part of the Veda Technology internship project.
