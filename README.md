# Home-Credit-Default-Risk-Detection
Home Credit Default Risk mission is to promote financial inclusion by providing a positive and safe borrowing experience for the unbanked population. To achieve this goal, Home Credit makes use of alternative data, including telco and transactional information, to predict their clients' repayment abilities. The project aims to address the issue faced by individuals who have weak or non-existent credit records, making it challenging for them to obtain loans. So, in this project, we predict the repayment abilities of financially underserved populations and provide loans to those who can repay, while avoiding those who cannot.

# Data Description:
Data is taken from a Kaggle project named Home Credit Default Risk. Home Credit strives to broaden financial inclusion for the unbanked population by providing a positive and safe borrowing experience. The dataset consists of 7 tables and one metadata file consisting of the column’s description of the tables. Of these 7, the table “application_{train test}” is considered the main table as it includes the applications, we are trying to make the predictions for. In addition to this main table, there are six sub-tables that relate hierarchically to this main table.

Here is the description of all the files included in the dataset:
#   	application_{train test}.csv:
o   This is the main table, broken into two files for Train (with TARGET) and Test (without TARGET).
o   Static data for all applications. One row represents one loan in our data sample.
#   	bureau.csv:
o   All client's previous credits provided by other financial institutions were reported to the Credit Bureau (for clients who have a loan in our sample).
o   For every loan in our sample, there are as many rows as the number of credits the client had in the Credit Bureau before the application date. 
#   	bureau_balance.csv:
 o   Monthly balances of previous credits in Credit Bureau.
o   This table has one row for each month of history of every previous credit reported to the Credit Bureau – i.e. the table has (#loans in sample * # of relative previous credits * # of months where we have some history observable for the previous credits) rows.
#  	POS_CASH_balance.csv:
o   Monthly balance snapshots of previous POS (point of sales) and cash loans that the applicant had with Home Credit.
o   This table has one row for each month of history of every previous credit in Home Credit (consumer credit and cash loans) related to loans in our sample – i.e. the table has (#loans in sample * # of relative previous credits * # of months in which we have some history observable for the previous credits) rows.
#   	credit_card_balance.csv:
o   Monthly balance snapshots of previous credit cards that the applicant has with Home Credit.
o   This table has one row for each month of history of every previous credit in Home Credit (consumer credit and cash loans) related to loans in our sample – i.e. the table has (#loans in sample * # of relative previous credit cards * # of months where we have some history observable for the previous credit card) rows.
#   	previous_application.csv:
o   All previous applications for Home Credit loans of clients who have loans in our sample.
o   There is one row for each previous application related to loans in our data sample.
#   	installments_payments.csv:
o   Repayment history for the previously disbursed credits in Home Credit related to the loans in our sample.
o   There is a) one row for every payment that was made plus b) one row each for a missed payment.
o   One row is equivalent to one payment of one installment OR one installment corresponding to one payment of one previous Home Credit related to loans in our sample.




 



