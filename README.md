# Fine tuning a BERT network for sentiment analysis of Reddit comments


# the GoEmotions dataset
In order to fine tune a network for sentiment analysis, we first need some suitable data. The GoEmotions set was published in [1], and consists of 58000 manually annotated english comments collected from Reddi, and labelled into one of 28 categories. From these categories we can also format the data into positive, negative, ambiguous and neutral samples, and use these to fine tune a network for analysing comments. 

# The data for analysis 
The data was collected using the reddit api from comments on 9 different reddit posts, of varying topics.


# The model

We can see how the model performs on the test data with the confusion matrix below here 0,1,2,3 correspond to neutral,positive,negative,ambiguous respectively. 
The model performs with an F1 score of 0.69, which is around the baseline performance introduced in the paper; this could likely be improved slightly via optimization of the parameters. 
![image](https://user-images.githubusercontent.com/60330103/221457172-ffef0820-281d-45ce-85dd-c2302c1fb4b1.png)






#What can we see from the model's predictions

As one might predict the comments on a post of a a cat are largely positive, whereas posts concering controversial topic matters seem to in general result in a more negative sentiment in general. We can see this from the median sentiment, most common sentiment, and also the average sentiment.


We can see the distribution of the median sentiment on the bar-chart below
![image](https://user-images.githubusercontent.com/60330103/221458671-a88aded3-d6f0-42ed-9163-9957fcb92da6.png)


#Conclusions
Although in general most of the comments were returned as neutral, we can see the network works well enough to get the general sentiment. Comments that would be expected to get negative comments, comments on posts related to the war in ukraine were in general negative in sentiment, whereas comments on a post of a picture of a cat were in general positive. 
# References
[1] https://arxiv.org/abs/2005.00547
[2] https://praw.readthedocs.io/en/stable/code_overview/reddit_instance.html
[3]
