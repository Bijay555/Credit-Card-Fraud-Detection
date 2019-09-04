# Credit-Card-Fraud-Detection
This project is about anomaly detection(also called outlier detection) through various techniques.
Python Packages in use: Numpy,Panda, sklearn,seaborn and matplotlib.

Few Anomaly Detection Techniques:
# 1. Local Outlier Factor:
      In anomaly detection, the local outlier factor (LOF) is an algorithm proposed by Markus M. Breunig, Hans-Peter Kriegel, Raymond T. Ng and Jörg Sander in 2000 for finding anomalous data points by measuring the local deviation of a given data point with respect to its neighbours.
      Local Outlier Factor (LOF) is a score that tells how likely a certain data point is an outlier/anomaly.

    LOF ≈1 ⇒ no outlier

    LOF ≫1 ⇒ outlier

First, I introduce a parameter k which is the number of neighbors the LOF calculation is considering. The LOF is a calculation that looks at the neighbors of a certain point to find out its density and compare this to the density of other points later on. Using a right number k isn’t straight forward. While a small k has a more local focus, i.e. looks only at nearby points, it is more erroneous when having much noise in the data. A large k, however, can miss local outliers.

# 2. Isolation Forest:
      One of the newest techniques to detect anomalies is called Isolation Forests. The algorithm is based on the fact that anomalies are data points that are few and different. As a result of these properties, anomalies are susceptible to a mechanism called isolation.

This method is highly useful and is fundamentally different from all existing methods. It introduces the use of isolation as a more effective and efficient means to detect anomalies than the commonly used basic distance and density measures. Moreover, this method is an algorithm with a low linear time complexity and a small memory requirement. It builds a good performing model with a small number of trees using small sub-samples of fixed size, regardless of the size of a data set.
 
# How Isolation Forests Work

The Isolation Forest algorithm isolates observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of the selected feature. The logic argument goes: isolating anomaly observations is easier because only a few conditions are needed to separate those cases from the normal observations. On the other hand, isolating normal observations require more conditions. Therefore, an anomaly score can be calculated as the number of conditions required to separate a given observation.

# The datasets for the Credit Card Fraud Detection is in the link below. Feel Free to Explore!!!!!
https://www.kaggle.com/mlg-ulb/creditcardfraud/kernels


# Happy Coding!!!!
