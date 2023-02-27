# Fine tuning a BERT network for sentiment analysis of Reddit comments



#The comments
The data was collected using the reddit api from commonts on 9 different reddit posts, of varying topics.

We can see how the model performs on the test data with the confusion matrix below here 0,1,2,3 correspond to neutral,positive,negative,amibguous respectively. 
The model performs with an F1 score of 0.69, which is around the baseline performance introduced in the paper; this could likely be improved slightly via optimization of the parameters. 
![image](https://user-images.githubusercontent.com/60330103/221457172-ffef0820-281d-45ce-85dd-c2302c1fb4b1.png)
We can see from this that neutral state








#What can we see from the model's predictions

As one might predict the comments on a post of a a cat are largely positive, whereas posts concering controversial topic matters seem to in general result in a more negative sentiment in general. We can see this from the median sentiment, most common sentiment, and also the average sentiment.


We can see the distribution of the median sentiment on the bar-chart below
![image](https://user-images.githubusercontent.com/60330103/221458671-a88aded3-d6f0-42ed-9163-9957fcb92da6.png)
