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
```
import pandas as pd
df = pd.read_csv("Data_set.csv")
df.head(10)
df.tail()
df.info()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['show_name'].mode(0))
df.head()
df['rating']=df['rating'].fillna(df['rating'].mean())
df.info()
df['rating']=df['rating'].fillna(df['rating'].mean())
df.head(20)
```
# OUPUT
![f1](https://user-images.githubusercontent.com/94219582/159970189-45e2b104-f0ef-479b-9a51-9d352a3a6565.PNG)
![f2](https://user-images.githubusercontent.com/94219582/159970220-ad5b07a5-0138-47d5-870a-c4bd644e11a5.PNG)
![f3](https://user-images.githubusercontent.com/94219582/159970242-b1222cf7-6d3d-41e4-9f24-fc7f91244af8.PNG)
![f4](https://user-images.githubusercontent.com/94219582/159970286-259c5806-cfb3-4efe-8711-b8dc124a2e80.PNG)
![f5](https://user-images.githubusercontent.com/94219582/159970320-0897470e-761b-4136-b2ed-21cb047ba4b2.PNG)
![f6](https://user-images.githubusercontent.com/94219582/159970370-a38a96cb-5c87-4278-b22d-e668168ae9d9.PNG)

