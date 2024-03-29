# Mini-Project - Marks Adding

A brief description of what this project does and who it's for

1)We have given a CSV file in which we have given a Roll numbers and marks. 

2 )Same roll number have given marks a number of times in different rows.

3) In this project , we will add marks of same roll numbers , then get the total marks .

As shown below






![243881755-9be14aa0-eaa0-403a-9575-32771724f0e2 (1)](https://github.com/Prabh-84/Mini-project-2---Marks-adding/assets/164873550/3182c948-4eeb-4075-853c-92e1def8ec75)

## Steps 

Step 1 - Extract a CSV file into a Pandas Dataframe

Step 2 - Group the Data frame by the key column by use of groupby() and using sum() to add same key values

Step 3 - Export the Dataframe into CSV file

Complete code



# Usage

1)import pandas as pd


### Read the Excel file
df = pd.read_csv('/content/Mini Project - Marks Adding.csv')

### Print the DataFrame
print(df)

### 2) Group the DataFrame by the 'Roll Num' column and sum the 'Marks' column
df_sum= df.groupby('Roll Num')['Marks'].sum()

### Print the summed DataFrame
print(df_sum)

### 3)export the dataframe to a CSV file
df_sum.to_csv('Total marks after adding.csv')


    
