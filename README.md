# Texture_Classification
 
 The goal of this project is to train a learning model to determine the category of the texture of a given surface image.
 
 The idea is to use a filter bank called LM filters, which are 48 filters that operates as calculating changing in values in 48 different ways for a given pixel. Then we would apply K-Means to find K features (bag of words) and calculates the frequency of appearance of each feature in each images. We will use this length K vector to represent each images. We then choose an appropriate classification model to assign each new image a label based on our results from training and validation set.
 
 One difficulty to note for this project is the size of the data. If we work with the original data, after we apply all 48 filters, we would have large data which is of size 325 GB that would kill our kernel. Hence, we will first resample the pixels we are working with.
 
 More details are in Writeup.PDF
 
 