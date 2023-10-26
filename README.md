# A categorizer for Credit Card Segment
Today on most banks we have some credit card categories. Those categories define some benefits to the customers. In general, the most popular category has no benefits at all, but once the categories are getting less popular the benefits are getting better.<p>

The problem we have here is trying to determine which category we should put a person in, given some financial and demographic data. We need to build a good categorizer to make our model accurate and to be sure that the model understands all the categories and not put everyone on the most popular one. 

I already tried to solve our problem clusterizing the clients with KNN, but, although it had great accuracy, the problem is that the model set almost everyone to the most popular category, which represents 93% of our database. I.e., the model is just smart because the database is unbalanced. We need to get better results.

The next step is to build a deep neural network to see how it performs to solve the problem. 

Follow me to get updated when I try the new approach.  

# Any doubts

- Denner Bocardi: denner.bocardi@gmail.com