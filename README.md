# RFM Analysis
## **I. Introduction**

### **1. About RFM Analysis**

RFM (Recency – Frequency – Monetary): is a part of Marketing Analysis and is used to analyze customer value to help businesses analyze each customer group they have. From there, there are special marketing or care campaigns.
### **2. About business**
- SuperStore Company is a global retail company, so the company has a lot of customers.

- On the occasion of Christmas and New Year, the Marketing department wants to run marketing campaigns to thank customers who have supported the company over the past time. As well as exploit customers with the potential to become loyal customers.

- However, the Marketing department has not yet been able to group each customer this year because the data set is too large to be processed manually like previous years, so the Data Analysis Department should support the implementation of a segmentation problem for each customer to implement each marketing program suitable for each customer group.
### **3. Approach** 

- Prepare a data set suitable for the RFM model.
- Determine the calculation method and calculate the R, F, M scores of each customer. Note: The calculation date of the R index is December 31, 2011.
- Provide the calculation method with the corresponding score on a scale from 1 to 5.
- Use the classification table to group each customer.
- Visualize the number of segment sets with data dimensions.
- Analyze the current status of the company and give suggestions to the Marketing team.

## **II. Data Visualization with Python**

### 1. Histogram chart 
- Distribution of Recency and Distribution of Recency with R_score>=3 

  ![Recency](https://github.com/user-attachments/assets/c8012ebc-4081-4a7e-919c-ae50ab3da6bf)

- Distribution of Frequency and Distribution of Frequency with F_score<=4 

  ![Frequency](https://github.com/user-attachments/assets/747817a9-5250-4386-8719-0dcbc5354d24)

- Distribution of Monetary Histogram and Distribution of Monetary with M_score<=4 

  ![Monetary](https://github.com/user-attachments/assets/436c9284-49f0-463b-88e5-6f32338d4d30)

### 2. Treemap chart 
- RFM Segments of Customer Count 

  ![Count](https://github.com/user-attachments/assets/a017982a-aa7b-4a98-98cf-98043219c743)

- RFM Segments of Sales 

  ![Sales](https://github.com/user-attachments/assets/8babcd5d-5c4f-4731-8e59-951e70e90002)

## **III. Insights**

### 1. Histogram Chart: In general, all 3 variables have the same distribution pattern, the most distribution is on the left.
- Recency: cut with the condition <= 92 days (R_score is 3,4,5) has the highest distribution for a clearer view. In the range of 21-40 recent days, the highest distribution proves that the business is currently operating very well.
- Frequency: cut with the condition <= 120 purchases (F_score is 1,2,3,4). For the customer group with F_score = 5, which is over 120 purchases (accounting for 1/5 of the total number of customers), the business should have its own customer appreciation program. In the cut chart, it can be seen that the number of customers who purchase from 1-20 times is the highest.
- Monetary: cut with the condition <= 1957.32 USD (M_score is 1,2,3,4). For the group of customers with F_score=5 above 1957.32 USD (accounting for 1/5 of the total number of customers but bringing a lot of profit to the business), these may be the agents, the business should have its own customer appreciation program.
### 2. Treemap Chart:
- Champions segment has about 18.42% of customers but brings in revenue up to 59.06%. => Need to maintain a Champions customer group.
- Besides, need to study the Cannot Lost Them group to gain experience, not lose more Champions and Loyal.
- Find ways to convert Potential Loyalist, Need Attention, At Risk, Promising groups into Champions and Loyal customer groups.

## **IV. Recommendations**

![Recommendation](https://github.com/user-attachments/assets/2f28dc54-0288-4d14-8284-c5b255a63f67)

