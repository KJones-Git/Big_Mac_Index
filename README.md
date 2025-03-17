# Big Mac Price Analysis

## 📌 Project Overview  
This project analyzes the **historical Big Mac prices** in the **United States and Europe**, using a dataset containing global Big Mac prices. The goal is to **track the price progression over the years** and compare it against **inflation trends**.

Additionally, this analysis evaluates the **Big Mac Index (BMI)**—a well-known economic indicator used to measure **purchasing power parity (PPP)**—to determine whether it remains a **reliable metric for tracking inflation** in today’s economy.

## 🛠 Steps Taken

1. **Data Import & Integration**  
   - Imported **three different datasets**:  
     - **Big Mac prices** dataset  
     - **Inflation rates** dataset  
     - **Beef prices** dataset  
   - Formatted and cleaned each dataset to ensure consistency.  
   - Merged all three datasets into **one central dataset** for analysis.  

2. **Data Preprocessing**  
   - Checked for missing values and corrected inconsistencies.  
   - Standardized column names and data types.  
   - Ensured the datasets aligned properly by year for accurate comparisons.  

3. **Exploratory Data Analysis (EDA)**  
   - Visualized historical **Big Mac prices, inflation rates, and beef prices** over time.  
   - Analyzed trends and relationships between inflation and food prices.  
   - Identified any deviations between price trends and economic inflation.  

4. **Big Mac Index Evaluation**  
   - Calculated the **annual percent increase** in Big Mac prices.  
   - Compared these trends with official inflation rates.  
   - Assessed whether the **Big Mac Index (BMI)** remains a reliable economic indicator.  

5. **Findings & Conclusions**
   - The **Big Mac Index (BMI) was a reliable indicator** of inflation before **2005**, closely following general inflation trends.
   - After **2005**, the **Big Mac Index became less accurate**, as both **Big Mac prices and beef prices** began rising **more sharply than inflation**.
   - This suggests that **factors beyond general inflation**, such as **rising labor costs, supply chain disruptions, and commodity price volatility**, have increasingly influenced Big Mac pricing.
   - As a result, the **Big Mac Index may no longer be a strong standalone economic indicator** for inflation tracking, though it still provides insight into purchasing power differences globally.  



## 📈 Visualizations

**Big Mac Index**

This chart visualizes the trends in **Big Mac prices, beef prices, and inflation rates** over time.  
It highlights how **Big Mac and beef prices began rising more sharply than inflation after 2005**, making the **Big Mac Index less reliable as an inflation indicator**.


![image_alt](https://github.com/KJones-Git/Big_Mac_Index/blob/72e614d0761103771bc1344bb8b398d536dadf1e/big_mac_chart.png)

**EU Big Mac Prices**

A heatmap was generated to illustrate how Big Mac prices have changed over time in different EU countries. The color intensity indicates variations in the dollar price across years.

![image_alt](https://github.com/KJones-Git/Big_Mac_Index/blob/b4914afa85b569991d506e14efdae14bfa0bfd9b/EU_heatmap.png)


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

The analysis reveals that while the **Big Mac Index (BMI)** was a reliable economic indicator before **2005**, it has since diverged from inflation trends. **Big Mac prices and beef prices have risen more sharply than general inflation**, suggesting that other external factors such as **rising beef prices** have increasingly influenced pricing beyond simply inflation.

As a result, the **BMI may no longer be a strong standalone measure of inflation**, though it still provides insights into **purchasing power and economic trends** across different regions. This study underscores the importance of considering multiple economic factors when analyzing inflation and cost-of-living changes.


## Future Plans
Use these data sets to create more complex visuals in Tableau.

---
### 🖋 Author: Kyle Jones
|Website     |  Handle   | 
|---------|-----------------|
|Github| https://github.com/KJones-Git        |
|Tableau |   https://public.tableau.com/app/profile/kyle.jones8049/vizzes      |
|LinkedIn |  https://www.linkedin.com/in/kylelaurencejones/      |
