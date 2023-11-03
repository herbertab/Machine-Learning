# Food Clustering and Classification

## Dataset
The dataset used in this project is a collection of foods and their nutritional compositions, available on [Kaggle](https://www.kaggle.com/shrutisaxena/food-nutrition-dataset). Each food item in the dataset is accompanied by detailed information about its macronutrient and micronutrient content.

The primary objective of this project is to perform unsupervised clustering of foods to identify groups of foods with similar characteristics. This approach can be valuable for creating personalized diets, allowing for the substitution of foods with equivalent nutritional attributes.

## Clustering Technique: K-means
To carry out unsupervised clustering of foods, we utilized the K-means algorithm. K-means is a technique that partitions a dataset into K clusters based on the similarity of attribute values.

The choice of the ideal K value was determined using the silhouette metric, and the results indicated that the best division of the dataset occurs in 3 distinct groups.

## Classification Technique: Decision Tree
After grouping foods into clusters, we added a column to the dataset to indicate the group to which each food item belongs. This enabled us to prepare the data for building a Decision Tree. A Decision Tree is an intuitive and straightforward machine learning technique, making it accessible even to individuals with limited knowledge of machine learning.

## Results
Results obtained with the K-means algorithm showed silhouette scores of 0.52 for K=2, 0.54 for K=3, and 0.37 for K=4. Based on these results, we decided to divide the dataset into 3 distinct groups.

The Decision Tree exhibited a training and testing accuracy of 99.9%, indicating that the algorithm identified patterns in the data consistent with the groups defined by K-means. The final tree had 6 levels and 20 leaves, with the "Data.Water" attribute being the most important, followed by the "Data.Carbohydrate" attribute, responsible for classifying 94.3% of the data.

This project provides a comprehensive approach to clustering foods based on their nutritional compositions. The classification method was used to confirm that the clusters are predictable wich means that the algorithm identified good patterns in the dataset, offering valuable insights for dietary planning and more informed food choices.
