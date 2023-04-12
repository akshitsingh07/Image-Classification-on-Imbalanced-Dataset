# Image-Classification-on-Imbalanced-Dataset
Image Classification on Imbalanced Dataset
Image classification can be performed on an Imbalanced dataset, but it requires additional considerations when calculating performance metrics like accuracy, recall, F1 score, AUC, and ROC.

When the dataset is Imbalanced, meaning that one class has significantly more samples than the others, accuracy alone may not be a reliable metric for evaluating the performance of the model. Instead, we need to consider other metrics such as recall, precision, F1 score, AUC, and ROC.

Here is a step-by-step approach to evaluating an image classification model on an Imbalanced dataset:

1. Split the dataset into training and test sets. It is important to use stratified sampling to ensure that each class is represented in both the training and test sets.
2. Train the image classification model on the training set.
3. Predict the classes of the test set.
4. Calculate the confusion matrix. The confusion matrix shows the number of true positives, true negatives, false positives, and false negatives for each class.
5. Calculate the accuracy, recall, precision, and F1 score for each class. These metrics can be calculated using the confusion matrix.
  Accuracy: (TP+TN) / (TP+TN+FP+FN)
  Recall: TP / (TP+FN)
  Precision: TP / (TP+FP)
  F1 Score: 2 * (precision * recall) / (precision + recall)
6. Calculate the AUC and ROC. The AUC is a measure of how well the model can distinguish between the positive and negative classes. The ROC curve is a plot of the true positive rate (recall) versus the false positive rate (1-specificity) at different classification thresholds.

7. Calculate the RUC, which stands for “Receiver Operating Characteristics,” and is used to evaluate the performance of binary classification models.

In conclusion, it is possible to perform image classification on an unbalanced dataset, but it requires additional considerations when evaluating the performance of the model. We need to use metrics like recall, precision, F1 score, AUC, and ROC to ensure that the model is performing well on both the majority and minority classes.

A bar chart of precision, recall, and F1 score for each class
A ROC curve for each class, along with the AUC score
Note that since we artificially made the MNIST dataset Imbalanced, the performance of the model on each class may vary widely. In practice, it is important to balance the dataset as much as possible to avoid biased results.


