## Step-by-Step Guide to Data Visualization with Matplotlib

### Introduction

This guide provides a step-by-step walkthrough of creating various graphical visuals using Python's Matplotlib library. We will cover the plotting of Line Graphs, Bar Graphs, Histograms, and Pie Charts, using two datasets: Gas Prices and FIFA Player Data. The goal is to demonstrate how to import, manipulate, and visualize data effectively.

### Prerequisites

- Basic knowledge of Python programming
- Familiarity with Jupyter Notebook
- Installed Python libraries: Pandas, NumPy, and Matplotlib

### Step 1: Importing the Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
```

### Step 2: Importing the Datasets

#### Gas Prices Dataset

```python
gas_data_url = 'https://github.com/KeithGalli/matplotlib_tutorial/blob/master/gas_prices.csv'
gas_data = pd.read_csv(gas_data_url)
```

#### FIFA Player Dataset

```python
fifa_data_url = 'https://github.com/KeithGalli/matplotlib_tutorial/blob/master/fifa_data.csv'
fifa_data = pd.read_csv(fifa_data_url)
```

### Step 3: Exploring the Datasets

#### Gas Prices Dataset

```python
print(gas_data.head())
```

#### FIFA Player Dataset

```python
print(fifa_data.head())
```

### Step 4: Plotting Line Graphs

#### Gas Prices Over Years

```python
plt.plot(gas_data['Year'], gas_data['USA'], label='USA')
plt.plot(gas_data['Year'], gas_data['Canada'], label='Canada')
plt.plot(gas_data['Year'], gas_data['South Korea'], label='South Korea')
plt.plot(gas_data['Year'], gas_data['Australia'], label='Australia')
plt.xlabel('Year')
plt.ylabel('Price in USD')
plt.title('Gas Prices of Countries over Years')
plt.legend()
plt.show()
```

### Step 5: Plotting Bar Graphs

#### Player Distribution in FIFA 2018

```python
plt.bar(fifa_data['Overall'], fifa_data['Name'])
plt.xlabel('Skill Level')
plt.ylabel('Number of Players')
plt.title('Distribution of Player Skills in FIFA 2018')
plt.show()
```

### Step 6: Plotting Histograms

#### Skill Level Distribution in FIFA 2018

```python
plt.hist(fifa_data['Overall'])
plt.xlabel('Skill Level')
plt.ylabel('Number of Players')
plt.title('Distribution of Player Skills in FIFA 2018')
plt.show()
```

### Step 7: Plotting Pie Charts

#### Foot Preference in FIFA Match

```python
foot_counts = fifa_data['Preferred Foot'].value_counts()
plt.pie(foot_counts, labels=foot_counts.index, autopct='%1.2f%%')
plt.title('Foot Preference in FIFA Match')
plt.show()
```

### Final Project Insights

- Gas Prices: South Korea has the highest gas prices, followed by Australia, Canada, and the USA. There is a significant rise in gas prices after 2002.
- FIFA Player Data: The majority of players have skill levels ranging from 60 to 70. Approximately 76.81% of players prefer using their right foot during matches.

By following this guide, you can create informative and visually appealing graphs using Matplotlib, enabling you to gain insights from your datasets.
