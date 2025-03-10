# Big Mac Price Analysis (United States)

## 📌 Overview
This project analyzes the historical Big Mac prices in the United States using a dataset containing global Big Mac prices. The goal is to track the price progression over the years and visualize the trend.

## 📊 Dataset
The dataset contains the following columns:
- **`date`**: Date of Big Mac price recording.
- **`currency_code`**: Three-letter currency code.
- **`country`**: Name of the country.
- **`local_price`**: Price of a Big Mac in local currency.
- **`dollar_ex`**: Exchange rate to USD.
- **`dollar_price`**: Price of a Big Mac in USD.

## 🛠 Steps Taken

### 1️⃣ Data Preprocessing
✔ Renamed the `name` column to `country`.  
✔ Filtered the dataset to include only records for the United States.  
✔ Extracted the `year` from the `date` column.  
✔ Removed unnecessary columns: `date`, `currency_code`, `dollar_ex`, and `dollar_price`.  
✔ Reset the index and rearranged columns to place `year` first.  

### 2️⃣ Handling Duplicate Years
✔ Identified duplicate years where multiple Big Mac prices existed.  
✔ Averaged the `local_price` for duplicate years.  
✔ Rounded the values to two decimal places.  

### 3️⃣ Data Visualization
✔ Created a line chart to visualize the progression of Big Mac prices over the years in the United States. 
✔ Create a heat map to visualize pricing evolution in Europe 

## 📈 Visualization
A line chart was generated to show how Big Mac prices have changed over time in the U.S.
A heatmap was generated to illustrate how Big Mac prices have changed over time in different EU countries. The color intensity indicates variations in the dollar price across years.

```python
import matplotlib.pyplot as plt
plt.figure(figsize=(10, 5))
plt.plot(df_us_avg["year"], df_us_avg["local_price"], marker="o", linestyle="-", color="b")
plt.xlabel("Year")
plt.ylabel("Average Big Mac Price (USD)")
plt.title("Big Mac Price Progression in the United States")
plt.grid(True)
plt.show()
```
```python
plt.figure(figsize=(12, 8))
sns.heatmap(heatmap_data, cmap="coolwarm", annot=True, fmt=".2f", linewidths=0.5)
plt.title("Big Mac Prices Over Time by Country (USD)")
plt.xlabel("Year")
plt.ylabel("Country")
plt.xticks(rotation=45)
plt.yticks(rotation=0)
plt.show()
```


## How to Reproduce
### Requirements
- Python 3.x
- Pandas
- Matplotlib
- Seaborn

### Steps
1. Load the dataset into a Pandas DataFrame.
2. Perform the preprocessing steps outlined above.
3. Use Matplotlib to generate the line chart and heat map.

## Conclusion
This analysis provides insight into the historical price trends of Big Macs in the U.S. and Europe, highlighting inflation through the price of a hamburger.

## Future Plans
Use these new data sets to create more visuals using Tableau

---
### 🖋 Author: Kyle Jones
|Website     |  Handle   | 
|---------|-----------------|
|Github| https://github.com/KJones-Git        |
|Tableau |   https://public.tableau.com/app/profile/kyle.jones8049/vizzes      |
|LinkedIn |  https://www.linkedin.com/in/kylelaurencejones/      |
