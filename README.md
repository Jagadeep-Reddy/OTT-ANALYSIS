# OTT-ANALYSIS
OTT Content Viewership Prediction
This repository contains an end-to-end data analysis and predictive modeling project for an OTT (Over-The-Top) platform, using a linear regression model to predict content viewership and provide actionable business insights.

Table of Contents
Project Overview

Repository Contents

Methodology

Key Recommendations

Dependencies

How to Run the Project

License

1. Project Overview
The primary objective of this project is to identify the key variables that influence content viewership on an OTT platform. By developing a predictive model, the goal is to provide data-backed insights to guide business decisions related to content acquisition, marketing, and scheduling. The analysis helps answer the critical business question: "What drives a piece of content to be successful?"

2. Repository Contents
This repository contains the following files:

OTT_Data_Analysis_and_Linear_Regression_Model_1.ipynb: A Jupyter Notebook containing all the Python code for data preprocessing, exploratory data analysis (EDA), model building, and evaluation.

OTT_Platform_Business_Report.md: A business report summarizing the project's findings and providing actionable recommendations for business stakeholders and subject matter experts.

ottdata (1).csv: The raw dataset used for the analysis.

3. Methodology
The project follows a standard data science workflow:

Data Preparation: The raw data was cleaned by handling missing values (using median/mode imputation), removing duplicates, and treating outliers via the Interquartile Range (IQR) method.

Feature Engineering: A new feature, total_views, was created to combine trailer and content views for a more holistic view. Categorical variables (genre, dayofweek, season) were converted into numerical format using one-hot encoding.

Exploratory Data Analysis (EDA): A comprehensive univariate and bivariate analysis was conducted to understand the distribution of variables and identify initial relationships, such as the strong correlation between trailer views and content views.

Predictive Modeling: A linear regression model was chosen for its interpretability. The model was trained on a split of the dataset (80% training, 20% testing) to predict content viewership.

Model Evaluation: The model's performance was evaluated using R-squared, Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). The assumptions of linear regression were validated using residual plots and a Variance Inflation Factor (VIF) check.

4. Key Recommendations
Based on the model's findings, the following recommendations are provided to the OTT platform:

Prioritize Trailer Quality: Trailer views are the single most important predictor of content viewership. Investment in high-quality, engaging trailers and their promotion should be a top priority for the marketing team.

Optimize Release Schedule: Strategically release major content on weekends and during the Fall and Winter seasons, as these periods demonstrate higher viewership.

Invest in High-Demand Genres: The "Action" and "Sci-Fi" genres consistently perform well. The content acquisition team should focus on acquiring or producing more content in these genres.

Capitalize on Overall Platform Traffic: Increasing overall platform traffic (visitors and ad impressions) has a direct positive impact on content views. Broad marketing campaigns should be leveraged to drive user acquisition.

5. Dependencies
The following Python libraries are required to run the Jupyter Notebook:

pandas

numpy

matplotlib

seaborn

statsmodels

scikit-learn

You can install these dependencies using pip:

pip install pandas numpy matplotlib seaborn statsmodels scikit-learn

6. How to Run the Project
Clone the repository:

git clone [repository-url]
cd [repository-name]

Install the dependencies (if you haven't already):

pip install -r requirements.txt

(Note: If requirements.txt is not provided, use the pip install command from the Dependencies section).

Open the Jupyter Notebook:

jupyter notebook

Navigate to OTT_Data_Analysis_and_Linear_Regression_Model_1.ipynb and run the cells sequentially.

7. License
This project is licensed under the MIT License.
