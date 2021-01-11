# VBA_StockMarketAnalysis
This VBA analyzed the daily total volume and yearly return on 12 stock tickers for years 2017 and 2018.

## Overview of Project
Our friend Steve liked a previous project we completed for him, which allowed him to compare the stock tickers he was watching for 2017 and 2018 with a few button clicks. That said, he now wants be able to watch the entire stock market the same way, so we had to refactor the code to make it work for thousands of stock tickers, not just the original 12.

### Primary Purpose
Therefore, we have two purposes for this macro we created. The primary purpose is to be able to analyze the daily total volume of various stock market tickers, as well as its overall return over the course of two years—2017 and 2018. At a quick glance, Steve can see which tickers performed well via formatting for easy recognition.

### Secondary Purpose
Secondly, we wanted to see if there was an advantage for refactoring the code to work for all tickers, not just 12. So, we included a timer to test the macro’s overall runtime speed. 

## Results
We compared 12 tickers over a two-year span (stock samples shown below)––one comparison for 2017 and another for 2018. 

![Tickers] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/tickers.png

The macro ran through all our data to first identify and uniquely analyze each ticker (identification steps shown here):

![Ticker_Identification] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/%7Bticker%20identification%7D.png

Then it delivered the ticker results, including the total volume and ROI for a birds’ eye view of the results (shown here):

![Ticker_Output] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/%7Bticker%20output%7D.png

### 2017 Results
Out of the 12 tickers we monitored, only one had a negative return on investment, or lost money, in 2017. It was TERP, with an ROI of -7.2%. All other stocks had a positive ROI, ranging from 8.9% to 199.4%. The highest performer was DQ (199.4%), followed closely by SEDG(184.5%).

![2017_Results] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/2017_results.png

### 2018 Results
2018 looked nearly opposite of 2017, with only two stocks having a positive ROI––ENPH(81.9%) and RUN(84.0%). Every other stock had a negative ROI, anywhere from -3.5% to -62.6%.

![2018_results] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/2018_results.png

### Overall Takeaways
Only two stocks performed positively both years––ENPH with a very promising average ROI of 170.5%, and RUN with an ROI of 44.75%.

### Execution Times of Original Script vs. Refactored Script
There was an 85% reduction in run time after refactoring the macro, making it run in less than 1/10 of a second afterward, as opposed to over 1/2 second prior.
#### 2017 Comparison
Before
![Original_2017_runtime] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/VBA_Challenge_OriginalScript_2017.png

After
![Refactor_2017_runtime] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/VBA_Challenge_2017.png

#### 2018 Comparison
Before
![Original_2018_runtime] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/VBA_Challenge_OriginalScript_2018.png

After
![Refactor_2018_runtime] https://github.com/andeevosters/VBA_StockMarketAnalysis/blob/main/Resources/VBA_Challenge_2018.png

## Summary
### Advantages and Disadvantages of Refactoring Code
#### Advantages
	•	It can significantly decrease the run time, which in turn saves file space in storage
	•	It can help make the code easier to read and/or manipulate in the future, whether you read it again or someone else needs to view it
	•	It helps a developer think bigger and broader about a solution 

#### Disadvantages
	•	It can be time-consuming
	•	It is possible to miss critical changes that are hard to identify
	•	It may not improve your original code by much, in the end

### How The Pros and Cons Apply To This Challenge
Refactoring, although time-consuming, and at times quite frustrating, was advantageous in the end, because it significantly cut down on run time. While that may not make a big dent in the analysis now, once we move beyond analyzing 12 stocks to all of them, the refactoring will very much prove itself to be worthwhile.
