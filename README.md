# Sales-Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/63aefb39-ca90-42b3-8488-f5c99ac6395f/ReportSection?experience=power-bi

## Problem Statement

This dashboard serves as a vital tool for the company, offering deep insights into their sales performance. By providing a comprehensive overview, it enables the company to gauge satisfaction levels with current sales, pinpoint areas for improvement, and ultimately enhance overall sales figures. Specifically, it sheds light on crucial metrics such as Total Revenue, profit margins, and quantity sold across different states, years, and categories.

Notably, the data underscores a significant opportunity for growth within the Technology category, which contributes approximately 46% of total profits and sales, compared to Office Supplies (roughly 35%) and Furniture (about 19%). This highlights a clear imperative for the company to focus on optimizing profitability and sales within this particular category to maximize overall performance.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Transformed data as per required.
- Step 3 : Calculated column was created.

for creating new column following DAX expression was written;
       
        Day of Week = WEEKDAY(Orders[Order Date],2)

        Weekday/Weekend = IF(Orders[Day of Week]=6 || Orders[Day of Week]=7,"Weekend","Weekday")
        
        Days of Shipment = DATEDIFF(Orders[Order Date],Orders[Ship Date],DAY)

        Customer Name = Orders[First Name] & " " & Orders[Last Name]
Snap of new calculated columns ,

![image](https://github.com/JaiKattimani45/Power-BI-Dashboard/assets/110810509/b266b232-cc46-4903-ab5a-e4cc7bfd9b86)

 
 # Report Snapshot (Power BI DESKTOP)

![image](https://github.com/JaiKattimani45/Power-BI-Dashboard/assets/110810509/cbb431fe-1ca0-4877-b9fe-d056306cf5bd)

![image](https://github.com/JaiKattimani45/Power-BI-Dashboard/assets/110810509/7149ce90-90a2-431b-a2e6-07e54a248553)

![image](https://github.com/JaiKattimani45/Power-BI-Dashboard/assets/110810509/a29444c0-bb0f-4518-b68c-4319074eab1a)


# Insights

A multi page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

###  Total Revenue = $12.64M

![image](https://github.com/JaiKattimani45/Power-BI-Dashboard/assets/110810509/e6166fe9-6055-4d74-a644-37b10ac4de83)
   - Consumer = $6.51M (51.48%)        
   - Corporate = $3.82M (30.25%)
   - Home office = $2.31M (18.27%) 
   

           thus, higher number of Sales & Profit are from Consumer Segment.
           
### Some other Insights 

![image](https://github.com/JaiKattimani45/Power-BI-Dashboard/assets/110810509/3ddb12a9-6558-41d0-b474-e7d4fb3be544)

        thus, higher number of Sales are in Quarter 4 for every year.

![image](https://github.com/JaiKattimani45/Power-BI-Dashboard/assets/110810509/830661ae-fbb7-46d6-a66f-828af16f747d)

        thus, New York City has higher number of Quantity sold & Porfit earned.
        
### Conclusion
The Sales Dashboard serves as a powerful tool for analyzing sales performance at various levels of granularity. By harnessing the insights it provides, users can enhance their understanding of sales trends, identify areas for improvement, and drive business growth.
