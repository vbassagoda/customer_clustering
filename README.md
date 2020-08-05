# Creating Customer Segments

## Dataset
The dataset includes product spending data collected for customers of a wholesale distributor in Lisbon, Portugal.

1) `Fresh`: annual spending on fresh products (Continuous); 
2) `Milk`: annual spending on milk products (Continuous); 
3) `Grocery`: annual spending on grocery products (Continuous); 
4) `Frozen`: annual spending on frozen products (Continuous);
5) `Detergents_Paper`: annual spending on detergents and paper products (Continuous);
6) `Delicatessen`: annual spending on and delicatessen products (Continuous); 
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)
8) `Region`: {Lisbon - 1, Oporto - 2, or Other - 3} (Nominal)
More information can be found in https://archive.ics.uci.edu/ml/datasets/Wholesale+customers. 

## Project Overview
I will first explore the data by selecting a small subset to sample and determine if any product categories highly correlate with one another. Afterwards, preprocess the data by scaling each product category and then identifying (and removing) unwanted outliers. With the clean customer spending data, I will apply PCA transformations to the data and implement clustering algorithms to segment the transformed customer data. Finally, I compare the segmentation found with an additional labeling and consider ways this information could assist the wholesale distributor with future service changes.

## Motivation for the project
A wholesale distributor recently tested a change to their delivery method for some customers, by moving from a morning delivery service five days a week to a cheaper evening delivery service three days a week. Initial testing did not discover any significant unsatisfactory results, so they implemented the cheaper option for all customers. Almost immediately, the distributor began getting complaints about the delivery service change and customers were canceling deliveries, losing the distributor more money than what was being saved. I aim to find what types of customers they have to help them make better, more informed business decisions in the future. I used unsupervised learning techniques to see if any similarities exist between customers, and how to best segment customers into distinct categories.

## Software and Libraries
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [matplotlib](http://matplotlib.org/)
- [Jupyter Notebook](http://ipython.org/notebook.html)
- [Python 2.7](https://www.python.org/download/releases/2.7/)

Please note that this is an old project and that's why it uses python 2.7.

## How to run it
virtualenv --no-site-packages -p /usr/bin/python2.7 .env
source .env/bin/activate
pip install requirements.txt