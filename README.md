# A categorizer for Credit Card Segment
Today on most banks we have some credit card categories. Those categories define some benefits to the customers. In general, the most popular category has no benefits at all, but once the categories are getting less popular the benefits are getting better.<p>

The problem we have here is trying to determine which category we should put a person in, given some financial and demographic data. We need to build a good categorizer to make our model accurate and to be sure that the model understands all the categories and not put everyone on the most popular one. 

I already tried to solve our problem clusterizing the clients with KNN, but, although it had great accuracy, the problem is that the model set almost everyone to the most popular category, which represents 93% of our database. I.e., the model is just smart because the database is unbalanced. We need to get better results.

The next step is to build a deep neural network to see how it performs to solve the problem. 

Follow me to get updated when I try the new approach.  

# Project Struture
We have a preprocessing notebook to explore and clean the raw dataset. We save this cleaned dataset on the *'datasets'* folder as a *.csv* file, both of them in the *'notebooks'* folder.<br>
On the *'notebooks'* folder we also have the notebooks of the models we are building to solve this problem. 
'''
card_caregorizer
├──notebooks/     # the notebooks folder, where the models are stored
│  ├──datasets/   # folder where the datasets are stored
│  │  ├──bank_segmentation_data.csv # our raw dataset
│  │  └──preprocessed_dataset.csv # the clean dataset  
│  ├──preprocessing_data.ipynb # nootebook where we clean and explore the dataset
│  └──knn_estimator_for_card_category.ipynb # building our KNN model 
└──README.md # this file
'''

# Any doubts

- Denner Bocardi: denner.bocardi@gmail.com