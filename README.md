# Credit-Card-Default-Fraud-Prediction
In this project, I will be implementing classification algorithms like Support Vector Machines, Decision Trees and Boosting Algorithm on Credit card payment default dataset. I will use k fold cross validation and parameter tuning to identify the best classification algorithm. I will be implementing Artificial Neural Network and K Nearest Neighbors algorithms as well to see if they improve the prediction accuracy.   
The dataset source of Credit card default dataset:    
https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset   

## About Credit Card Default Dataset     
Credit card fraud causes a huge amount of bad debt for banks. Detecting fraud such as credit card payment default in advance can save financial institutions from significant losses. Predictive analytics is extensively used by financial institutions to identify fraud instances and take action to avoid or mitigate such situation. I’ve chosen this dataset as it would help me explore how machine learning algorithms can be used for fraud prevention.       
The dataset contains information on default payments, demographic factors, credit data, history of payment, and bill statements of credit card clients in Taiwan from April 2005 to September 2005.It has 30,000 observations and 25 attributes. The target variable is whether credit card user will default or not.     

## Attributes:   
•	ID: ID of each client   
•	LIMIT_BAL: Amount of given credit in NT dollars     
•	SEX: Gender (1=male, 2=female)    
•	EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)   
•	MARRIAGE: Marital status (1=married, 2=single, 3=others)  
•	AGE: Age in years    
•	PAY_0: Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, … 8=payment delay for eight months, 9=payment delay for nine months and above)  
•	PAY_2: Repayment status in August, 2005 (scale same as above)  
•	PAY_3: Repayment status in July, 2005 (scale same as above)   
•	PAY_4: Repayment status in June, 2005 (scale same as above)  
•	PAY_5: Repayment status in May, 2005 (scale same as above)   
•	PAY_6: Repayment status in April, 2005 (scale same as above)    
•	BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)   
•	BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)   
•	BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)   
•	BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)  
•	BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)   
•	BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)   
•	PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)   
•	PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)   
•	PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)   
•	PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)   
•	PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)   
•	PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)    
•	default. payment. next. month: Default payment (1=yes, 0=no)      

For detailed analysis on classification algorithms, refer to Credit Card Default Fraud Classification.pdf.The code for the analysis is avaiable in Credit Card Default Prediction Code 1.     
For detailed analysis on Artificial Neural Network model, refer to Credit Card Default(ANN).pdf.The code for the analysis is avaiable in Credit Card Default Prediction Code 2.     
## Conclusion   
After performing all the three classification algorithms,Adaboost tree provides best accuracy (~82%).However, the best model for the Credit Card Default dataset would be Artificial Neural Network model with test accuracy of 82% and highest precision score of 0.37.Our primary goal is to identify defaults.As misclassifying default as not default will have a higher negative impact than misclassifying a non default as default.Hence we want high precision score.      
