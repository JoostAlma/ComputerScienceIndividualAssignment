
# README

This project is an assignment for the MSc Econometrics course "Computer Science For Business Analytics (FEM21037)" from the Erasmus University of Rotterdam.
The project takes a close look at duplicate detection using data from the file "TVs-all-merged.json" containing information of 1624 online advertisements for televisions. The data is pre-processed using Locality-Sensitive Hashing (LSH) to reduce the number of comparisons to be made. The Jaccard- and cosine-similarity measures are used to compute the similarity between the titles of products, using model words to represent the titles as binary vectors.


The Python code in this github is structured as follows:

First, the data in imported and added to a list.
Next, two functions are depicted, "textfunc2" for text processing/cleaning purposes and "randomNumberGenerator" for minhashing.
Then the function "fulltransformation" takes as input the (x and y) data to be used, the number of bands and rows for LSH and the threshold for the Jaccard- and cosine-similarity calculations and returns the performance measures for LSH as well as for classification.


The "fulltransformations" function operates in the following order: 
Data transformation and normalization, model words, inputmatrix, minhashing, signaturematrix, constructing bands/rows, extracting candidatepairs, performing similarity measures and overall performance.

Finally, bootstrap is used to obtain robust estimates of all performance measures. The bootstrapped performance measures are averaged and plotted in different graphs. 


Joost Alma
