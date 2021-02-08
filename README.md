# Amazon Vine Analysis

Using PySpark our team sorted and filtered data from the AWS dataset to get the required dataframes by performing some calculations. The below tables are available in the Vine_Review_Analysis.ipynb file (link above)

1. vine_df : This DataFrame contains all the schema as required in pgAdmin table.
2. vote_count_df : This DataFrame has total_votes count equal to or greater than 20
3. voting_percent_df : This DataFrame has the number of Helpful Votes divided by Total Votes equal to or greater than 50%.
4. paid_reviews_df : This DataFrame has all the rows where a review was written as part of the Vine program (paid); unpaid_reviews_df : This DataFrame has all the rows where a review was written as part of the Vine program (unpaid)

## DataFrame Analysis
Using our created DataFrame, we can provide an analysis to the following questions:
1. How many Vine reviews and non-Vine reviews were there? - There are 3 Vine reviews and 3,094 non-Vine reviews.

<img src="https://github.com/jratliff1215/Amazon_Vine_Analysis/blob/main/images/Vine_Reviews.PNG" width="600" height="150">

<img src="https://github.com/jratliff1215/Amazon_Vine_Analysis/blob/main/images/NonVine_Reviews.PNG" width="600" height="150">


2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars? - There are 2 Vine reviews which are 5 stars and 1,704 non-Vine reviews which are 5 stars.

<img src="https://github.com/jratliff1215/Amazon_Vine_Analysis/blob/main/images/Vine_Five.PNG" width="650" height="150">

<img src="https://github.com/jratliff1215/Amazon_Vine_Analysis/blob/main/images/Nonvine_Five.PNG" width="650" height="150">

3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars? - 66.66 % of Vine reviews are 5 stars and 55.07 % percentage of non-Vine reviews are 5 stars.

<img src="https://github.com/jratliff1215/Amazon_Vine_Analysis/blob/main/images/Paid_Five.PNG" width="650" height="150">

<img src="https://github.com/jratliff1215/Amazon_Vine_Analysis/blob/main/images/NonPaid_Five.PNG" width="650" height="150">

## Is There Bias in the Data?

Overall, the results show no positivity bias for the Personal Care Applicances. Of the paid reviews, there were minimal compared to the overall dataset and not all paid reviews were 5 start reviews. A larger percentage of non-vine users were more critical of the products (45% non-five star reviews). However, these reviews are not verified and may not be product related. An additional datapoint that should be considred is why the review was critical. Was is a prodcut defect? Shipping delays? Many online reviwers can provide critial feedback not related to the actual product but to a service around the product. These types of reviews should be studied and likely eliminated. 
