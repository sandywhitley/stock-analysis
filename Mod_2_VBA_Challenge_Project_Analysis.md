#Module 2 VBA Challenge 
Sandy Whitley 9/27/20

### Overview of Project
This goal of this project was to refactor a VBA script to run more efficiently and quickly for a stock ticker performance summary. 

### Results
The refactored VBA script and original VBA script produced identical correct outputs however the refactored VBA script ran 75%-76% more quickly than the original script.
![VBA Script Run Time Analysis](/resources/VBA_Challenge_Perf_Overview.png)
![Original 2017 VBA Script Run Time](/resources/VBA_Challenge_Before_2017.png)
![Refactored 2017 VBA Script Run Time](/resources/VBA_Challenge_After_2017.png)
![Original 2018 VBA Script Run Time](/resources/VBA_Challenge_Before_2018.png)
![Refactored 2018 VBA Script Run Time](/resources/VBA_Challenge_After_2017.png)

### Summary
The data consisted of 2 separate worksheets, 2017 and 2018, containing a daily stock performance information including the ticker symbol, date, open price, high price, low price, close price, 
adjusted close, and trade volume. Both the scripts compiled the total daily volume and the return based on the starting close ticker price and the ending ticker close price for each unique ticker symbol. 

The original script looped through the entire script for each ticker symbol independently. In the refractored VBA script, a tickerIndex was created and included in a loop which eliminated redundant looping 
and thus processing time. This project demonstrated the benefits of refractoring script to remove redundancy and improve efficiency.