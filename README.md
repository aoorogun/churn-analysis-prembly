# churn-analysis-prembly



## Overview
This project focuses on **churn analysis** for Prembly Inc, identifying customer retention patterns, and predicting churn behavior based on historical data. The analysis is performed using two Jupyter notebooks:
- `Churn EDA.ipynb`: Exploratory Data Analysis (EDA) on customer activity, transaction logs, and churn behavior.
- `Churn.ipynb`: In-depth analysis of churn trends over a **nine-month** and **three-month** period.

## Objectives
1. Define and analyze churn trends over multiple timeframes.
2. Identify key factors contributing to customer churn.
3. Perform time-series and correlation analysis.
4. Develop predictive models for churn classification.
5. Provide actionable insights to reduce churn rates.

## Dataset
The data comprises **API usage logs, wallet transactions, business registrations, and customer demographics**. The key attributes include:
- `business_name`: Name of the business.
- `total_calls`: Number of API calls made.
- `success_calls`: Number of successful API calls.
- `churn_status`: Whether a business has churned or not.
- `country`: The country of registration.
- `lead_source`: How the customer was acquired.
- `document_upload`: Whether business documents were provided.
- `wallet_topups`: Transaction history related to wallet funding.
- `endpoints_called`: Specific API endpoints accessed by customers.

## Methodology
### 1. **Exploratory Data Analysis (EDA)**
- Cleaning and preprocessing of data.
- Distribution of customers by success rate, country, and sector.
- Customer segmentation based on activity levels.
- Time-series analysis of API calls and revenue trends.
- Correlation analysis of churn-related factors.

### 2. **Churn Analysis**
- Identification of churned customers over **three-month** and **nine-month** periods.
- Breakdown by signup date, country, lead source, and industry sector.
- Analysis of failed API calls and server errors.
- Wallet funding behavior of churned customers.
- Endpoint usage trends among churned customers.

### 3. **Predictive Modeling**
- Feature engineering to create class labels.
- Splitting data into training and testing sets.
- Training machine learning models for churn prediction.
- Evaluating model performance using accuracy, precision, recall, and F1-score.

## Key Insights
- The highest churn rate was observed among businesses that **never successfully used the API**.
- Businesses with **no referral source** had a higher likelihood of churn.
- The **NIN and Voter ID API endpoints** had the highest number of failed calls from churned customers.
- **Most churned customers signed up in June and April**, indicating seasonal patterns in customer retention.
- **Wallet funding activity was low among churned customers**, suggesting a direct correlation between financial engagement and retention.

## Next Steps
- Improve API reliability and reduce server errors.
- Enhance customer onboarding experience to improve first-time success rates.
- Offer targeted retention strategies based on churn risk factors.
- Further refine predictive models to enhance churn forecasting accuracy.

## Installation & Usage
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn

### Running the Notebooks
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/churn-analysis.git
   ```
2. Navigate to the project directory:
   ```sh
   cd churn-analysis
   ```
3. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
4. Open Jupyter Notebook:
   ```sh
   jupyter notebook
   ```
5. Run the `Churn EDA.ipynb` and `Churn.ipynb` notebooks step by step.

## Contributors
- Okunola Orogun
- Akinrolabu 'Tunde
## License
This project is licensed under the MIT License.

