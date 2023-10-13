# ODD2023-DataScience-Ex-03
## AIM:
To read the given data and perform the univariate analysis with different types of plots.

## EXPLANATION
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## ALGORITHM:
#### Step1: 
Read the given data.

#### Step2
Get the information about the data.

#### Step3
Remove the null values from the data.

#### Step4
Mention the datatypes from the data.

#### Step5
Count the values from the data.
## PROGRAM:
```
Developed By : JENISHA.J
Register Number : 212222230056
```
#### superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('/content/SuperStore (1).csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
#### employeesal.csv
```
import pandas as pd
df=pd.read_csv("/content/employeesal (1).csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
#### diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
## OUTPUT:
#### superstore.csv
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/023fa84b-8e58-44de-8f96-509ef8acc4f5)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/b3509fea-bff0-447d-b577-b0e533ec2511)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/fa0f28a6-d014-4bff-89b3-26ffa6c8baf4)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/2449c8ee-e1a2-4588-bb53-6c020c732b4d)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/fac88e9e-0b64-4411-a137-50aaeec077ee)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/c878b1cf-a3f8-46d5-842e-4342714557e6)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/3b0aa3b9-444f-490f-84e1-d12758aa5751)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/ba134c8c-cfb7-4cc8-9a2c-a1345a9319bb)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/b989ca48-f109-439f-b4f2-c043713c1f8b)

#### employeesal.csv
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/fa163c69-0445-446f-a1db-742183886545)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/0276d8ad-9109-4640-9a71-761bb2e01190)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/24a72c9a-575e-42ce-a884-22f43766cdda)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/72fd3986-8ea4-4c81-a32c-090743528560)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/69e7db3d-34eb-4fb1-9e93-503230753580)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/4f9d67e8-2e42-4195-9fd8-e347b47d876d)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/4e69c469-3e43-40c2-96df-46eac73f1cf2)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/ac861a96-d2d4-4825-b185-9aaaacfdc4d0)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/c914a24a-967c-4b5b-8f43-46336a8fe6fb)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/e81c4088-fd69-4bf2-b8a5-3badc7c562c6)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/d61cc1ee-de32-4c5e-b7ee-482763401025)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/3d1e6b59-8996-40eb-92b6-fdc1461bc23f)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/d768a98d-c763-4330-9863-257bb32c5df1)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/9a2eb633-f3ec-4823-af08-c16815e2a6e1)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/663938e8-1187-48ed-9371-160d8bfc3895)

#### diabetes.csv
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/d014bdb6-df24-413f-8ea6-7902a5ba8013)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/baeb7c6f-3ba6-4905-8b86-9245d67ba180)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/e249e336-ce10-4241-984b-9f31aae630fa)
![image](https://github.com/Jenishajustin/ODD2023-DataScience-Ex-03/assets/119405070/da1d0ab1-73bb-4e31-9f6f-828e1fe1f813)

## RESULT:
Hence the univariate analysis is verified.

