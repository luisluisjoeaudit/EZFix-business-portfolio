 # EZFix-EXCEL-portfolio
 This file features our Excel programs used to automate monthly sales reporting, client issues, stocks, revenue, and profit. By automating these tasks using Excel, we were able to focus on priorities which required further attention, such as the syrnchonization between our clients and our databases. 

## Our Goal
Data entry is seen both as tedious and time-consuming, especially within a fast-paced enviroment where time is of the essence. A business could not risk losing clients due to the aforementioned expedits. Consenquently, I decided to establish a automated system in Excel where these tasks could be completed automatically. 

One such example laid in our stocks and revenue. Normally, I had to manually insert values such as the price per unit for our aftermarket parts, coordinate with our clients and observe how many parts we needed, how many aftermarket parts were in our inventory, and then caculate the final revenue. To reduce human error through this process, I determined that a XLOOKUP function was critical for extracting values from one table to another to verify whether our aftermarket parts were available or not within our inventory. 
```excel
=IF(G3>XLOOKUP(F3,B:B,D:D),"Stock Unavailable","Available")
```
Furthermore, 
