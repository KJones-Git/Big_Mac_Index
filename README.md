# Big_Mac_Index
Analyzing the global and domestic prices of the McDonald's Big Mac since the year 2000
Big Mac Price Analysis (United States)

Overview

This project analyzes the historical Big Mac prices in the United States using a dataset containing global Big Mac prices. The goal is to track the price progression over the years and visualize the trend.

Dataset

The dataset contains the following columns:

date: Date of Big Mac price recording.

currency_code: Three-letter currency code.

country: Name of the country.

local_price: Price of a Big Mac in local currency.

dollar_ex: Exchange rate to USD.

dollar_price: Price of a Big Mac in USD.

Steps Taken

Data Preprocessing

Renamed the name column to country.

Filtered the dataset to include only records for the United States.

Extracted the year from the date column.

Removed unnecessary columns: date, currency_code, dollar_ex, and dollar_price.

Reset the index and rearranged columns to place year first.

Handling Duplicate Years

Identified duplicate years where multiple Big Mac prices existed.

Averaged the local_price for duplicate years.

Rounded the values to two decimal places.

Data Visualization

Created a line chart to visualize the progression of Big Mac prices over the years in the United States.

Visualization

A line chart was generated to show how Big Mac prices have changed over time in the U.S.

How to Reproduce

Requirements

Python 3.x

Pandas

Matplotlib

Steps

Load the dataset into a Pandas DataFrame.

Perform the preprocessing steps outlined above.

Use Matplotlib to generate the line chart.

Conclusion

This analysis provides insight into the historical price trends of Big Macs in the U.S., highlighting inflation and other economic factors over time.
