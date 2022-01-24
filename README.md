# **Cryptocurrency Arbitrage Application**
This program is to use Pandas to develop a *Python* application that will perform calculations to determine Cryptocurrency arbitrage opportunities using Bitstamp and Coinbase. To perform this calculations, data is provided in the *bitstamp.csv* and *coinbase.csv* files in the Resources folder.

User can select specific periods in a month such as January 16th, February 24th, March 26 of 2018 for Timseries Analysis. Once these parameters are selected, the application performs calculations for pricing of Bitcoin on both coinbase and bitstamp exchange and calculates any arbitrage opportunities. Box and Plot charts are also utilized as visuals to better understand the data from the calculations.  

---
## Technologies
This application is developed on the *Python 3.7.11 version* 
Jupyter Lab Notebook that is an open sourced, web based user interface for software design, coding, visualization and documentationis is used for running the program that incorporates the following required dependencies:

**Pandas**: To import functions needed to program appliation for financial analysis
**Pathlib**: To load and save files from and to paths
**%matplotlib**: To perform analyticals calculations

---
## Installation Guide
The following installation must be performed before running the program:

*Install pathlib*
*Install Jupyter Lab*
*Install Pandas*

## Usage
This section is an explanation of how to use this program: 

We begin with data Collection and Preparation:
In preparing the data collections needed to import and read the program we use the date files called, *Bitstamp.csv* and *Coinbase.csv*. To confirm our accuracy,we review the first 5 rows or the last 5 rows of the dataframe. Once this is done, the next step is to prepare and to clean the dataframes for statistical analysis. We are mainly using the "Close" columns which is the colum that has the closing price of Bitcoin on different exhcanges. In order to be able to execute the calculations in the *crypto_arbitrage.ipynb* we need to remove the dollar sign infront of the numbers. In addition, NaN values and any unknowns must also be removed and need to make sure the data type is set to 'float64'. 


The next step is to analyzing the Data and Calculating the Arbitrage Profitability:
To analyze the data, we select 'Timestamp' and 'Close' columns as the specific areas to focus on. The 'Close' column is analyzed, as it is the closing price for Bitcoin on each exchange. 
Then, review the 'Summary Statistics'using the *describe* function and then use the *plot* function to plot the data on charts for all dates. Here, both exchanges are plottted individually for Bitcoin prices; then, the plots are overlayed to determine if there are any difference in prices visually. 
Next, focus on specific dates, select the day to analyze. The dates I picked were 01/16/2018, 02/24/2018 and 03/26/2018. These three dates will be compared to each other to measure arbitrafe spread, spread returns, and profitability. 
To further look in to the analysis, we focus on profits per trade and calculate the trades that exceeded the 1% transaction cost. This will identify the net profit trading Bitcoin on Bitstamp and Coinbase exchanges. 
A verification of data and information is need to validate the accuracy. To review the program code results and check the accuracy, we use *describe* function to get a summary statisstics and afterwards using the *plot* function to plot box charts and line graphs as a visual to see the results more clearly. 


---
## Contributors
*Contributors*: Saina Azimi

*Email*: azimi.sainaa@gmail.com

*LinkedIn*: https://www.linkedin.com/in/azimi-saina/ 

---
## License
UC Berkeley

---
