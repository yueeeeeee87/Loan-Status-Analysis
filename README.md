# Loan_Status_Analysis
The main goal of this project is to identify and predict the loan status of lenders.   
To figure out whether the dataset has time series characteristic, two validation methods (K-fold, TimeSplit) are also used.  
In this project, RandomForest is the main model to predict and analyze the loan status.  


## Data Description
The Dataset for model training includes 916567 rows and 10 columns from 2007 to 2017. 

### The Y variable in the project is:  

* loan_stat -> Including 3 status, Fully Paid, Charged Off, and Default


#### There are 10 X variables using in this project:
  
* annual_inc -> Annual income  
* emp_length -> Employment length  
* dti ->  The debt-to-income ratio of the borrower  
* delinq_2yrs -> The number of times the borrower had been 30+ days past due on a payment in the past 2 years  
* term -> Borrowing term  
* grade -> History credit grading  
* inq_last_6mths -> The borrower’s number of inquiries by creditors in the last 6 months  
* purpose -> Purpose for borrowing  

## Dummy vairables transformation 

#### loan_stat  
Fully_paid -> 0  
Defult, Charged-Off -> 1  
#### Grade  
A, B, C, D, E, F, D -> 1, 2, 3, 4, 5, 6, 7  
#### Purpose  
debt_consolidation -> 1  
Other -> 0  
