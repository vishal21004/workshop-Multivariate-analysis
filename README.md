# workshop-Multivariate-analysis

# Aim:
To Perform Bivariate/Multivariate Analysis

# Algorithm:
1.Read the given data

2.Get information from the data 

3.Perform the Bivariate/Multivariate Analysis

4.Save the clean data to File

# Program:

```
Developed by:VISHAL M.A
Reg no: 212222230177
```
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_excel("flight.xlsx")
df
df.info()
df.describe()

sns.scatterplot(df['Price'],df['Source'],df['Destination'])
sns.scatterplot(df['Source'],df['Destination'],df['Total_Stops'])
sns.barplot(df['Source'],df['Price'],df['Destination'])
sns.barplot(df['Price'],df['Airline'],df['Source'])
sns.barplot(df['Price'],df['Source'])

df['Airline'].value_counts()
df['Route'].value_counts()
```

# output:
## dataset:
![image](https://user-images.githubusercontent.com/94154683/195608813-4107feb9-8a82-43fc-b232-84e3de95fd80.png)
## df.info
![image](https://user-images.githubusercontent.com/94154683/195609070-f54c73fa-df35-4d89-bc08-9ab7d9b24483.png)
## df.describe
![image](https://user-images.githubusercontent.com/94154683/195609225-8fe8e354-a321-4684-95ef-8104690c190b.png)
## scatterplot:
![image](https://user-images.githubusercontent.com/94154683/195609362-c876600d-e4bc-4517-9e52-f89fd4dc3c60.png)

![image](https://user-images.githubusercontent.com/94154683/195609559-b9134162-1cb7-4ec5-8a33-095e91b33da7.png)

![image](https://user-images.githubusercontent.com/94154683/195609650-c73294ef-bd9f-4842-ad66-216c109ee280.png)

![image](https://user-images.githubusercontent.com/94154683/195609839-b0095918-e8ca-4e16-941f-fbdc9bdeee65.png)

![image](https://user-images.githubusercontent.com/94154683/195609916-397d22d8-b7e8-421a-890e-0fc1d84c3a26.png)



## Airlines value_count:
![image](https://user-images.githubusercontent.com/94154683/195610119-7ca31dcb-f550-415f-84de-b34d8ef816ef.png)
## Route value_count:
![image](https://user-images.githubusercontent.com/94154683/195610462-b613831e-35ef-49f7-b12e-154f1219a59c.png)

# Result:
Thus we applied Bivariate/Multivariate Analysis Successfully
