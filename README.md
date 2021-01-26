## Problem Statement
Twitter has now become a useful way to build one's business as it helps in giving the brand a voice and a personality. The platform is also a quick, easy and inexpensive way to gain valuable insight from the desired audience. Identifying the sentiments about the product/brand can help the business take better actions.

You have with you evaluated tweets about multiple brands. The evaluators(random audience) were asked if the tweet expressed positive, negative, or no emotion towards a product/brand and labelled accordingly.


## Dataset Description
This dataset contains around 7k tweet text with the sentiment label.

The file train.csv has 3 columns

tweet_id - Unique id for tweets. tweet - Tweet about the brand/product sentiment - 0: Negative, 1: Neutral, 2: Positive, 3: Can't Tell

## Data Cleaning steps:
1. Drop tweet which has NaN value from the data.
2. Drop tweets which has sentiment value 3(Can't Tell) because these were not adding any value and count is very less(125)
3. Checking and converting the emoji into text
4. Encoding the text by removing the Non-ASCII characters
5. Removing #sxsw which is occurring the most and adding no value(sxsw is the name of the conference)
6. Extracting the top 10 frequent hastags in a DataFrame and displaying them in a bar chart
7. 



## Evaluation Metric
We will be using ‘weighted’ F1-measure as the evaluation metric for this competition
