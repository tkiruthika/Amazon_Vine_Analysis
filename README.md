# Amazon_Vine_Analysis

## Overview

The overview of this module is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

## Purpose

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

## Results

### Deliverable 1

  - Using the knowledge of the cloud ETL process, create an AWS RDS database with tables in pgAdmin, pick a dataset from the Amazon Review datasets (Links to an external site.), and extract the dataset into a DataFrame.
  - Transform the DataFrame into four separate DataFrames that match the table schema in pgAdmin.
  - Upload the transformed data into the appropriate tables and run queries in pgAdmin to confirm that the data has been uploaded.

  **The customers_table DataFrame**

![1](https://user-images.githubusercontent.com/95719819/164983474-5b9ab199-9491-4172-ae2a-f9f05144de90.png)

  **The products_table DataFrame**

![2](https://user-images.githubusercontent.com/95719819/164983481-18e5aedd-d7f4-4646-b33c-6985f94f6111.png)

  **The review_id_table DataFrame**

![3](https://user-images.githubusercontent.com/95719819/164983494-63b60c6f-a21f-4640-9efe-21072d537f37.png)

  **The vine_table DataFrame**

![4](https://user-images.githubusercontent.com/95719819/164983500-d753b27a-60ec-439c-9aa3-1c733cbe12ba.png)

  **Tables are created in pgAdmin and the dataframes are loaded to the corresponding tables**
  
  ![1](https://user-images.githubusercontent.com/95719819/165000406-121ecfec-39e5-4fe8-b8f7-dbdee3828c5b.png)


### Deliverable 2

  - Using PySpark, determine if there is any bias towards reviews that were written as part of the Vine program. 
  - For this analysis, determine if having a paid Vine review makes a difference in the percentage of 5-star reviews.

  **How many Vine reviews and non-Vine reviews were there?**

  ![1](https://user-images.githubusercontent.com/95719819/164982888-27664039-4b0f-485b-9545-4f7a4a883e1f.png)

  **How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?**

  ![2](https://user-images.githubusercontent.com/95719819/164982901-178f08a6-4e22-420c-96c6-5c4edcf9b13b.png)
  
  **What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?**
  
  ![3](https://user-images.githubusercontent.com/95719819/164982910-05972262-058e-4689-bcb8-4d5af9d4b719.png)

## Summary

  - From our analysis we can see there is bias in the reviews of paid and unpaid Vine reviewers as the difference in the percentage of the 5-star reviews of paid and unpaid is 7.33923.(54.411765-47.072535=7.33923).
  - Also, the overall percentage of reviews for paid and unpaid are 0.017169 and 2.274802 respectively. So, it proves that there is bias in the reviews that were written as part of the Vine program.
  
  ![1](https://user-images.githubusercontent.com/95719819/164985998-de6891e8-9792-44fc-a25e-f4bb1cf1b2b3.png)
