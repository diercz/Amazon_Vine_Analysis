# Amazon_Vine_Analysis

## Overview

Amazon Vine Program is a service that allows companies to receive reviews for their products.  Companies such as SellBy pay a small fee to Amazon and provide prodcuts to Amazon Vine members, who are then required to publish a review.  Within this project I chose to use *US Apparel* product reviews from Amazon to determine if there is any positivity bias in reviews written by members of the paid Amazon Vine program.  

## Resources
- Datasets
    - [US Apparel dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

- Technology Utilized
    - Google Colab
    - Postgres SQL
    - AWS, S3, and RDS

### Results

I filtered the dataset down to reviews with more than twenty votes, to focus our analysis on the most popular reviews.  I then filtered the results to those who received a helpful rating greater than or equal to 50%.  This filtered our total number of reviews to 42,452 from our dataset.

![webpage](https://github.com/diercz/Amazon_Vine_Analysis/blob/main/Images/Helful%20Rate.png)

Of the helpul reviews, only 30 are *Paid Vine Program* reviews.  With *Non-Vine* reviews making up 42,422 of the dataset.

![webpage](https://github.com/diercz/Amazon_Vine_Analysis/blob/main/Images/vine_yes.png)

![webpage](https://github.com/diercz/Amazon_Vine_Analysis/blob/main/Images/vine_no.png)

Within our dataset, there are a total of 22,473 *5-Star* reviews, accounting for 53% of reviews.

![webpage](https://github.com/diercz/Amazon_Vine_Analysis/blob/main/Images/5_star_count.png)

Of the *Vine* reviews, 44.67% were 5-Star, while 52.42% of the of *Non_Vine* 5-Stars.

![webpage](https://github.com/diercz/Amazon_Vine_Analysis/blob/main/Images/5_star_percent.png)

- Paid Vine Program
    - 30 total Reviews
    - 14 were 5-Stars
    - 46.67% of Vine reviews were 5-Star

- Unpaid Reviews
    - 42,452 total reviews
    - 22,733 5-star review
    - 52.42% of unpaid reviews were 5-Star

## Summary 

In review, there is no evidence to suggest that the vine reviews contain any bias.  As shown above, only 30 total reviews came from the Vine Program and only about half were 5-Star rated (46.67%).  Similarly, the Non-Vine reviews resulted in a little over half being 5-Star reviews (52.42%).  The Vine Program may not be worth it for an apparel company and is already not very popular with the results that I reviewed. I would advise an apparel company to invest in the Vine Program as it does not appear to incentivize individuals to write a better review of the product.  

In conclusion on this analysis customers do not feel a positivity bias for leaving a good review in the Vine Program as there was a limited amount and not so many well rated.  I did further analysis to calculate the average of the star ratings on each programs reviews to identify if there is any difference.  Vine Review avg rating was 4.09, while Non-Vine reviews averaged 3.87.  This shows there is still not a lot of incentive to to enroll in the Vine program.  For further analysis we could review the actual words used in each review.  This way we could see if Vine reviews are more indepth and detailed regarding the product vs Non-Vine members.  