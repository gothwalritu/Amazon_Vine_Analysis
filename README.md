
### Module 16

# Amazon_Vine_Analysis

In this module I learnt the following:

•	First, I learnt what is the big data, about the four Vs, big data related problems and the related technologies to handle big data.
•	I learnt about the Hadoop, and its three main components: Hadoop Distributed File System (HDFS), MapReduce, Yet Another Negotiator (YARN)
•	I learnt about the key features and architecture of Spark and compared the Spark with Hadoop. 
•	I learnt about the Google Colab Notebooks, and created an account there to work on this project. I installed PySpark package for libraries which I wanted to use. Also, created session by importing the library and setting the “spark” variable.
•	I learnt about the Spark DataFrames and Data sets, Spark Functions, Natural Language Processing and its core concepts.
•	I learnt to use AWS Simple Storage Service (S3) and relational databases for basic cloud storage. 

## Overview of the project:  

In this project I am analyzing Amazon reviews written by members of the paid Amazon Vine program. I choose the dataset related to the reviews of video games and performed the ETL process using PySpark, to extract and transform the dataset. The dataset was connected to an AWS RDS instance and loaded the transformed data into pgAdmin. 

In the analysis of review, I picked only the rows which had equal to or greater than 20 total reviews. Then, I selected only those rows which had equal to or greater than 50 percent of the helpful_votes over total_votes. Afterwards, I separated the paid reviews from the unpaid reviews. I did the total  counts of paid and unpaid reviews. I also counted the number of reviews for paid and unpaid, which had five star rating and calculated its percentage against the totals of the respective class.

## Results: 

#### Vine reviews and non-Vine reviews:

![Picture_1](https://github.com/gothwalritu/Amazon_Vine_Analysis/blob/main/Scrnshots/result_1.png)

![Picture_1](https://github.com/gothwalritu/Amazon_Vine_Analysis/blob/main/Scrnshots/results_2.png)


### Vine reviews with 5 stars and non-Vine reviews with 5 stars:

![Picture_1](https://github.com/gothwalritu/Amazon_Vine_Analysis/blob/main/Scrnshots/result_3.png)

![Picture_1](https://github.com/gothwalritu/Amazon_Vine_Analysis/blob/main/Scrnshots/result_4.png)


### Percentage of Vine reviews with 5 stars and percentage of non-Vine reviews with 5 stars:

![Picture_1](https://github.com/gothwalritu/Amazon_Vine_Analysis/blob/main/Scrnshots/result_6.png)

![Picture_1](https://github.com/gothwalritu/Amazon_Vine_Analysis/blob/main/Scrnshots/result_5.png)


## Summary: 

The results showed that the percentage of reviews with five-star rating for paid and unpaid are approximately 51 and 38 respectively, but the sample size for paid reviews are significantly smaller than the unpaid reviews. Hence, it looks like that the paid reviews are positively biased. I chose only those rows which had equal or more than 20 total reviews. However, to increase the sample size of reviews with five-star ratings especially for paid reviews, I could have reduced this limit from 20 to some less number. I could also have performed the statistical distribution with mean, mode, medians for both paid and unpaid reviews to get more accurate results for this project.

