# Skin-color extraction and classification
This programm allow you to extract skin color from face and classify it to the arbitraty number of clusters

## The pipeline of my method may be divided into four primary segments: 
* 1) Face detection - obtaining bounding box around the face.
* 2) Apply k-Means Clustering to the face on the HSV color space to obtain the most dominant color which is assumed to be the skin color. 
* 3) The center of the prevalent cluster would represent the color of a person. So, I collect those colors for a set of images (~ 20k+ using UTKFace dataset).
* 4) After this I apply k-Means clustering algorithm to the set of collected colors and look for an optimal number of clusters that would give a meaningful result.

## Project structure
Project consist of 2 jupyter notebooks.
1) Data downloading & preprocessing & color extraction algoritm
2) Data analysis and conclusions

## Results 
![Example of color classification using K-means](https://raw.githubusercontent.com/Nikolaytv/Skin_color_classifier/master/Result.jpg)
