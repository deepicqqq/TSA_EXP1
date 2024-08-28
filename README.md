## NAME:DEEPIKA P
## REG NO:212223240024

# Ex.No: 01A PLOT A TIME SERIES DATA

# AIM:
To Develop a python program to Plot a time series data of daily delhi climate test.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Plot the data according to need and can be altered monthly, or yearly.
4. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv('dailydelhiclimatetest.csv', parse_dates=['date'])
data.set_index('date', inplace=True)
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['meantemp'], label='Mean Temperature')
plt.plot(data.index, data['humidity'], label='Humidity')
plt.plot(data.index, data['wind_speed'], label='Wind Speed')
plt.plot(data.index, data['meanpressure'], label='Mean Pressure')
plt.xlabel('Date')
plt.ylabel('Values')
plt.title('Delhi Climate Data')
plt.legend()
plt.show()
```
# OUTPUT:

![Screenshot 2024-08-24 083428](https://github.com/user-attachments/assets/67928fcc-0910-4d2c-af7a-5155689a6d33)

# RESULT:
Thus the given python program executed in successfully.
