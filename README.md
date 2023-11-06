![credit card](https://github.com/dennerbocardi/card_categorizer/blob/main/images/credit_card.jpg)

# A categorizer for Credit Card Segment

## Overview
Banks engage in credit card segmentation to tailor their offerings to diverse customores needs and risk profiles. By categorizing customers based on their creditworthiness, spending habits, and financial behavior, banks can create trageted credit card products. This approach ensures that customers receive suitable credit limits, interest rates, rewards, and benefits, enhancing customer satisfactions and loyalty. Additionaly, segmentation allows banks tp manage risck effectively by aligning credit limits with individual repayment capacities, minimizing the likelihood of defaults and ensuring responsible lending practices. 

# The Problem
We need to build a categorizer to, given some financial and demographic information, we can set the client in its proper category. We have 4 caregories: "Blue", "Silver", "Gold" and "Platinum". Each one more demanding than the other, but also with more benefits and minor rates. We also have an unbalanced group that is the "Blue" category: 93% of the public is on that category. With that in mind we need to get a deeper look on how our model is fitting the customers, becouse if it fit everyone on the "Blue" category, some metrics (such as accuracy) will be high, for the model will fit right for most people, but it means that the model can only identify the "Blue" category and not the others. We will build a Confusion Matrix to evaluate that. 

## The dataset
This dataset is a fictional exemple. I get is on Kaggle, [here](https://www.kaggle.com/datasets/thedevastator/predicting-credit-card-customer-attrition-with-m)

## Approach
The approach I am assuming here is quite simple
- We load, explore and clean the dataset;
- We preprocees the dataset to perfmorm our models; 
- Test some different model approaches (KNN, XGBoost, and Neural Network);
- Build the confusion matrix for each model;
- Evaluate the mdodels;
- Save the most evaluated model;

At the end of the projec we must have a good cart categorizer. Right now the only model I built was the KNN, in a next update I will perfmorm and evaluate the XGBoost. 

## Project Struture
We have a preprocessing notebook to explore and clean the raw dataset. We save this cleaned dataset on the *'datasets'* folder as a *.csv* file, both of them in the *'src'* folder.<br>
On the *'src'* folder we also have the notebooks of the models we are building to solve this problem. 
```
card_caregorizer
├── src/     # the notebooks folder, where the models are stored
│  ├── datasets/   # folder where the datasets are stored
│  │  ├── bank_segmentation_data.csv # our raw dataset
│  │  └── preprocessed_dataset.csv # the clean dataset  
│  ├── preprocessing_data.ipynb # nootebook where we clean and explore the dataset
│  └── knn_estimator_for_card_category.ipynb # building our KNN model 
├── images / # folder with some images I might use (for aesthetic purposes only)
└── README.md # this file
```

## Lenguages and Tools
<p align="left">  <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a><a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/><a href="https://scikit-learn.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="scikit_learn" width="40" height="40"/> <a href="https://jupyter.org/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/3/38/Jupyter_logo.svg" alt="jupyter" width="40" height="40"/> </a> <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/> </a>

## Any doubts
Contact me
 - Email: denner.bocardi@gmail.com
 - LinkedIn: https://www.linkedin.com/in/dennersdenner/
