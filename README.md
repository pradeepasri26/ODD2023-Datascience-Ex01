# Ex-01_DS_Data_Cleansing


## AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE 
# For Data_set
```
 import pandas as pd
 df=pd.read_csv("/content/Data_set .csv")
 df

 df.head(10)

 df.info()

 df.isnull()

 df.isnull().sum()

 df['show_name']=df['show_name'].fillna(df['aired_on'].mode()[0])
 df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
 df['original_network']=df['original_network'].fillna(df['aired_on'].mode()[0])
 df.head()

 df['rating']=df['rating'].fillna(df['rating'].mean())
 df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean
 df.head()

 df['watchers']=df['watchers'].fillna(df['watchers'].median())
 df.head()

 df.info()

 df.isnull().sum()
```

# For loan_set
```
 import pandas as pd
 df=pd.read_csv("/content/Loan_Data.csv")
 print(df)

 df.head(5)

 df.info()

 df.isnull()

 df.isnull().sum()

 df['Loan_ID']=df['Loan_ID'].fillna(df['Education'].mode()[0])
 df['Education']=df['Education'].fillna(df['Education'].mode()[0])
 df['Married']=df['Married'].fillna(df['Education'].mode()[0])
 df.head()

 df['ApplicantIncome']=df['ApplicantIncome'].fillna(df['ApplicantIncome'].mean())
 df['LoanAmount']=df['LoanAmount'].fillna(df['LoanAmount'].mean())
 df.head()

 df.head()

 df['Loan_Amount_Term']=df['Loan_Amount_Term'].fillna(df['Loan_Amount_Term'].median())
 df.head()

 df.info()

 df.isnull().sum()
```
# OUTPUT
# For Data_Set
# DATA
![Screenshot (28)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/19b27941-bb32-4d1f-ac7e-88f22627c2f4)

![Screenshot (29)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/e0066b7c-fde8-41c4-95fd-3cfa91bbc487)

![Screenshot (31)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/b771523b-8783-4fbb-80c1-7612d4b22cd9)

![Screenshot (33)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/1b8dd877-b20d-4e34-8d1f-77b9cfe3b747)

![Screenshot (72)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/c963baec-059f-4663-b6a0-188a3caf6617)

# NON NULL BEOFRE
![Screenshot (39)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/85eed589-ae9c-4c95-81f3-64ea67ca48ea)

![Screenshot (40)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/6fc698f6-97d2-4114-8827-3d653fddac5c)

![Screenshot (41)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/f6ef2000-21a5-433a-a1c8-5b33fe432542)

# MODE
![Screenshot (45)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/16b83227-2a98-453b-b260-3febc9ba561f)

# MEAN
![Screenshot (46)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/e74744fb-a440-458a-bc73-86c94e4b30b3)

# MEDIAN
![Screenshot (47)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/3f2a24c9-7f89-4469-942d-2737199a726e)

# NON NULL AFTER
![Screenshot (50)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/2e0e2667-758b-4670-92ee-2e0e5e7188c6)

![Screenshot (51)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/cc99c0d4-02ec-4ba2-a524-8a924e2aa43b)

# For loan_data
# DATA
![Screenshot (57)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/377cd686-c252-421f-889f-dd46cb609aa7)

![Screenshot (58)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/22a33740-dd9d-497b-b767-694dcef822f1)

# NON NULL BEFORE
![Screenshot (59)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/7b752ee1-08c6-44b9-82ce-093556262975)

![Screenshot (60)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/5a72eac1-94d7-4d2c-b1f9-f7406f1ecc43)

![Screenshot (61)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/e3e91cf4-a689-4aa6-aa9b-36bfe10b9d6d)

# MODE
![Screenshot (67)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/bf787221-16f7-4e45-bd3f-b3813bff24dd)

# MEAN
![Screenshot (68)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/3de43e23-0f1e-4fbe-93b0-360088bc07de)

# MEDIAN
![Screenshot (69)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/d1ca9d3a-435e-4a19-8e18-755de9132730)

# NON NULL AFTER
![Screenshot (70)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/519393f9-0ea5-4dd7-b1c7-9f17c24cde55)

![Screenshot (71)](https://github.com/pradeepasri26/ODD2023-Datascience-Ex01/assets/131433142/4029e170-2c06-40d3-b13e-b866ea448f75)

## RESULT
Thus, the given data is read, cleansed and the cleaned data is saved into the file.

