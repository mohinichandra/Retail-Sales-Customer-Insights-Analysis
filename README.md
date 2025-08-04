# Retail-Sales-Customer-Insights-Analysis

### Project Overview:
This project showcases the end-to-end analysis of a retail business using SQL and Power BI. The goal of this project is to extract actionable insights on sales trends, product performance, regional profitability, and customer behavior to support strategic decision-making.

### Key Objectives
1. Track overall business performance (Sales, Profit, Margins)
2. Identify top-performing products and categories
3. Analyze customer segments and purchasing patterns
4. Understand regional and state-wise performance
5. Explore the impact of discounts on profitability
6. Present trends over time and highlight business recommendations

### Tools & Technologies Used
1. SQL -	Data cleaning, transformation, relationship building, and querying
2. Power BI -	Interactive dashboards and data visualization
3. Excel -	Data splitting and preprocessing

DAX Queries:
1.Average Order Value(AOV) = AVERAGE(Orders_Table[Sales])
2. Average Spent per Customer = DIVIDE(SUM(Orders_Table[Sales]),DISTINCTCOUNT(Orders_Table[Customer ID]))
3. Profit Margin % = DIVIDE([Total Profit],[Total Sales])*100
4. Repeat Customer % = DIVIDE(COUNTROWS(FILTER(CustomersOrder,CustomersOrder[Order Count] >1)),
COUNTROWS(CustomersOrder)
)*100

5. Total Profit = SUM(Orders_Table[Profit])*100
6. Total Sales = SUM(Orders_Table[Sales])
7. CustomersOrder = SUMMARIZE(Orders_Table, Orders_Table[Customer ID],"Order Count",COUNTROWS(VALUES(Orders_Table[Order ID])))

### Dashboard : 
1. Overview Page
<img width="1319" height="727" alt="Screenshot 2025-08-02 061803" src="https://github.com/user-attachments/assets/49555f86-9337-4287-b4cf-34df6a0a0292" />

3. Customer Insight Page
<img width="1308" height="726" alt="Screenshot 2025-08-02 061845" src="https://github.com/user-attachments/assets/774a694b-2417-4f07-8ddf-a948da70a940" />

4. Product Analysis Page
<img width="1292" height="726" alt="Screenshot 2025-08-02 061929" src="https://github.com/user-attachments/assets/baef5263-31a2-42d8-965b-d219a996d0fa" />

5. Geographic Analysis Page
<img width="1295" height="727" alt="Screenshot 2025-08-02 062011" src="https://github.com/user-attachments/assets/6df876c2-ad7b-4bcf-acf1-efaada3a005f" />
         
Outcome:
1. Kin Lonsdale is the top customer with generating hishest revenue.
2. West Region is generating high profit, South region has poor performance.
3. Sales peaked during November–December, indicating a strong seasonal trend.
4. Consumer section is perfoming well, we need to focus more on Home Office
5. West region has more customers, we need to target more on South region with low customer count.
6. There is increase in customer during november to december.
7. There is huge demand in Technology, followed by Office Supply
8. We need to focus in Tables as it is generating less profit.
9. High demand in Phones and least demand in Fateners.
10. California brings the highest profit and Georgia brings the least profit.
