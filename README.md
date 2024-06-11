# Atliq_hardware_SQL_Analysis

<p><b>Details of data:</b><p>
<p><b>1)Dim_customer table :</b></p>

<p> 1)Customer_code: A unique identifier for each customer. </p>
<p> 2)Customer: The name or identifier of the customer.</p>
<p> 3)Platform: The specific platform through which the customer interacts with the business. </p>
<p> 4)Channel: The means by which the customer was acquired or through which they interact with the company. </p>
<p> 5)Market: The geographic or demographic segment where the customer is located or to which they belong. </p>
<p> 6)Sub_zone: A more granular geographic or organizational subdivision within a market. </p>
<p> 7)Region: A broader geographic area that encompasses multiple sub-zones.</p>

<p><b>2)Fact_sales_monthly table:</b></p>
<p> 1)Date: The specific date when the sales transaction occurred. </p>
<p> 2)Product_code: A unique identifier for each product sold. </p>
<p> 3)Customer_code: A unique identifier for each customer.</p>
<p> 4)Sold_quantity: The quantity of the product sold in the specific transaction or during the specific period (e.g., month). </p>
<p> 5)Fiscal_year: The fiscal year in which the sales transaction occurred.</p>

<p><b>3)Dim_product table :</b></p>
<p> 1)Product_code: A unique identifier for each product. </p>
<p> 2)Division: A high-level classification of products, often representing a major product line or business unit within the company. </p>
<p> 3)Segment: A mid-level classification within a division, providing a finer categorization of products. </p>
<p> 4)Category: A more detailed classification within a segment, often used to further differentiate products based on specific features, uses, or customer preferences.</p>
<p> 5)Product: The specific name or identifier of the product. </p>
<p> 6)Variant: A specific version or variation of the product.</p> 

<p><b>4)Fact_manufacturing_cost table :</b></p>
<p> 1)Product_code: A unique identifier for each product</p>
<p> 2)Cost_year: The year in which the manufacturing cost was incurred. </p>
<p> 3)Manufacturing_cost: The total cost incurred in the manufacturing of the product for the specified year.</p> 

<p><b>5)Fact_pre_invoice_deduction table :</b></p>
<p> 1)Customer_code: A unique identifier for each customer.</p>
<p> 2)Fiscal_year: The fiscal year in which the pre-invoice deduction applies.</p>
<p> 3)Pre_invoice_discount_pct: The percentage of discount applied to the customer's invoice before it is issued.</p> 

<p><b>6)Fact_gross_price table :</b></p>
<p> 1)Fiscal_year: The fiscal year in which the gross price is applicable.</p>
<p> 2)Fiscal_year: The fiscal year in which the gross price is applicable.</p>
<p> 3)Gross_price: The gross price of the product for the specified fiscal year.</p>

<p><b>Questions:</b></p>

<p> Q1.Provide the list of markets in which customer "Atliq Exclusive" operates its business in the APAC region.</p>
<p> Q2.What is the percentage of unique product increase in 2021 vs. 2020? The final output contains these fields : 1) unique_products_2020 2) unique_products_2021 3)percentage_chg</p>
<p> Q3.Provide a report with all the unique product counts for each segment and sort them in descending order of product counts. The final output contains 2 fields: 1)segment 2)product_count</p>
<p> Q4.Which segment had the most increase in unique products in 2021 vs 2020? The final output contains these fields : 1) segment product_count_2020 2) product_count_2021 3)difference</p>
<p> Q5.Get the products that have the highest and lowest manufacturing costs. The final output should contain these fields: 1)product_code 2)product 3)manufacturing_cost</p>
<p> Q6.Generate a report which contains the top 5 customers who received an average high pre_invoice_discount_pct for the fiscal year 2021 and in the Indian market. The final output contains these fields: 1)customer_code 2)customer 3)average_discount_percentage.</p>
<p> Q7.Get the complete report of the Gross sales amount for the customer “Atliq Exclusive” for each month. This analysis helps to get an idea of low and high-performing months and take strategic decisions
The final report contains these columns: 1)Month 2) Year 3) Gross sales Amount.</p>
<p> Q8.In which quarter of 2020, got the maximum total_sold_quantity? The final output contains these fields sorted by the total_sold_quantity, Quarter total_sold_quantity.</p>
<p> Q9.Which channel helped to bring more gross sales in the fiscal year 2021 and the percentage of contribution? The final output contains these fields: 1)channel 2)gross_sales_mln 3)percentage.</p>
<p> Q10.Get the Top 3 products in each division that have a high total_sold_quantity in the fiscal_year 2021? The final output contains these fields: 1)division product_code 2) product 3)total_sold_quantity 4)rank_order.</p>
