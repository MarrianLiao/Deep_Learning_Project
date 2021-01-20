# Deep Learning Project
The purpose of our project is to help local business and government monitor people wearig mask or not during this pandemic.
In this project, we scrapped 1400+ images with people with or without masks from Google image using open-source Github repository and Google extension Imageye,
and performed data preprocessing by rescaling the image and splitting it into training set and test set. 

Then, we build 3 Convolutional neural networks model. 
Since we only have 453 pictures with masks and 974 pictures without masks, we use data augmentation in order to enlarge our dataset and avoid overfitting. 
By using this method, the accuarcy of a classification model has significant improvement. We build two CNN with pre-trained convolution base - MobileNetV2. 
The first pre-trained model includes drop-out in its fully-connected layer. The second pre-trained model's fully-connected drop-out was removed and we introduced early-stopping.


The best model is the second model with highest accuracy on validation and better confusion matrix.
The notebook file is MaskvsNoMask.ipynb, the data is in the Datasets folder, and the image scrapping code is in No limit Image downloads.ipynb.
