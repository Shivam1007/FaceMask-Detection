# Face Mask Detection

## About Project: 
This project trains different Machine Learning models, including Convolutional Neural Networks to differentiate between images of people with and without masks. The MLP models manages to get the highest accuracy, 98.1% ,on the LDA transformed dataset. The dataset consists close ups of 2203 pictures of people with mask and 4500 pictures without masks. The models achieve high accuracies and are able to differentiate a picture, irrespective of the colour of the mask or the direction in which the person is facing in the picture.

## Preprocessing:  
All the images were then converted to gray scale. Then the images were resized to (64 x 64) and flatten to extract all the pixel values(features). The dataset was then randomly shuffled such that the whole dataset consists of randomnly spread images of people with mask and without mask.

## Dimensionality Reduction:
Two dimensionality reduction techniques were used: 1)LDA 2)PCA . Firstly, Standard Scaler was applied on the dataset and then the dimensionality reduction techniques were applied. Linear discriminant analysis (LDA) is a dimensionality reduction technique used to reduce the number of features to a more manageable number by minimizing the intraclass distances and maximizing the distances between different classes. Principal Component Analysis, or PCA, is a dimensionality-reduction method that is often used to reduce the dimensionality of large data sets.

## Training and Testing:
Three different classifiers are used to train the dataset and test it on the testing dataset to give accuracy, f1-score and logloss for LDA, PCA and Normal dataset. The three different classifiers used are: 1)SVC 2)MLP 3)Random Forest. For each classifier, each type of dataset was trained and testing was performed.

## Comparison:
The comparison for each type of dataset and for each type of classifier was also done with the help of cross validation scores and corresponding boxplots were plotted.

## Additional Classifiers:
Convolutional Neural Network (MobileNetV2): 
MobileNetV2 is a convolutional neural network architecture that seeks to perform well on mobile devices. It is based on an inverted residual structure where the residual connections are between the bottleneck layers. Its hyperparameters were varied and were finally decided as follows:
1) Learning Rate: 1e-4
2) Epochs: 20
3) Batch Size = 32
One hot encoding was performed on the labels and the data was then split into training and testing.

## Team Members:
1) Shivam Sharma (B19CSE084)
2) Shubh Doshi (B19EE080)
