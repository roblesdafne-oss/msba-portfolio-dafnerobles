{\rtf1\ansi\ansicpg1252\cocoartf2867
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fmodern\fcharset0 CourierNewPSMT;\f1\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;}
\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\deftab720
\pard\pardeftab720\li1920\fi-480\sl306\partightenfactor0

\f0\fs26\fsmilli13333 \cf2 \expnd0\expndtw0\kerning0
## 
\f1\fs32 What 3\'965 source tables would you expect a real company to use for customer churn? For each source, what does one row represent, for example one customer, one month, one event\
1. Account information - One line per account \
2. Billing transactions - One line per billing transaction (payment, reimbursement)\
3. Services (One line per service per customer)\
4. Support transactions (one line per customer interaction with support)\
5. Customer information - one line per customer (an account might have more than 1 user)\
\

\f0\fs26\fsmilli13333 ## 
\f1\fs32 What keys would you use to connect the data, for example customer_id, account_id, date, etc?\
Account_id, customer_id, date, service_id, billing_id, supportcase_id\
\
\pard\pardeftab720\li1920\fi-480\sl306\sa213\partightenfactor0

\f0\fs26\fsmilli13333 \cf2 ## 
\f1\fs32 What are two risks and how would you reduce them? Examples of risks are duplicates, missing IDs, using information that only exists after churn happens, and definitions changing over time.\
Missing information: having locks on information that is needed and having rules to fill information if not needed. For example if total_billed = 0 but tenure_mo = 0 then this is a true scenario, but if tenure_mo is more than 1 month flag these lines to investigate.\
Duplicate values: have a cyclic review of duplicate values and delete the ones that have exact same time stamp\
Empty lines: weekly clean up of lines that are empty\
Definitions housekeeping: keep an updated dictionary with clear business rules and review actions on data when something changes. \
\
}