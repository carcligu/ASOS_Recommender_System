# Data Science Festival X ASOS
## Data Science Festival Workshop 7 November 2020 – Building a fashion recommender using Tensorflow/Keras with ASOS.

This repo has been developed following the session on the Data Science Festival by ASOS. 

## Learning to Rank

The aim is to build a recommender system based on ranking products. This rank can be created in different ways: 

* in a personalised way based on old purchases from the customer
* rank products in relation to each other, trying to find similar products

Asos has tens of thousend of products and tens of millions of users, and deep learning will be used. 

For each customer, we are going to give a score to every product, and then we will rank the producs, so the ones with the higher score will be shown first. 

We will build this model with something called **matrix factorization**. For every user and for every product, we will come up with a list of random numbers. We will multiple this number and sum them: 

First number of the user vector gets multipled for the first number on product vector, and so on, and we get a final score. We can now if the model is doing a good job if it is ranking is placing first products that the customer has bought. 

As we start this process with random numbers, intially the model will make terrible mistake, and probably will rank at the end products that the customer has bought. In that case, the model will change the random weights given when initializing the model. 
