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

## 📈 Visualization
A line chart was generated to show how Big Mac prices have changed over time in the U.S.

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

## 🚀 How to Reproduce
### 🔧 Requirements
- Python 3.x
- Pandas
- Matplotlib

### 📝 Steps
1. Load the dataset into a Pandas DataFrame.
2. Perform the preprocessing steps outlined above.
3. Use Matplotlib to generate the line chart.

## 📢 Conclusion
This analysis provides insight into the historical price trends of Big Macs in the U.S., highlighting inflation through the price of a hamburger.

---
### 🖋 Author: Your Name
