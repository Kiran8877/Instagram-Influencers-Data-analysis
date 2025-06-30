# Instagram-Influencers-Data-analysis
Instagram Influencers Data Analysis
This project presents a detailed analysis of an Instagram influencer dataset consisting of global influencer profiles. The objective is to extract insights into follower dynamics, engagement rates, regional influence trends, and performance predictors using data cleaning, visual analytics, statistical testing, and regression modeling.

Project Overview
Loaded and cleaned the dataset by parsing formatted numbers (e.g., "1.2K", "475.8M"), removing duplicates, and handling missing values.

Conducted exploratory data analysis (EDA) to identify trends in influencer count, average engagement rates by country, and relationships among numerical metrics.

Performed statistical hypothesis testing including T-tests and Z-tests to examine differences in engagement across follower groups and against benchmark values.

Applied feature engineering to improve regression modeling by generating log-transformed features, categorical bins, interaction terms, and dummy variables.

Developed multiple linear regression models to predict influencer engagement and validate model performance using R² scores and error metrics.

Tools and Libraries Used
The following Python libraries were used to perform the analysis:

Pandas and NumPy: For data cleaning and manipulation

Matplotlib and Seaborn: For plotting visualizations

Scipy: For statistical hypothesis testing (T-test, Z-test)

Scikit-learn: For regression modeling and evaluation

Warnings: Suppressed to ensure clean output

Key Steps and Insights
1. Data Cleaning and Preprocessing
Parsed formatted strings such as "14.5K" and "2.3M" into numeric types for analysis.

Removed unnecessary characters from percentage and numerical fields.

Filled missing values using mode (for categorical fields like country) or dropped incomplete records.

Final cleaned dataset was verified for data type consistency and completeness.

2. Exploratory Data Analysis
Distribution of Influence Scores: Most influencers had influence scores in the range of 60–80.

Top 10 Countries by Influencer Count: USA, India, and Brazil had the highest number of influencers.

Correlation Heatmap: Strong correlation observed between followers and average likes.

Engagement vs Followers: Influencers with more followers tended to have lower engagement rates.

Boxplots by Country: Engagement rate variation and outliers observed across countries.

3. Statistical Testing
T-Test: Compared engagement rate between high and low follower groups. The difference was statistically significant (p < 0.05).

Z-Test: Tested whether mean engagement rate differs from a benchmark (e.g., 100). Result showed significant deviation.

4. Feature Engineering
Created additional features to improve model accuracy:

Log Transforms: Log_Followers, Log_Posts, Log_Avg_Likes

Follower Bins: Categorized into Small, Medium, Large, Very Large

Interaction Term: Posts × Engagement Rate

Boolean Flag: High Average Likes

One-hot Encoding: Applied to country and follower bins

5. Regression Modeling
Built a baseline regression model using numerical variables such as followers, average likes, and engagement rate.

Developed an enhanced model with engineered features and country-based dummy variables.

The final model showed improved R² scores and better residual distribution, confirming the effectiveness of feature engineering.

Files Included
Instgram influencers analysis.ipynb – Jupyter Notebook containing full analysis and model development steps.

Instagram influencers analytical Dashboard.xlsx – Excel dashboard for stakeholder-friendly summary visuals.

Instagram influencers analysis summary report.pdf – PDF document summarizing methods, visualizations, and key findings.

Author
K. Kiran Sai Karthik
Email: kanagarlakiransaikarthik@gmail.com

