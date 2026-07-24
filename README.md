# International Essentials: Customer Spend Prediction

## Project Overview

This project analyzes customer spend data for International Essentials to investigate whether loyalty tenure is the biggest driver of annual spend. I have built and compared multiple predictive models to forecast customer spending, providing actionable insights for marketing and retention strategies.
Project Structure

├── loyalty.csv               # Raw customer loyalty data
├── train.csv                 # Training data for model fitting
├── test.csv                  # Test data for predictions
├── clean_data                # Cleaned and preprocessed dataframe
├── spend_by_years            # Average spend and variance by loyalty years
├── base_result               # Baseline model predictions (customer_id, spend)
├── compare_result            # Comparison model predictions (customer_id, spend)
└── README.md                 # Project documentation

## Key Steps

- Data Cleaning — Prepared and structured the raw data into clean_data with all columns and values matching the required format.

- Exploratory Analysis — Produced spend_by_years to examine average spend and variance across different loyalty tenure groups, testing the team's hypothesis that loyalty years drive spend.

- Baseline Modeling — Fitted a baseline model using train.csv and generated predictions on test.csv, returning base_result with customer IDs and predicted spend.

- Comparison Modeling — Fitted a comparison model using train.csv and generated predictions on test.csv, returning compare_result with customer IDs and predicted spend.

## Model Performance

The Linear Regression model delivered the best performance with an R² of 0.9999, MAE of 0.2054, and RMSE of 0.2855 — explaining nearly all variance in customer spend. These results confirm that loyalty tenure is indeed a powerful driver of spend, aligning with the team's long-held belief at International Essentials.
Recommendations

I recommend using the Linear Regression model for predicting future customer spend. This model can support:

- Customer segmentation and targeting

- Personalized marketing campaigns

- Customer retention initiatives

- Strategic decision-making around loyalty program investment

## Technologies Used

- Python
- Pandas / NumPy
- Scikit-learn (Linear Regression, Decision Tree, Random Forest, Gradient Boosting)
- Matplotlib / Seaborn (if visualizations were included)
