 # EZFix-EXCEL-portfolio
 This file features our Excel programs used to automate monthly sales reporting, client issues, stocks, revenue, and profit. By automating these tasks using Excel, we were able to focus on priorities which required further attention, such as the syrnchonization between our clients and our databases. 

Data entry is seen as both tedious and time-consuming, especially within a fast-paced environment where time is of the essence. A business cannot risk losing clients due to the aforementioned delays. Consequently, I decided to establish an automated system in Excel where these tasks could be completed seamlessly.One such example lay in our stock and revenue. 

Normally, I had to manually insert values such as the price per unit for our aftermarket parts, coordinate with our clients to observe how many parts we needed, determine how many aftermarket parts were in our inventory, and then calculate the final revenue. To reduce human error throughout this process, I determined that the XLOOKUP function was critical for extracting values from one table to another, in order to verify whether our aftermarket parts were available in our inventory.
```excel
=IF(G3>XLOOKUP(F3,B:B,D:D),"Stock Unavailable","Available")
```
Furthermore, I engineered a financial model to audit monthly revenue metrics and track profit margins, which reduced data entry errors by 80%. Additionally, this saved valuable time, allowing us to expedite our efforts toward creating one of the most challenging parts of our business, the data synchronization between our clients and databases. Below are a few samples of what I implemented to make data entry automation possible. 
```excel
=[@[Price per Unit]]*[@[Quantity Requested]]
=[@Charge] - [@[Repair Cost]]
```
By utilizing caculation equations, we were not only able to save time but also give us a pinpoint answer for our revenue and our profit margin, thus resulting in a fair and balanced wages. Similiarly, we avoided wasting time by entering our clients names through multiple sheets by leveraging the following equation. 
```excel
=XLOOKUP(A3,'Customer Info'!A:A,'Customer Info'!B:B)
```
Simply put, XLOOKUP would look through our "Customer Info" sheet, and fetches values from our customer names under the aforementioned sheet. 
