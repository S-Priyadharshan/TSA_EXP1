# Ex.No: 01A PLOT A TIME SERIES DATA
###  Name: Priyadharshan S
###  Date: 19-08-2025

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:

```python
import pandas as pd
import matplotlib.pyplot as plt

data=pd.read_csv("/content/silver prices.csv")

data.head()

data.tail()

data["Date"]=pd.to_datetime(data["Date"])

plt.plot(data['Date'], data['Close/Last'], label='Time Series Data')
plt.xlabel('Date')
plt.ylabel('Price')
plt.title('Time Series Plot')
plt.legend()
plt.show(block=False)
plt.show()

data['Volume'].mean()

```

# OUTPUT:

<img width="541" height="243" alt="image" src="https://github.com/user-attachments/assets/9ff8da88-7a75-4008-af82-95d73efc2dfd" />

<img width="733" height="562" alt="image" src="https://github.com/user-attachments/assets/e08b462d-842d-40e9-b529-d4e2d189ac52" />

<img width="287" height="49" alt="image" src="https://github.com/user-attachments/assets/cc59a846-04ef-4ba3-91ca-115da36f85c2" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
