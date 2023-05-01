# Health-Insurance-Cross-Sell-Prediction

# Problem Statement

Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.

For example, you may pay a premium of Rs. 5000 each year for a health insurance cover of Rs. 200,000/- so that if, God forbid, you fall ill and need to be hospitalised in that year, the insurance provider company will bear the cost of hospitalisation etc. for upto Rs. 200,000. Now if you are wondering how can company bear such high hospitalisation cost when it charges a premium of only Rs. 5000/-, that is where the concept of probabilities comes in picture. For example, like you, there may be 100 customers who would be paying a premium of Rs. 5000 every year, but only a few of them (say 2-3) would get hospitalised that year and not everyone. This way everyone shares the risk of everyone else.

Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

# Our Goal -

# Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

 # Attribute Information-
 
 1. id : Unique ID for the customer

2. Gender : Gender of the customer

3. Age : Age of the customer

4. Driving_License : 0 - Customer does not have DL, 1 - Customer already has DL

5. Region_Code : Unique code for the region of the customer

6. Previously_Insured : 1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance

7. Vehicle_Age : Age of the Vehicle

8. Vehicle_Damage : 1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.

9. Annual_Premium : The amount customer needs to pay as premium in the year

10. PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.

11. Vintage : Number of Days, Customer has been associated with the company

12. Response : 1 : Customer is interested, 0 : Customer is not interested

# Summary

The health insurance cross sell prediction dataset is a dataset that contains information about customers of an insurance company and whether they have purchased a particular insurance product. The goal is to build a predictive model that can accurately identify which customers are likely to purchase the product.

In this project, we analyzed the dataset and performed exploratory data analysis to understand the patterns and relationships in the data. We then preprocessed the data and trained four different classification models:

Logistic Regression, KNN, Random Forest, and XGBoost.

# Conclusion 

1.Starting from loading our dataset, we initially checked for null values and duplicates. There were no null values and duplicates so treatment of such was not required.

Through Exploratory Data Analysis,

2.we observed that customers belonging to youngAge are more interested in vehicle response.while Young people below 30 are not interested in vehicle insurance.

3.We observed that customers having vehicles older than 2 years are more likely to be interested in vehicle insurance. Similarly, customers having damaged vehicles are more likely to be interested in vehicle insurance.

4.The variable such as Age, Previously_insured,Annual_premium are more afecting the target variable.

5.For Feature Selection, we applied the Mutual Information technique. Here we observed that Previously_Insured is the most important feature and has the highest impact on the dependent feature and there is no correlation between the two.

6.We observed that the target variable was highly imbalanced.So this issue was solved by using Random Over Sample resampling technique.

7.we applied feature scaling techniques to normalize our data to bring all features on the same scale and make it easier to process by ML algorithms.

8.Further, we applied Machine Learning Algorithms to determine whether a customer would be interested in Vehicle Insurance.

For the logistic regression we got an accuracy of 78% for the

KNN classifier we got an accuracy of 85% for

XGBClassifier we got the aacuracy of 81% whereas,.

# We are getting the highest accuracy of about 94% and ROC_AUC score of 94% with Random forest
So, From this we can conclude that random forest is the best models as compare to the other models.

