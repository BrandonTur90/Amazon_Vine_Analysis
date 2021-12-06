# Amazon Vine Analysis

## Purpose

The purpose of this analysis was to use AWS, SQL, and PySpark to import a set of watch reviews from Amazon,
organize them into dataframes, export them to SQL, and then run a series of analysis using PySpark.

## Results

After the initial organizing of the data, several questions needed to be answered:

* How many of the reviews were part of the Vine program of paid reviews? How many were not?

![vine_df_y](/images/vine_df_y.PNG)

![vine_df_n](/images/vine_df_n.PNG)

There were a total number of 8,409 watch reviews. 47 of which were Vine (paid) reviews, the 
remaining 8,362 were non-Vine reviews.

* How many Vine reviews were 5 stars?

![five_star_y](/images/five_star_y.PNG)

There were a total of 15 Vine reviews that were 5 stars.

* How many non-Vine reviews were 5 stars?

![five_star_n](/images/five_star_n.PNG)

And there were 4,332 unpaid 5 star reviews.

* Finally, what percentage of Vine reviews were 5 stars, and what percentage of non-Vine reviews were 5 stars?

![percent](/images/percent.PNG)

The percentage of paid 5 star reveiews was 32%, whereas the percentage of non-vine 5 star reviews was 48%

## Conclusion

According to the data, it seems that the Vine program doesn't lead to an increase in 5 star reviews, actually
it could lead to the opposite. It should be noted that the data for Vine reviews is incredibly small, only 
47 out of 8,409 reviews were Vine reviews. The other problem is that all the 5 star Vine reviews weren't 
verified purchases according to the data. If this is an oversight on how Vine reviews are done, or if a
Vine review can be submitted without a verified purchase, it needs to be corrected or accounted for 
for future analysis to be accurate.