{\rtf1\ansi\ansicpg1252\cocoartf2867
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;\f1\fswiss\fcharset0 ArialMT;}
{\colortbl;\red255\green255\blue255;\red255\green255\blue255;}
{\*\expandedcolortbl;;\cssrgb\c100000\c100000\c100000;}
\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 ## BUSINESS PROBLEM\
\
Customer churn is a major challenge for TruSource, the objective of this project is to:\
1. Predict which customers are likely to leave\
2. Retain current customers\
3. Build a model that predicts not only which customers will churn but also that can give us insights on what are the main reasons a customer might churn\
4. Create a strategy around the most important insights\
\
## KEY RESULTS \
1. After testing several methods we end up choosing XGBoost which uses a gradient boosted decision trees supervised learning method. This method was chosen as it gave us the best ROC-AUC and because it could manage the data imbalance in our dataset. \
2. Identify important variables: Contract term, referrals, Tenure Months, Monthly Fee and Marriage status + dependent status are the most important features identified by our model\
3. We are able to identify a segment of the population that churns the most: no dependents + early tenure + month to month contract term and provide recommendations around these results. \
\
##HOW TO RUN THE CODE\
In order to keep the code a bit cleaner we have 2 files: one testing XG Boost and the other testing Random Forest. \
1. Make sure to have the data set file called ***retentiondata_case.csv*** in the same file as the .ipynb files\
2. Open any of the ipynb files depending on the model you want to test in your preferred python editor that can read .ipynb files\
3. Run the code step by step, there will be an explanation of what each step is doing\
4. First steps will be around data cleaning and feature engineering \
\
##RISK OR LIMITATIONS\
In this model we are using a data set from un specific quarter where 73% of the data is not a churn customer while the rest is. We are also dealing with specific data inconsistencies in this file which might be different in others, so make sure to check for missing data and what is the best way to deal with it. 
\f1\fs38\fsmilli19093 \cf2 \expnd0\expndtw0\kerning0
\outl0\strokewidth0 \strokec2 \
}