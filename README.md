# Amazon_Vine_Analysis

## Overview of Analysis:
Client requested an analysis of Amazon reviews from the Video Games category. Specifically, an analysis comparing reviews published via the Vine program vs those that were not. The source data linked below was broken into four separate tables in Colaboratory and then uploaded to an AWS RDS server via pgAdmin. It was then requested that the table containing information on review id, vine status, star rating, helpful votes, total votes, and verified purchases be exported into a csv file and analyzed in Jupyter Notebook. 

## Resources
- Source Data: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Video_Games_v1_00.tsv.gz
- Software: Colaboratory, pgAdmin4, PostgreSQL 14, Python 3.10 (64-bit), Jupyter Notebook 6.4.8, AWS 

## Results

- There were 90 Vine reviews and 37385 non-Vine reviews.

- There were 44 5-Star Vine review and 14626 5-star non-Vine reviews.

- 49% of the Vine reviews were 5-star and 39% of the non-Vine reviews were 5-star.

<p align="center">
  <img src="https://github.com/justinkirk8/Amazon_Vine_Analysis/blob/main/images/Vine_stats.png" width="300" /><space>
  <img src="https://github.com/justinkirk8/Amazon_Vine_Analysis/blob/main/images/non_Vine_stats.png" width="300" />
</p>

## Summary

From the results of the requested analysis, there appears to be a positivity bias for reviews in the Vine Program due to the Vine program having 10% more 5-star reviews. However, this along does not provide much statistical weight. An additional analysis that could be done is a t-test to determine if there is a statistical difference between the distributions of star reviews between the Vine reviews and the non-Vine reviews. This shows that there is a significant difference between the distributions. 
  
<p align="center">
  <img src="https://github.com/justinkirk8/Amazon_Vine_Analysis/blob/main/images/t_test.png" width="700" />
</p>


