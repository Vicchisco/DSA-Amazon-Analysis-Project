# DSA-Amazon-Analysis-Project
## Step1: The raw Excel file was carefully cleaned to ensure accurate analysis and reliable insights. Below are the steps taken:
Created calculated columns:

discount_percentage = (actual_price - discounted_price) / actual_price * 100

potential_revenue = actual_price * rating_count

price_bucket (e.g., <₹200, ₹200–₹500, >₹500)
 
## Step 2: Pivot Table Analysis 

Each of the following business questions was addressed using Pivot Tables, Calculated Fields, and Charts in Excel.

1. What is the average discount percentage by product category?

> Pivot grouped by category and used average of discount_percentage.

2. How many products are listed under each category?

> Used count of unique product_id per category.


3. What is the total number of reviews per category?

> Aggregated review_count in a pivot table grouped by category.


4. Which products have the highest average ratings?

>  Filtered and sorted pivot table based on rating in descending order.


5. What is the average actual price vs. discounted price by category?

>  Side-by-side column comparison using AVERAGE(actual_price) and AVERAGE(discounted_price) per category.


6. Which products have the highest number of reviews?

>  Sorted data by review_count descending to highlight top-reviewed products.


7. How many products have a discount of 50% or more?

>  Applied filter on discount_percentage >= 50% and counted.


8. What is the distribution of product ratings ?

>  Created rating bins (0-10, 11–20, 21–30, etc.) and used pivot to count frequency.


9. What is the total potential revenue (actual_price × rating_count) by category?

> Created calculated column potential_revenue, summed by category using pivot.

10. What is the number of unique products per price range bucket (<₹200, ₹200–₹500, >₹500)?

> Created a helper column price_bucket and used it in pivot to count product_id.


11. How does the rating relate to the level of discount?

> Used a line chart to visualize trends between rating and discount_percentage.

12. How many products have fewer than 1,000 reviews?

 Applied filter to review_count < 1000 and counted entries.


13. Which categories have products with the highest discounts?

> Sorted pivot table by average discount_percentage descending, grouped by category.


14. Identify the top 5 products in terms of rating and number of reviews combined.

> Created a score: rating × review_count to rank and list top 5 products.

## Visualisation
   visuals: Bar-Charts, Pie-Charts, Line Charts, simple plane shapes with figures
   
![Image alt](https://github.com/Vicchisco/DSA-Amazon-Analysis-Project/blob/main/Screenshot%202025-08-01%20011408.png?raw=true)

## Findings
•	From analysis the average discount percentage is 46.69% with the home improvement category having the highest percentage discount.
	
•	They are 9 categories in total. for the car and motorbike category there is just 1 product listed. For Computer and accessories  (453) product , for Electronics 526,  for health and personal care 1 product, Home and Kitchen (448), Home improvement (2) , Musical instruments  (2),  Office products (31) and toy and games Category  having just 1 product.

•	The total number of reviews is 26,766,377 with electronics category having the highest review as 15, 778,848 followed by computer and accessories (7,728,689), Home and kitchen (2,991,069), office products (149,675), Musical instruments (88,882), toys and games (15,867), home improvement (8,566), health and personal care (3663), and car and motorbike category having the least reviews as (1,118).

•	751 products have a discount of 50% or more.

•	The product with the highest average rating are, syncwire ltg, Amazon Basics Wireless, Redtech Usb-C with an Average rating of 5 each. Meanwhile the product with the highest number of reviews is Boat Bassheads 100 having a review total of 1, 091,137.

•	The total potential revenue is (121,197,753,243.63). With Electronics category having the highest potential revenue of (102,303,489,886) then Home and kitchen (14,192,788,365.70), Computer and accessories (4,679,436,446.93), Car and motorbikes (9,356,000), Office products (8,452,087), Musical instruments (1,926,132), Health and personal care (1,708,100), Home improvement (573,726) and toy and games having a potential revenue of (22,500)

•	The number of unique products <200 is 199, Unique product between 200-500 is 377 and that >500 is 889

•	1448 products have reviews fewer than 1000

•	The Computer and accessories category have the product with the highest Discounts with a maximum discount percentage of 94%

•	The top 5 products in terms of rating is Boat bassheads 100, redmi 9A sport, Amazon basic highspeed, Amazon Basic flexible premium, Jbl C100si wired.

   
