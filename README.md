# <u> Credit Card Customer Segmentation</u>

--------------------------------------------------------------------------------
<p align="center">
  <img src="credit_cards.jpeg" style="width: 800px; height: 270px;" />
</p>



**Business Context:** This project aims to develop a customer segmentation to define marketing strategy. The dataset has about 9000 credit card holders information for last 6 months.


## Project Overview
* Derived new KPI by using data manipulation methods.
* Checked the multi-collinearity using heatmap.
* Standardized the data and applyied PCA to get optimal number of Pricipal Components.
* KMeans Clustering is used - Silhotte Score and Cluster Inertia Score used to fix the number of clusters.
* Done profiling to draw insights for the clusters.

## Dataset Description

<b>CUST_ID:</b> Credit card holder ID<br>
 <b>BALANCE:</b>  Monthly average balance (based on daily balance averages)<br>
 <b>BALANCE_FREQUENCY:</b>  Ratio of last 12 months with balance<br>
 <b>PURCHASES: </b> Total purchase amount spent during last 12 months<br>
 <b>ONEOFF_PURCHASES: </b> Total amount of one-off purchases<br>
 <b>INSTALLMENTS_PURCHASES: </b> Total amount of installment purchases<br>
 <b>CASH_ADVANCE: </b> Total cash-advance amount<br>
 <b>PURCHASES_FREQUENCY: </b> Frequency of purchases (Percent of months with at least one purchase)<br>
 <b>ONEOFF_PURCHASES_FREQUENCY: </b> Frequency of one-off-purchases<br>
 <b>PURCHASES_INSTALLMENTS_FREQUENCY: </b> Frequency of installment purchases<br>
 <b>CASH_ADVANCE_FREQUENCY: </b> Cash-Advance frequency<br>
 <b>AVERAGE_PURCHASE_TRX:</b>  Average amount per purchase transaction<br>
 <b>CASH_ADVANCE_TRX: </b> Average amount per cash-advance transaction<br>
 <b>PURCHASES_TRX: </b> Average amount per purchase transaction<br>
 <b>CREDIT_LIMIT:</b>  Credit limit<br>
 <b>PAYMENTS: </b> Total payments (due amount paid by the customer to decrease their statement balance) in the period<br>
 <b>MINIMUM_PAYMENTS: </b> Total minimum payments due in the period.<br>
 <b>PRC_FULL_PAYMEN: </b> Percentage of months with full payment of the due statement balance<br>
 <b>TENURE: </b> Number of months as a customer<br>


## Final Clusters and Recommendations 
* Based on silhouette_score, i have taken number of clusters to be 4.

<p align="center"><img src="Picture5_clusters_plot.png"  style="width: 600px; height: 370px" /></p>

* **Suggested Marketing Strategy for these clusters:**


* Group 0 
   - They are potential target customers who are paying bills and doing purchases and maintaining comparatively good credit score. So we can <i>increase credit limit or can lower down interest rate. Promote premium cards/loyality cards</i> to increase transcations.
   
* Group 1
   - These customers are taking maximum cash advance, these customers should be given remainders for payments. Offers can be provided on early payments to improve their payment rate.

* Group 2
   - This is performing best among all the clusters are maintaining highest monthly average purchases. Giving any reward points might increase their purchases.
   
* Group 3
   - This group is doing maximum oneoff payments(may be for bills only). Customers of this group can be offered discount/offer on next transactions upon full payment.
   
