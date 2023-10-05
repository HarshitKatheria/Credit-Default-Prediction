# Credit Default Prediction

![](https://images.unsplash.com/photo-1589758438368-0ad531db3366?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1932&q=80)

## Table of Contents

- [Introduction](#introduction)
- [Files in this Repository](#files-in-this-repository)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Welcome to the Credit Default Prediction project! This repository contains a machine learning model for predicting credit default risks. Credit default prediction is crucial in the financial industry to assess the likelihood of a borrower failing to repay their debt.

In this project, we've developed a predictive model that takes various financial and personal attributes of borrowers as input and predicts whether they are likely to default on their credit.

## Files in this Repository

- `EDA.ipynb`: Jupyter Notebook containing exploratory data analysis of the dataset.
- `LICENSE`: The project's license file.
- `README.md`: The main README file that provides an overview of the project.
- `main.ipynb`: Jupyter Notebook containing the main code for the credit default prediction model.
- `requirements.txt`: File listing the required Python packages for this project.
- `streamlit_app.py`: Python script for creating a Streamlit web application for the model.
- `webappmodel.joblib`: A trained machine learning model saved as a joblib file.

## Dataset

We used the [GiveMeSomeCredit dataset](https://www.kaggle.com/c/GiveMeSomeCredit) from Kaggle for training and evaluation. This dataset contains the following features:

- `RevolvingUtilizationOfUnsecuredLines`: This feature represents the total balance on credit cards and personal lines of credit, divided by the sum of credit limits. It is a measure of how much credit is being used relative to the total available credit.

- `age`: The age of the borrower.

- `NumberOfTime30-59DaysPastDueNotWorse`: The number of times the borrower has been 30-59 days past due (but not worse) on any credit obligation in the last two years.

- `DebtRatio`: This feature represents the monthly debt payments, including alimony and living costs, divided by the monthly gross income.

- `MonthlyIncome`: The monthly income of the borrower.

- `NumberOfOpenCreditLinesAndLoans`: The number of open credit lines (e.g., credit cards or loans) the borrower has.

- `NumberOfTimes90DaysLate`: The number of times the borrower has been 90 days or more past due on any credit obligation.

- `NumberRealEstateLoansOrLines`: The number of real estate loans or lines of credit the borrower has.

- `NumberOfTime60-89DaysPastDueNotWorse`: The number of times the borrower has been 60-89 days past due (but not worse) on any credit obligation in the last two years.

- `NumberOfDependents`: The number of dependents the borrower has.

The target variable for this dataset is:

- `SeriousDlqin2yrs`: This is a binary target variable. It indicates whether a borrower experienced a serious delinquency (1) or not (0) within two years.

Before running the code, make sure to download and place the dataset in the `data` directory.


## Installation

To run this project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/HarshitKatheria/Credit-Default-Prediction.git
   cd Credit-Default-Prediction
   ```

2. Install the required python packages:
```bash
pip install -r requirements.txt
```
3. Run the project:
```bash
python main.py
```
## Web Application

We've created a web application for this credit default prediction model using Streamlit. With the web app, you can easily interact with and make predictions using the trained model.

To run the web application locally, follow these steps:

1. Make sure you've completed the [Installation](#installation) steps to set up the project on your machine.

2. Open a terminal and navigate to the project directory.

3. Run the Streamlit app with the following command:

   ```bash
   streamlit run streamlit_app.py
   ```
   

https://github.com/HarshitKatheria/Credit-Default-Prediction/assets/123855321/f685c208-6f4d-481a-af2f-cb170f07262a



## Usage

To use the credit default prediction model, follow these steps:

1. Install the project as mentioned in the [Installation](#installation) section.

2. Open the `main.ipynb` Jupyter Notebook where you've performed the modeling.

3. Preprocess your data within the `main.ipynb` notebook if you have your own dataset. You can use the provided dataset as a reference.

4. Train the model within the `main.ipynb` notebook using your data.

5. Evaluate the model within the `main.ipynb` notebook. Assess its performance and make predictions on new data as needed.

# License

This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to reach out if you have any questions or need further assistance with this project. Happy predicting!



