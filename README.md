# Amazon_Vine_Analysis

## Overview of Project
The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, I accessed approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. I picked one of these datasets (Furniture) and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. I also had the ability to use PySpark, Pandas, or SQL to determine if there was any bias toward favorable reviews from Vine members in your dataset.

## Results

Resources used:
- Data Source: [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), [Furniture Review dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Furniture_v1_00.tsv.gz)
- Software: Google Colab Notebook, PostgreSQL 12.5, pgAdmin 4, AWS

**Vine reviews Vs non-Vine reviews**:
For the entire Furniture product review file, the majority has a small Amazon Vine review: 
![vine](https://github.com/kushalishah/Amazon_Vine_Analysis/blob/main/Images/vine_novine_reviews.png)

**5 Star Reviews Vine vs Non-Vine:** 
For the entire review dataset, I found a few 5 Star reviews from Vine reviews:
![5star](https://github.com/kushalishah/Amazon_Vine_Analysis/blob/main/Images/5star_reviews.png)

**Percentage of Vine Reviews are 5-star:**  
For all the Vine Reviews, I found almost the same reviews, perhaps a little lower ratings than 5 Star.
**Percentage of Non-Vine Reviews are 5-star:** 
In General, the 5 star non-Vine reviews are higher than the Vine reviews.  
![pct5star](https://github.com/kushalishah/Amazon_Vine_Analysis/blob/main/Images/percent_5star_reviews.png)



