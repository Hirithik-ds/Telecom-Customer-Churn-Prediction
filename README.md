# Telecom-Customer-Churn-Prediction

# Problem Statement

In the telecom industry, customers are able to choose from a pool of companies to cater their needs regarding communication and internet. Customers are very critical about the kind of services they receive and judge the entire company based on a single experience! These communication services have become so recurrent and inseparable from the daily routine that a 30 minute maintenance break kicks in anxiety in the users highlighting our taken-for-granted attitude towards these services! Coupled with high customer acquisition costs, churn analysis becomes very pivotal! Churn rate is a metric that describes the number of customers that cancelled or did not renew their subscription with the company. Thus, higher the churn rate, more customers stop buying from your business, directly affecting the revenue! Hence, based on the insights gained from the churn analysis, companies can build strategies, target segments, improve the quality of the services being provided to improve the customer experience, thus cultivating trust with the customers. That is why building predictive models and creating reports of churn analysis becomes key that paves the way for growth!

**The following libraries were used in this project:**

- Pandas 🐼: For handling and analyzing the data.
- NumPy 📐: For performing numerical operations.
- Matplotlib & Seaborn 📊: For visualizing the data.
- Scikit-learn 🤖: For building, evaluating, and deploying the models.

# ⚙️ Data Preprocessing
**The preprocessing steps included:**

- Handling Missing Values 🧩: Filling in missing values to ensure data completeness.
- Feature Engineering 🔧: Creating additional features that could provide better predictive power.
- Encoding Categorical Variables 🔢: Converting categorical variables into numerical values for model use.
- Splitting the Data ✂️: Dividing the data into training and test sets for model evaluation.
  
# 📊 Exploratory Data Analysis (EDA)

- EDA was conducted to understand the distribution and relationships between the features. Key visualizations and insights were:

![image](https://github.com/user-attachments/assets/b75de1f4-9eea-4a7c-828a-a39c7ec0a5ee)

**Distribution of Tenure:**

- High concentration of customers having very low tenure near zero. This suggests that many customers leave shortly after joining.
- There are some peaks at specific tenure points e.g., around 70+ months, possibly indicating long-term loyal customers.
- The presence of peaks at both low and high tenure values suggests two major customer groups:
- New customers who tend to churn early.
- Long-term subscribers who have stayed for extended periods.

**Analysis of Monthly Charges Distribution:**

- Monthly charges exhibit a similar right-skewed distribution, meaning a significant number of customers are paying lower charges.
- A high concentration of customers is seen at the lower end 20, indicating a basic service plan that is widely chosen.
- The distribution gradually spreads towards higher charges 100, showing that some customers opt for premium services.
- The KDE suggests a gradual increase in density beyond the initial peak, indicating that while most customers pay low fees, a substantial portion is distributed across various pricing tiers.

![image](https://github.com/user-attachments/assets/0babe12c-03c9-48ef-806f-2cfbacd25cf9)

- **Gender Distribution** --> Male and Female contributes equally
- **Internet Service Distribution** ---> Fiber Optic Internet Service is the most used service among customers followed by DSL
- **Contract Type Distribution** ---> Customers prefering Monthly Subscription over yearly Subscription


![image](https://github.com/user-attachments/assets/f72b5072-52c0-4a04-b45a-36c49eb5a26f)

**Monthly Charges & Churn:**

- Customers who churn (blue) generally have higher monthly charges compared to those who do not churn (red).
- The median monthly charge for churned customers is higher, suggesting cost might be a factor in churn.
- The interquartile range (IQR) is similar for both groups, indicating variability in charges.

**Tenure & Churn (Right Plot):**

- Customers who churn have significantly lower tenure, with most churned users having less than 20 months of tenure.
- Long-tenured customers (above 40-50 months) rarely churn, indicating customer loyalty increases over time.
- There are some outliers in the churned group, but they do not significantly impact the trend.


# Churn Analysis Summary:

- Contract Type: Month-to-month contracts have the highest churn, while yearly and two-year contracts show significantly lower churn, indicating that longer commitments reduce customer attrition.
- Internet Service: Fiber optic users exhibit higher churn than DSL and those without internet, possibly due to pricing or service issues.
- Payment Method: Customers using electronic checks have the highest churn, suggesting that automatic payments (bank transfers, credit cards) lead to better retention.
- Senior Citizens: Older customers (Senior Citizen = 1) have a higher churn rate proportionally compared to younger customers, indicating a potential demographic risk factor.






