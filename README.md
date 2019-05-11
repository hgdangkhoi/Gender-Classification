# Gender-Classification

## Summary

This is the final project for CSC215 - Artificial Intelligence at California State University, Sacramento.

Gender prediction has become an essential in numerous applications such as image retrieval system, humancomputer interaction, biometrics, and especially, face recognition. Past researchers have shown that deep convolutional neural network (CNN) can predict a person’s gender from an input image with high accuracy. However, training a deep CNN model requires significant hardware power and long training time, which is not always available to researchers. 

In this project, I propose method of using supervised learning and autoencoder to extracts important features of the images before training. This approach saved significant training time, while only sacrifice 1-2% accuracy comparing to the best deep CNN model or transfer learning.

## Implementation
1. **Dataset**: The dataset used in this project is Labeled faces in the wild. They are available on sklearn library and the following link: http://vis-www.cs.umass.edu/lfw/

2. **Model and Methodology**: There are 4 main approaches in this project:
  - Base approach using Deep CNN model
  - Use a shallow CNN to extract features, then train using SVM, KNN, Random Forest
  - Use Autoencoder to extract features, then train using a shallow CNN
  - Transfer learning with VGG-16

## Result:
Approach of using pretrained model still exhibits the best performance and training time, however, the approaches in this project achieved close performance with only little longer training time. These results can be improved by using pretrain models or deeper autoencoder to extract features.

### Future Work:
- Modular the code for reproductivity
- Benchmark the model with Adience and IMDB-Wiki dataset
- Try Residual Network
