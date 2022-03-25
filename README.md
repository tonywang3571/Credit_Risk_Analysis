# Credit_Risk_Analysis

## Overview of Project  

**Purpose:**  
The purpose of this project is to perform 
## Resources:  
- Data Source: [US Reviews Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)  
- Software: Anaconda 4.10.3, Python 3.9.7, Jupyter Notebook 6.4.5, scikit-learn 0.24.2  






## Analysis and Results  

**Analysis:**  
For this project, I chose to use the shoes dataset to perform my analysis. I loaded the dataset into Colab and extracted data into 4 different dataframes, customer_id, products_df, review_id_df, and vine_df. After extracting the dataframes, I used AWS to create and connect a server to pgAdmin to load my dataframes into a SQL database. Next, I used the vines dataframe to preform calculations to see if there are any bias of paid and unpaid reviews based on 5-star rated reviews and total votes. I also calculated percent of the votes being 5-star rated.  

**Results:**  
**Vine Reviews (paid)**  
- total vine reviews = 22  
- 5-star reviews = 13  
- % of 5-star reviews = 59.09%  

**Non-Vine Reviews (unpaid)**  
- total vine reviews = 26987  
- 5-star reviews = 14475  
- % of 5-star reviews = 53.64%  

## Summary  

**Conclusion**  
The purpose of this project is to perfrom an analysis on an Amazon product dataset to determine if there are any bias for paid and unpaid reviews. According to our results, we can see that there are very minimal number of paid reviews compared to unpaid reviews that are rated 5-stars. The percentage of reviews are also very similar to each other, even though the quantity of 5-star reviews differ by so much. I would think that if there are any bias within the Amazon Vine Program, there would be greater number of 5-star reviews so consumers would be more willing to purchase those products. Another analysis I would perform would be the same calculations with combined 4 and 5 star reviews because 4 and 5 star reviews are still positive and can sway consumers to purchase those products.  

### Codes Used  
(Please look at specific files for codes used)  
Code for [creating the four tables](https://github.com/tonywang3571/Amanzon_Vine_Analysis/blob/master/Amazon_Reviews_ETL.ipynb)  
(NOTE: Error did occur when creating review_id_table due to data already loaded into SQL database)  
Code for [vine_review calculations](https://github.com/tonywang3571/Amanzon_Vine_Analysis/blob/master/Vine_Review_Analysis.ipynb)  
