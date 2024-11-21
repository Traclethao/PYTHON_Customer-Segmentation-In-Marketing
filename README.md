# Customer Segmentation In Marketing  
## **I. Introduction**

### **1. About RFM Analysis**

**RFM (Recency – Frequency – Monetary)**: is a part of **Marketing Analysis** and is used to analyze customer value to help businesses analyze each customer group they have. From there, there are **special marketing** or **care campaigns**.

### **2. About business**
- SuperStore Company is a **global retail company**, so the company has a lot of customers.

- On the occasion of Christmas and New Year, the Marketing department wants to **run marketing campaigns** to thank customers who have supported the company over the past time. As well as exploit customers with the potential to become loyal customers.

- However, the Marketing department has not yet been able to group each customer this year because the data set is too large to be processed manually like previous years, so the Data Analysis Department should support the implementation of a **segmentation problem for each customer to implement each marketing program suitable for each customer group**.

## **II. EDA & RFM Model** 

### **1. EDA**
#### **1.1. Import data from Excel file**
- Code

  ![Import data](https://github.com/user-attachments/assets/760d004f-3f76-4f18-b97b-09bb03363808)

- Result

  ![Result 1 11](https://github.com/user-attachments/assets/03691798-2ccd-4eba-be33-6743a47556c5)
  ![Result 1 12](https://github.com/user-attachments/assets/dd09484a-52e0-450b-b226-179eea4e14f4)

#### **1.2. Check & Handle data**
- df table 
  + Check Missing, Dupplicate, incorrect data
  
  ![Check](https://github.com/user-attachments/assets/8df1e55b-ef3e-431e-bd15-33055ab878e0)
  
  + Handle

    ![handle](https://github.com/user-attachments/assets/cc751102-fe21-4d88-9bb2-561bfdb226f1)
    ![Create report](https://github.com/user-attachments/assets/f5e82af9-2152-4db6-8140-c978352c8937)

  + Result

    ![2 11](https://github.com/user-attachments/assets/30e4c623-8856-4870-9bfa-b784cba02a95)
    ![result 2 12](https://github.com/user-attachments/assets/af04db3f-d868-463c-8c18-fee7bd2bc122)

- Segmentation table
  + Code

    ![Segment](https://github.com/user-attachments/assets/c37a5483-d8b7-4d06-baa5-db247e7c2ffb)

  + Result
  
    ![result segment](https://github.com/user-attachments/assets/153d643d-57b9-43bb-87a4-b59352f28e30)

 
  
### **2. Calculation the R, F, M scores of each customer**. 
Note: The calculation date of the R index is December 31, 2011.

### **3. Use the quintile method of Statistics to scale R_score, F_score, M_score.**


### **4. Use Segmentation table to group each customer**


## **III. Data Visualization & Insight**

### 1. Histogram chart 
- **Distribution of Recency and Distribution of Recency with R_score>=3**

  ![Recency](https://github.com/user-attachments/assets/c8012ebc-4081-4a7e-919c-ae50ab3da6bf)

  => Cut with the condition <= 92 days (R_score is 3,4,5) has the highest distribution for a clearer view. In the range of 21-40 recent days, the highest distribution proves that the business is currently operating very well. 


- **Distribution of Frequency and Distribution of Frequency with F_score<=4** 

  ![Frequency](https://github.com/user-attachments/assets/747817a9-5250-4386-8719-0dcbc5354d24)

=> Cut with the condition <= 120 purchases (F_score is 1,2,3,4). For the customer group with F_score = 5, which is over 120 purchases (accounting for 1/5 of the total number of customers), the business should have its own customer appreciation program. In the cut chart, it can be seen that the number of customers who purchase from 1-20 times is the highest.


- **Distribution of Monetary Histogram and Distribution of Monetary with M_score<=4** 

  ![Monetary](https://github.com/user-attachments/assets/436c9284-49f0-463b-88e5-6f32338d4d30)

  => Cut with the condition <= 1957.32 USD (M_score is 1,2,3,4). For the group of customers with F_score=5 above 1957.32 USD (accounting for 1/5 of the total number of customers but bringing a lot of profit to the business), these may be the agents, the business should have its own customer appreciation program.

### 2. Treemap chart 
- **RFM Segments of Customer Count** 

  ![Count](https://github.com/user-attachments/assets/a017982a-aa7b-4a98-98cf-98043219c743)

- **RFM Segments of Sales** 

  ![Sales](https://github.com/user-attachments/assets/8babcd5d-5c4f-4731-8e59-951e70e90002)

**=> Insights:**
- Champions segment has about 18.42% of customers but brings in revenue up to 59.06%. => Need to maintain a Champions customer group.
- Besides, need to study the Cannot Lost Them group to gain experience, not lose more Champions and Loyal.
- Find ways to convert Potential Loyalist, Need Attention, At Risk, Promising groups into Champions and Loyal customer groups.

## **IV. Recommendations**

![Recommendation](https://github.com/user-attachments/assets/3c35fcd3-2ba1-49fb-89f5-c6c350de8930)

