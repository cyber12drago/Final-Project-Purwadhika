# Final Project Purwadhika - Bank Marketing

by:
1. Muhammad Naufal Refadi
2. Intan Tjendera

This Repository Contains:
- [Dataset](https://github.com/PurwadhikaDev/DataWarrior_JC_DS_FT_BSD_JKT_14_FinalProject/blob/main/bank-additional-full.csv)
- [Source Code](https://github.com/PurwadhikaDev/DataWarrior_JC_DS_FT_BSD_JKT_14_FinalProject/blob/main/Final_Project_Purwadhika_Bank_Marketing.ipynb)
- [Presentation](https://github.com/PurwadhikaDev/DataWarrior_JC_DS_FT_BSD_JKT_14_FinalProject/blob/main/Presentation/Final%20Project%20Bank%20Marketing%20Campaign.pptx)

Original Data Source: [https://www.kaggle.com/volodymyrgavrysh/bank-marketing-campaigns-dataset](https://www.kaggle.com/volodymyrgavrysh/bank-marketing-campaigns-dataset)

## Problem Statement
The following dataset shows a Portugal bank's marketing campaigns results in an attempt to evaluate the success of the bank's telemarketing. Conducted campaigns seem to be based mostly on direct phone calls, offering bank clients to place a term deposit. Term deposits allow banks to hold onto a deposit for a specific amount of time, letting banks invest in higher gain financial products in order to make a profit. Additionally, banks also hold a better chance to persuade term deposit clients into buying other products such as funds or insurance to further increase their revenues. The bank found a possible revenue decline problem upon investigation, where the root cause is that their clients are not depositing as frequently as before. Hence, the Portuguese bank would like to identify existing clients that have a higher chance to subscribe for a term deposit and focus marketing efforts on such clients.

A machine learning (ML) algorithm based on the following data can be utilized to help banks predict potential clients who are likely to place a deposit upon receiving the telemarketing campaign. Not only will this help the banks to have a more effective marketing effort by prioritizing target customers, but also aid in allocating funds and manpower appropriately to further minimize marketing costs. This may also give an insight to banks how effective direct phone call campaigns are, as compared to other sales channels; and vice versa.

This dataset will involve a supervised learning approach to a classification problem. We will look at accuracy, precision, recall, and f1-score to evaluate the goodness of the model, focusing on the recall portion as our end goal is to minimize the cost the bank spent on marketing.

The risks involved may include overestimation of target customer behavior despite having achieved all necessary aspects to be classified as 'a likely client', and vice versa

## Data Description
| Column Name | Description  | Type  |
| :---:   | :---:| :---: |
| age     | client's age | numeric |
| job   | type of job  | categorical |
| marital | marital status | categorical |
| education| last education | categorical |
| default  | has credit in default?  | categorical |
| housing  | has housing loan? | categorical |
| loan     | has personal loan?  | categorical |
| contact  | contact communication type| categorical |
| month     | last contact month of year | categorical |
| dayofweek | last contact day of the week | categorical |
| duration     | last contact duration, in seconds| numeric |
| campaign     | number of contacts performed during this campaign and for this client| numeric |
| pdays    | number of days that passed by after the client was last contacted from a previous campaign| numeric |
| previous     | number of contacts performed before this campaign and for this client| numeric |
| poutcome     | outcome of the previous marketing campaign| categorical |
| emp.var.rate | employment variation rate - quarterly indicator| numeric |
|cons.price.idx| consumer price index - monthly indicator|numeric|
|euribor3m| euribor 3 month rate - daily indicator|numeric|
|nr.employed|number of employees - quarterly indicator|numeric|
|y | has the client subscribed a term deposit?|numeric|

## Modeling
We use Random Forest because this model can be utilised to help the bank's call center to prioritise the call for potential clients and maximise the conversion rate - all while managing minimum cost on marketing.

#Evaluation
We have got 85% for recall score and AUC Score 0.75. Also by implementing the model, this can give about 2x more revenue to the bank.