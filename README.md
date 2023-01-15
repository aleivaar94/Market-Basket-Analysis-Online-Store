![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

# Market Basket Analysis - Online Store

The best way to keep clients is to have personalized offers. One way of using data analysis to provide personalized offerings in by association analysis, to finds patterns of items in large data sets. Association analysis is relatively lightweight on math, easy to implement and powerful to find insights. Market basket analysis is a type of association analysis which can be very useful in e-commerce such as finding unexpected purchasing patterns like buying beer and diapers in the same grocery errand. 

In this project I analyze an online retail [data set](http://archive.ics.uci.edu/ml/datasets/Online+Retail) to obtain insights of purchase combinations. The data contain transactions from a UK retailer between 2010-2011.

![image](https://github.com/aleivaar94/Market-Basket-Analysis-Online-Store/blob/master/images/shopping-cart.png)

# Methodology

- The [Apriori algorithm](http://rasbt.github.io/mlxtend/user_guide/frequent_patterns/apriori/) from the [MLxtend](http://rasbt.github.io/mlxtend/) library was used to generate the association rules and to also calculate support, confidence and lift.
    - Individual items need to be 1-hot encoded to analyze using the Apriori algorighm. Null values are replaced with 0.

# Results

This online store had most sales in the UK, although this online sotre shipped other countries in Europe and South East Asia.

Sales significantly increase in August, reaching peak in mid November and dropping dramatically in December and the first three months of the new year.

Combination of items purchased differ between different countries. Customers from Germany prefer to buy items other than lunchboxes, like different kinds of plasters. Consumers from The Netherlands buy different types of lunchboxes together, so we can make sure that customers that are browsing for lunchboxes are have lunchboxes in their cart, get offered more lunchboxes options.