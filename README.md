# Starbucks-Customer-Segmentation
EDA on the Starbucks customer Segmentation


Summary of the project
we will analyze simulated data that mimics customer behavior on the Starbucks rewards mobile app. The data provides information about the user demographics, offer details, and the user event log.

Starbucks sends out an offer to users of the mobile app, once every few days. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Also, some users might not receive an offer during certain weeks. The offers can be divided into 3 main types:

BOGO(buy-one-get-one): the user needs to spend a certain amount to get a reward equal to a threshold amount.
Discount: the user gains a reward equal to a fraction of the amount spent.
Informational: This offer contains no reward nor a minimum amount spent.
The main questions we are interested in answering from the analysis:

Can we identify which groups of people are most responsive to each type of offer?
Can we increase Starbucks ‘ profit by adopting a selective promotion strategy instead?
Furthermore, we will use RFM(Recency-Frequency-Monetary) clustering which is a method for customer segmentation. This method divides the customer’s into groups based on their purchase recency, frequency, and monetary value.

In this project, we presented the uplift modeling approach as a way to study the customer's response to offers. The current promotion strategy was to send offers to all the customers, this is a wasteful approach and costly since not all customers respond equally to offers. Additionally, RFM clustering was used in the model features and to segment the customer on purchasing behavior.

So what we have demystified at the course of the analysis?

Customer Demographics:

Income: Most people are in the 40k-80k income-range, 19% of the earners which is the 50k-60k income range.
Gender: 58% male users compared to 42% Females.
Age: the age group with the highest percentage in the members is 48–58 with 24%, the smaller group consists of the older generation (88–98).
RFM Segments and Customer Groups

RFM Segments Distribution: 41% of the customers are in the Low-value RFM group followed by the Mid-value RFM group, and the High RFM group with 23% of customers.
Customer Groups Distribution: 40% of the customers are in the Treatment response(TR) while the CR group had 14.9% of the customers. This can explain why the quadrant models performed worst on CN.
Gender in the RFM segments: The Males are present in the low-value and mid-value RFM while the females have a higher percentage in the high-value segment.
The Purchasing Behavior in RFM Clusters

Total spent vs RFM segment: there was a clear difference between the different segments in terms of amount spent.
Customer segments vs RFM clusters: The mid and high-value segments had higher percentages of the response compared to the low-value segment. This indicates that high and mid-value customers are responsive to targeted marketing while it did not make a difference in the Low values.
Customer Groups vs Demographic

Income vs Customer Segment: The highest income customers are in TR or CR group. 
Total Spent vs customer segment: The difference in the amount of money spent between the treatment and control groups is significant.
