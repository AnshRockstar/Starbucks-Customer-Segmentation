<h1 align="center"> Starbucks-Customer-Segmentation</h1>
<p align="center"> 
<img src="https://github.com/AnshRockstar/Starbucks-Customer-Segmentation/blob/main/Images/starbucks-coffee-starbucks.gif" alt="Animated gif" height="498px">
</p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📋 Abstract
This case study analyizes data provided by Starbucks that simulates their customer demographics and transactional activities during a promotional campaign. 
The campaign lasted for around a month, during which customers received a variaty of offers. The purpose of this case study is to understand customer response to different offers in order to come up with better approaches to sending customers specific promotional deals. 
Customers are classified into segments based on their transactional activities, so that specific recommendations can be given regarding individual segments to improve customer stickiness, brand awareness and increase revenue in general. 
Customer segmentation also provides insights on new customer targeting.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

##  💾 Project Files Description

<p>This Project includes 1 colab notebook and 3 datasets :</p>

### Executable Files:
- [Starbucks-Customer-Segmentation](https://github.com/AnshRockstar/Starbucks-Customer-Segmentation/blob/main/Starbucks_Customer_Segmentation.ipynb) - Includes all functions required for clustering the customers.

### Output:
- [Google Colab](https://github.com/AnshRockstar/Starbucks-Customer-Segmentation/blob/main/Starbucks_Customer_Segmentation.ipynb) - All the outputs are visible in the provided colab notebook.

### Input Files:
  <li><b>Portfolio.xlxs</b> - It contains the offer_id,reward,diffculty,channels and durations for the offer .</li>
  <li><b>Profile.xlxs</b> - It contains the demographics details about the customers.</li>
  <li><b>Transcation.xlxs</b> - It contains the transactional details about the customers.</li>
  
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📖 Introduction:

In today’s scenario we can see that offers and discount playing an important role in retain any customers and also add new customers. With enormous challenge from everywhere throughout the globe, it is
important for a Starbucks to realize that it is  continuing in the right way or not. To hold their place in the market, Starbucks need support to figure out how to attract new_customers and also reduce churn rate of the customers.
In our data set we have three xlxs files for data analysis:
Portfolio
Profile
Transcation
At first, we analysis the Portfolio data we have 10 rows and 8 columns , in the Profile data we have 14825 rows and 6 columns of data & in the Transcation data we have 197416 and 6 columns of data. We have to take the maximum outcomes from the data which help us to analysis the better approaches to sending customer offers and recommended strategies regarding specific customer groups. 
Our goal is to filter and make plots accordingly for a better EDA with respect to the final data. We need to explore and analyze the data to discover key factors responsible for recommended strategies regarding specific customer groups and better approaches to sending customer offers. 

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
### The contents of Portfolio are:

* reward: (numeric) money awarded for the amount spent.
* channels: (list) web, email, mobile, social.
* difficulty: (numeric) money required to be spent to receive reward.
* duration: (numeric) time for offer to be open, in hours.
* offer_type: (string) bogo, discount, informational.
* Offer_id: (string).

### The contents of Profile are:

* gender (str): gender of the customer (M: Male, F: Female, O: Others).
* age (int): age of the customer.
* id (str): customer id.
* became_member_on (int): the date when the customer created an app account.
* income (float): customer’s income.

### The contents of Transcation are:

* id: (string)customer id.
* event: (string) offer received, offer viewed, transaction, offer completed.
* offer id: (string) not associated with any "transaction".
* amount: (numeric) money spent in "transaction"
* reward: (numeric) money gained from "offer completed"
* time: (numeric) hours after start of test

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📋Problem Statements

1. Which Offer were Popular?
2. Do different groups of people react differently to offers.
3. Do people generally view and then use the offer? or they use the offer without notice it.
4. Which group of people is more likely to use the offer or make a purchase WITHOUT viewing the offer, if there is such a group?
5. Which type of offer is more likely to be used WITHOUT being viewed, if there is one?
6. RFM Distribution in the dataset.
7. How does demographic factors affect each groups.
8. How the transcational activities varies across different groups.


********************************************************************************************************************************************************************
## 📔 **What is Exploratory Data Analysis?**
Exploratory data analysis (EDA) is used by data scientists to analyze and investigate data sets for patterns, and anomalies (outliers), and form hypotheses based on our understanding of the dataset and summarize their main characteristics, often employing data visualization methods. It is an important step in any Data Analysis or Data Science project. It helps determine how best to manipulate data sources to get the answers you need.

EDA involves generating summary statistics for numerical data in the dataset and creating various graphical representations to understand the data better and make it more attractive and appealing.

The following are the various steps involved in the EDA process:
1. <b>Problem Statement</b> - We shall brainstorm and understand the given data set. We shall study the attributes present in it and try to do a philosophical analysis about their meaning and importance for this problem.
2. <b>Hypothesis</b> - Upon studying the attributes present in the data base, we shall develop some basic hypothesis on which we can work and play with the data to look for the varied results which we can get out of it.
3. <b>Univariate Analysis</b> - It is the simplest form of analyzing the data. In this we would initially pick up a single attribute and study it in and out. It doesn't deal with any sort of co-relation and it's major purpose is to describe. It takes data, summarizes that data and finds patterns in the data.
4. <b>Bivariate Analysis</b> - This analysis is related to cause and the relationship between the two attributes. We will try to understand the dependency of attributes on each other.
5. <b>Multivariate Analysis</b> - This is done when more than two variables have to be analyzed simultaneously.
5. <b>Data Cleaning</b> - We shall clean the dataset and handle the missing data, outliers and categorical variables.
6. <b>Testing Hypothesis</b> - We shall check if our data meets the assumptions required by most of the multivariate techniques.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📖	Steps Involved
After loading the dataset, we can start the exploration but before that, we need to check and see that the dataset is ready for performing several exploration operations or not, so let’s first have a look at the structure and the manner in which the data is organized.

### Data Cleaning
Our data set doesnot contains any null and duplicated values.

### Data Transforming 
From the information of data frame, we perform binning on the age and income columns.

### Exploratory Data Analysis
After establishing a good sense of each feature, we proceeded with plotting a pairwise plot between all the quantitative variables to look for any evident patterns or relationships between the features

### Single Variate Analysis
After that we analysis all the columns one by one to examine whether the particular column contain some useful information or not:


## 📋 Conclusion:
* Income: Most people are in the 40k-80k income-range, 19% of the earners which is the 50k-60k income range. Gender: 58% male users compared to 42% Females. Age: the age group with the highest percentage in the members is 48–58 with 24%, the smaller group consists of the older generation (88–98). RFM Segments and Customer Groups

* RFM Segments Distribution: 41% of the customers are in the Low-value RFM group followed by the Mid-value RFM group, and the High RFM group with 23% of customers. Customer Groups Distribution: 40% of the customers are in the Treatment response(TR) while the CR group had 14.9% of the customers. This can explain why the quadrant models performed worst on CN. Gender in the RFM segments: The Males are present in the low-value and mid-value RFM while the females have a higher percentage in the high-value segment. The Purchasing Behavior in RFM Clusters

* Total spent vs RFM segment: there was a clear difference between the different segments in terms of amount spent. Customer segments vs RFM clusters: The mid and high-value segments had higher percentages of the response compared to the low-value segment. This indicates that high and mid-value customers are responsive to targeted marketing while it did not make a difference in the Low values. Customer Groups vs Demographic

* Income vs Customer Segment: The highest income customers are in TR or CR group. Total Spent vs customer segment: The difference in the amount of money spent between the treatment and control groups is significant.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 💶 Credits

Contact me for Data Science Project Collaborations

[![GitHub](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)]([https://carrd.co/](https://anshbhatnagar.carrd.co/))
[![LinkedIn](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ansh-bhatnagar-093609117/)

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📚 References
*	GeeksforGeeks
*	Analytics Vidhya
*	Stackoverflow
*	Towards data science
*	Python libraries documentation
*	Data camp
* Medium

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📜 Feedback
If you have any feedback, please reach out to us at 123anshbhatnagar@gmail.com
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
