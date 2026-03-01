# Discussion and Conclusion

Dataset: CIFAR-10 dataset has 10 labels and 60K images of 3x32x32
3 channel, 32 width, 32 height. in pixel

Neural Network We are using 3x32x32 = 3072 features as input 
The output is 10 classes
        
In simple NN we loose the spatial information since we flatten the image
The BatchNormal is used to reduce computation time using the current batch
Droupout is used to prevent overfitting by cutting off impact of some neurons

Here We implement the AlexNet architecture for CIFAR-10 dataset
We are using 3x32x32 2d images as input
There are 8 layers in total
There are 5 layers of convolution and 3 layers of fully connected
2 max pool layer within the 5 Convolutional layers to reduce the size of the data
This architecture is a copy of the AlexNet architecture as provided in the resource

Tiny VGG
There are 2 Convolution blocks with a max pooling for both with 2 Convolutional layers.
and a pooling layer then there are two fully connected layers completing the tiny VGG architecture

## Prediction
The Simple NN should do the worst since it loses dimentionality and brute forces the computation
The Tiny VGG and AlexNet should work much better. 
In comparision Tiny VGG should be lightweight but AlexNet performance should be better

# The metrics

1. Accuracy
Fraction of correctly predicted samples out of all samples.
Overall performance of the model. High accuracy does not always mean good performance for imbalanced classes.
Formula: Num of Correct Predictions/ Total Predctions 

2. Precision
Measures correctness of positive predictions. High precision = model rarely labels something as a class incorrectly.
Formula (per class): TP/ TP + FP

3. Recall (Sensitivity)
Out of all actual samples of a class, how many were correctly identified by the model.
Measures completeness. High recall = model detects most of the actual class instances.
Formula (per class): TP / TP + FN

4. F1-Score
Harmonic mean of precision and recall.
Balances precision and recall. Useful when you want a single metric for class performance, especially in imbalanced datasets.
Formula: 2 (Precision * Rceall)/(Precison + Recall)

5. Confusion Matrix (CM)
A table showing actual vs predicted classes.
Structure:

# Results 

