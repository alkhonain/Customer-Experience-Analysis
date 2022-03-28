# SDC Project
The project idea is predict the customer mode regarding to the reviews

## Dataset

Nearly 7,000 reviews scraped from yelp.com about Austin, Texas coffee shops, attributes replaced, sentiments around attributes.

Collect reviews on coffee shops from Yelp.com with a row for each review, and columns with the following data:

- Coffee shop name 
- Review text
- Review Score

## Pre-processing
Transfrom Review Score feature from charecter to two features, one is the number of rate(score) and the other is the Satisfaction which is descripe if the customer Satisfied with the service or not, which will be binary feature that contains 0 and 1.
<br><br>
Transform Review Text by cleaning the text form any value that will effict it such as numbers, punc, stopwords and URLs and apply all NLP process to the text to finally get a clean text. here is an example of how clean text will be:<br>
NOT clean text<br>
10/18/2016 I got food wasted at The Factory!!! Not your average coffee shop! Super social without internet, novel idea!<br>
Clean text<br>
got food wasted   factory   average coffee shop super social without internet novel idea


## Analysis
The process of analysis is first to classify the user if he is satisfied with the provided service or not by calculating the rate then, implement the NLP Process to anlysis the review text to clean one by renmoving any efficting to it.

then implement sentiment analysis, from that we notice the most used words as positive, negitive and the words in general.
<br><br><p align="center">
    <img src="pos_neg.png" alt="pos" style="height: 500px; width:500px;"/>
    <img src="words.png" alt="words" style="height: 500px; width:500px;"/>
</p><br><br>

## Model
The data set was imbalance so, implement over saimpling technique to solve this issue and we got a nice results with 75% accuracy 
<br><br><p align="center">
    <img src="model.png" alt="model" style="height: 500px; width:500px;"/>
</p><br><br>