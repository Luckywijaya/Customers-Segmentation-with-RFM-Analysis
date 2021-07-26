# Customers-Segmentation-with-RFM-Analysis

In determining the performance of customer purchases, we use 3 parameters: <br>
1. **Recency**: Number of days from last order until the last date data was taken <br>
2. **Frequency**: Total orders amount <br>
3. **Monetary**: Total amount that the customer has spent on order 
<br><br>
The range of score values for every parameter is 1 to 4. The higher value means better performance. <br>
From the combination of these three parameters, we will create RFM score. From each parameter, the RFM score will be added up to get the total RFM, the total RFM value is used as segmentation for customers whose performance is low, medium, high.
<br><br>
**Segmentation** <br>
TotalRFM <= 5 : Low <br>
TotalRFM 6-9 : Medium <br>
TotalRFM > 9 : High 
<br><br>
With explanation as follows:<br>
Min TotalRFM 3 (combined RFM score: 111)<br>
Max TotalRFM 12 (combined RFM Score: 444)
<br><br>
The low limit is five because the customer has to have a minimum value of 2 points in each parameter or has more value in one of the parameters. <br>
The high limit is nine because there is a possibility that the customer has a total value of 9 with a combination of 144. This means that the customer often makes purchases with large total orders. However, the customer has not repurchased for a long time. <br>
Customers can have a total value of nine with a combination of 414 which means that the customer has just purchased with a large nominal amount. However, the customer has only made a purchase once so he has not become a loyal customer.
<br><br>
The RFM value uses the 25%, 50%, 75% percentile to see the distribution of the data on each parameter and divides it into 4 parts to determine the high/low parameter values owned by each customer. Example: A customer has RFMScore 344 and TotalRFM 11. It means that the customer has a value of Recency 3, Frequency 4, and Monetary 4. This means that the customer has recently placed an order. These customers often place orders and with a large total nominal. If the RFMScore is added, it will total 11 points. This indicates that the customer is included in the high segmentation because it has a total score of more than 9 points.
