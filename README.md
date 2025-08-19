# Ex.No: 01A PLOT A TIME SERIES DATA
# Developed By : Vedagiri Indu Sree
###  Date: 19/08/2025

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
```
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
data = pd.read_csv("rainfall (2).csv")

# Convert the 'Date' column to datetime
data['date'] = pd.to_datetime(data['date'])

# Plotting the 'Price' column over time
plt.figure(figsize=(10,6))
plt.plot(data['date'], data['rainfall'], label='rainfall', color='silver')

# Adding title and labels
plt.title('Daily Rainfall')
plt.xlabel('Date')
plt.ylabel('Rainfall rate')

# Displaying the plot
plt.legend()
plt.grid(True)
plt.show()
```

# OUTPUT:
<img width="1155" height="711" alt="image" src="https://github.com/user-attachments/assets/4dfc5bb0-1b60-4056-b1f9-5de1ea24bb40" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
