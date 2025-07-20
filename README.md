# DSA-Amazon-Analysis-Project
##The raw Excel file was carefully cleaned to ensure accurate analysis and reliable insights. Below are the steps taken:
Created calculated columns:

discount_percentage = (actual_price - discounted_price) / actual_price * 100

potential_revenue = actual_price * rating_count

price_bucket (e.g., <₹200, ₹200–₹500, >₹500)
 ##
Step 2: Pivot Table Analysis — Mapping to Analysis Questions

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
