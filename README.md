# Amazon_Vine_Analysis

## Overview

Amazon Vine Program is a service that allows companies to receive reviews for their products.  Companies such as SellBy pay a small fee to Amazon and provide prodcuts to Amazon Vine members, who are then required to publish a review.  Within this project I chose to use *US Apparel* product reviews from Amazon to determine if there is any positivity bias in review written by members of the paid Amazon Vine program.  

## Resources
- Datasets
    - [US Apparel dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

- Technology Utilized
 - Google Colab
 - Postgres SQL
 - AWS, S3, and RDS

### Results

I filtered the dataset down to reviews with more than twenty votes, to focus our analysis on the most popular reviews.  I then filtered the results to those who received a helpful rating greater than or equal to 50%.  This filtered our total number of reviews to 42,452 from our dataset.

![webpage](helpful rate)

Of the helpul reviews, only 30 are *Paid Vine Program* reviews.  With *Non-Vine* reviews making up 42,422 of the dataset.

![webpage](vine_yes)

![webpage](vine_no)

Within our dataset, there are a total of 22,473 *5-Star* reviews, accounting for 53% of reviews.

![webpage](5_star_count)

Of the *Vine* reviews, 44.67% were 5-Star while 52.42% of the of *Non_Vine* 5-Stars.

![webpage](5_star_percent)

- Paid Vine Program
    - 30 total Reviews
    - 14 were 5-Stars
    - 46.67% of Vine reviews were 5-Star

- Unpaid Reviews
    - 42,452 total reviews
    - 22,733 5-star review
    - 52.42% of unpaid reviews were 5-Star

## Summary 