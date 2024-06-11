# Atliq_hardware_SQL_Analysis

<p><b>1)dim_customer table :</b></p>

<p>customer_code: A unique identifier for each customer. </p>
<p>customer: The name or identifier of the customer.</p>
<p>platform: The specific platform through which the customer interacts with the business. </p>
<p>channel: The means by which the customer was acquired or through which they interact with the company. </p>
<p>market: The geographic or demographic segment where the customer is located or to which they belong. </p>
<p>sub_zone: A more granular geographic or organizational subdivision within a market. </p>
<p>region: A broader geographic area that encompasses multiple sub-zones.</p>

<p><b>2)fact_sales_monthly table:</b></p>
<p>date: The specific date when the sales transaction occurred. </p>
<p>product_code: A unique identifier for each product sold. </p>
<p>customer_code: A unique identifier for each customer.</p>
<p>sold_quantity: The quantity of the product sold in the specific transaction or during the specific period (e.g., month). </p>
<p>fiscal_year: The fiscal year in which the sales transaction occurred.</p>

<p><b>3)dim_product table :</b></p>
<p>product_code: A unique identifier for each product. </p>
<p> Division: A high-level classification of products, often representing a major product line or business unit within the company. </p>
<p>segment: A mid-level classification within a division, providing a finer categorization of products. </p>
<p>category: A more detailed classification within a segment, often used to further differentiate products based on specific features, uses, or customer preferences.</p>
<p>product: The specific name or identifier of the product. </p>
<p>Variant: A specific version or variation of the product.</p> 

<p><b>4)fact_manufacturing_cost table :</b></p>
<p>product_code: A unique identifier for each product</p>
<p>cost_year: The year in which the manufacturing cost was incurred. </p>
<p>manufacturing_cost: The total cost incurred in the manufacturing of the product for the specified year.</p> 

<p><b>5)fact_pre_invoice_deduction table :</b></p>
<p>customer_code: A unique identifier for each customer.</p>
<p>fiscal_year: The fiscal year in which the pre-invoice deduction applies.</p>
<p>pre_invoice_discount_pct: The percentage of discount applied to the customer's invoice before it is issued.</p> 

<p><b>6)fact_gross_price table :</b></p>
<p>fiscal_year: The fiscal year in which the gross price is applicable.</p>
<p>fiscal_year: The fiscal year in which the gross price is applicable.</p>
<p>gross_price: The gross price of the product for the specified fiscal year.</p>

<p>Questions:</p>

<p>Q1.Provide the list of markets in which customer "Atliq Exclusive" operates its business in the APAC region.</p>
<p>Q2.What is the percentage of unique product increase in 2021 vs. 2020?
The final output contains these fields : 1) unique_products_2020 2) unique_products_2021 3)percentage_chg</p>
<p>Q3. Provide a report with all the unique product counts for each segment and sort them in descending order of product counts. Final output contains 2 fields : 1)segment 2)product_count</p>
<p>Q4. Which segment had the most increase in unique products in 2021 vs 2020?
The final output contains these fields : 1) segment product_count_2020 2) product_count_2021 3)difference</p>
<p>Q5. Get the products that have the highest and lowest manufacturing costs.
The final output should contain these fields: 1)product_code 2)product 3)manufacturing_cost</p>
<p>Q6. Generate a report which contains the top 5 customers who received an average high pre_invoice_discount_pct for the fiscal year 2021 and in the Indian market. The final output contains these fields: 1)customer_code 2)customer 3)average_discount_percentage.</p>
<p>Q7. Get the complete report of the Gross sales amount for the customer “Atliq Exclusive” for each month . This analysis helps to get an idea of low and high-performing months and take strategic decisions
The final report contains these columns: 1)Month 2) Year 3) Gross sales Amount.</p>
<p>Q8. In which quarter of 2020, got the maximum total_sold_quantity? The final output contains these fields sorted by the total_sold_quantity, Quarter total_sold_quantity.</p>
<p>Q9. Which channel helped to bring more gross sales in the fiscal year 2021 and the percentage of contribution? The final output contains these fields: 1)channel 2)gross_sales_mln 3)percentage.</p>
<p>Q10.Get the Top 3 products in each division that have a high total_sold_quantity in the fiscal_year 2021? The final output contains these fields: 1)division product_code 2) product 3)total_sold_quantity 4)rank_order.</p>
