## **Project name:** Sephora Products & Skincare Analysis

**Objective**: I acted as an independent data consultant 


**Project Overview:** 

This project will leverage a comprehensive dataset of Sephora beauty products and user reviews to derive actionable insights for product pricing and promotions, brand and product performance analysis, competitive analysis, and trend identification. It aims to drive strategic decisions that will enhance product offerings, improve customer satisfaction, and achieve business growth in the beauty industry. 


**Problems**: 

1. **Optimizing Product Pricing and Promotions**
2. Determine the optimal pricing strategy and promotion tactics to maximize revenue and customer satisfaction.
3. **Brand and Product Performance Analysis**: Understand which brands and products perform best and why
4. **Competitive Analysis**: Gain insights into how Sephora’s products and brands compare to competitors
5. **Trend Identification**: Identify emerging trends in the beauty and skincare industry to stay ahead of market changes


**Questions**:

Q1: Which products show the highest increase in sales during the Sephora exclusive?

Q2: How do limited edition offers impact customer purchasing behavior?

Q3: Which brands have the highest ratings and customer satisfaction levels?

Q4: What are the top-performing products in terms of revenue?

Q5: How do Sephora’s product ratings and reviews compare to competitors? 

Q6: What categories were popular based on sales?


**Data Source**: Kaggle

Dataset - Sephora Products & Skincare Review

Link to the raw dataset:  https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews?select=product_info.csv


**Tools Used**:  

Data Analysis part → Data Visualization part

 MS Excel —>Microsoft SQL Server —> Microsoft Power BI 


**Data analysis**: 

Performed the three-phase process called ETL by extracting the raw dataset from the Kaggle website and loading it into Microsoft Excel by using power query to transform the data for analysis. Then input the clean dataset into the MYSQL server to query for data insight.

The SQL code portion of Microsoft SQL Server:

SELECT 
    p.product_id, 
    p.product_name, 
    p.brand_id, 
    p.brand_name, 
    r.author_id, 
    p.loves_count, 
    p.rating, 
    p.reviews, 
    p.size, 
    p.variation_value, 
    p.ingredients, 
    p.limited_edition, 
    p.new, 
    p.online_only, 
    p.sephora_exclusive, 
    p.highlights, 
    p.category, 
    p.child_count, 
    p.child_max_price, 
    p.child_min_price, 
    r.helpfulness, 
    r.total_feedback, 
    r.total_negative_feedback, 
    r.total_positive_feedback, 
    r.date, 
    r.skin_tone, 
    r.eye_color, 
    r.skin_type, 
    r.hair_color, 
    r.price_usd, 
    p.revenue 
FROM product_info AS p
LEFT JOIN reviews_info AS r
ON p.product_id = r.product_id;


**Data Visualization:** 

I used Power BI to visualize the analysis findings in the Sephora beauty products and user reviews dataset, highlighting patterns and trends for business decision-making.


**Dashboard:**

[Sephora Products & Skincare Analysis.pdf](https://github.com/user-attachments/files/16549338/Sephora.Products.Skincare.Analysis.pdf)


**Insights from the analysis**: 

Upon analyzing the datasets, several noteworthy insights into Sephora's business performance have been shown. The data underscores the prominence of The Ordinary, Drunk Elephant, Tatcha, Sunday Riley, and Biossance as the top five brands within the Sephora portfolio. It is worth noting that La Mer's Creme de la Mer Moisturizer has emerged as the highest revenue-generating product, followed closely by Drunk Elephant's Protini Polypeptide firming refillable moisturizer. Additionally, the data indicates a distinct preference among Sephora's clientele for skincare products over beauty items, along with a tendency to favor product offerings from competitors over those of Sephora.

**Recommendation:**

As a data consultant, I strongly advise Sephora's regional managers to prioritize stocking high-revenue brand names such as La Mer, Drunk Elephant, SK-II, Charlotte Tilbury, and Sunday Riley to drive sales and boost overall revenue.
