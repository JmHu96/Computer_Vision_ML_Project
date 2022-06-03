# Texture_Classification
 
The goal of this project is to train a learning model to determine the category of the texture of a given surface image.
 
The idea is to use a filter bank called LM filters, which are 48 filters that operate as calculating changing in values in 48 different ways for a given pixel. Then we apply K-Means to find K features (bag of words) and calculate the frequency of appearance of each feature in each image. We will use length K vector to represent each image. We then choose an appropriate classification method to assign each new image a label based on our results from training set and validation set.
 
One difficulty to note for this project is the size of the data. If we work with the original data, after we apply all 48 filters on all pixels with convolution, we would have a large data set which is of size 325 GB. If we choose to work with the all pixels without resampling, a data with this size could easily kill our kernel unless one is using a super computer. Hence, we will first resample the pixels we are working with. I ended up choosing pixels with a gap of 5 along both x-axis and y-axis in all images, i.e. choosing the most top left pixel in a 5 x 5 grid, which reduces the data size to 4\% of its original size.
 
More details are in Writeup.PDF
 
 