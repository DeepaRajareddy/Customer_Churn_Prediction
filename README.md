# Customer_Churn_Prediction

Telco is a provider of telecommunication services. Like many enterprises, Telco is finding mechanisms to prevent customer churn. For a telecommunication service provider like Telco, the cost of acquiring a new customer is a lot greater than that of retaining a current customer. Thus, the importance of developing an effective customer retention program to maintain the existing clientele. The first task is to build a classification model to predict whether a customer will cancel the service or not. The second task is to analyze the most important factors that lead to customer churn. Last, provide suggestions to prevent churn. 

### Data available: This project will use the Telco Customer Churn dataset which was last updated on February 23rd, 2018. In this data set, each row represents a customer and each column represents customer’s attributes. 

The attributes include four big categories:
● Customers who left within the last month – the column is called Churn. 
● Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies 
● Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges 
● Demographic info about customers – gender, age range, and if they have partners and dependents 

### Attributes: 
customerID: the id of the customer 
Gender: whether the customer is a male or female 
SeniorCitizen: Whether the customer is a senior citizen or not 
Partner: Whether the customer has a partner or not 
Dependents: Whether the customer has dependents or not 
Tenure: Number of months the customer has stayed with the company 
Phone Service: Whether the customer has a phone service or not 
Multiple lines: Whether the customer has multiple lines or not 
InternetService: Customer’s internet service provider (DSL, Fiber Optic, No) 
OnlineSecurity: Whether the customer has online security or not 
OnlineBackup: Whether the customer has online backup or not 
DeviceProtection: Whether the customer has device protection or not 
TechSupport: Whether the customer has tech contacted tech support or not 
Contract: type of contract (i.e., length) 
PaymentMethod: payment method 
MonthlyCharge: amount billed 
TotalCharges: lifetime amount billed 
Churn: whether the customer left 

1) Importing the “telco_train.csv” file into the dataframe df and print: 
a. the attribute names
b. Number of rows and columns 

2) Are there any null (i.e., missing) values in the target variable? How many null values were there? 
3) Droped NULL (na) values that I found and How many instances for each of the levels of the target variable (i.e., churn) are there left?
4) What is the mean and median value for tenure?
5) How are customers distributed (i.e., frequency) across gender? 
6) What’s the distribution of the tenure of customers? 
7) Making sure the data type for Churn are set as Category. Checking whether the variable churn as category type?
8) What is the ratio of average of Total Charges for Male Senior Citizens to that of Female Senior citizens? 
9) Creating a box plot with the Monthly Charges based on the type of contract the customers have. Concluding comparing the month-to-month compared to the two-year contract?

### Decision Tree model (default attributes)
 10) Running the following line of code in our notebook (copy and paste it). What does it do? 
df = pd.get_dummies(data=df, drop_first = True, columns=['gender', 'InternetService', 'PaymentMethod','Contract']) 

11) Creating a variable predictors with all the predictors (except for customerID and target variable). Creating a variable outcome with the target variable 
12) Using the train_test_split function from scikit-learn to split the data into train/test using a 70%/30% split, respectively. Setting the parameter random_state = 1. Making sure we import the necessary libraries from scikit-learn. Instantiate a Decision Tree model dt with the following parameters (max_depth = 4; random_state = 1) and fit the training data. Making sure we import the necessary libraries from scikit-learn. 
13) What is the precision and recall on the test data? 
14) What is the f-measure on the test data? 
15) What is the most important variable? [making sure we show how you determined it]

### Logistic Regression model (default attributes)
16) Using the data from (10) and (11), instantiate a Logistic Regression model lr with the following parameters (random_state = 1, solver = 'liblinear' ) and fit the training data. 
17) What is the precision and recall on the test data? 
18) What is the f-measure on the test data?
19) Which model (decision tree or logistic regression) performs better?

