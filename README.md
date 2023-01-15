## Convolutional neural network chest X-ray classification model to make diagnoses of lung disorders

- Used 1000 frontal-view X-ray images from the `ChestX-ray8` dataset (identifying 14 different pathological conditions) to train our model

- Used `MathplotLib` and seaborn to visualize the data and NumPy and pandas to manipulate it

- Prevented data leakage by doing the split to the patient level

- Made use of the ImageDataGenerator class from `Keras` framework to build a "generator" for images specified in the dataframe and used it to facilitate model training by standardizing the input distribution.

- Addressed class imbalanced by multiplying each example from each class by a class-specific weight factor

- Implemented a loss function that calculates the weighted loss for each batch

- Use of transfer learning to retrain a `DenseNet` model for X-ray image classification.

- Achieved an accuracy of 69.34 %

- Evaluated the performance of our model using classifications metrics such as Accuracy, prevalence, specificity, sensitivity, TP, TN, FP, FN, PPV, NPV, AUC, Confidence Intervals, F1 score

- Used the `ROC curve` to measure the goodness of fit of our model

- Used `Precision-Recall curve` to examine the trade-off between precision and recall for different thresholds.

- Obtained the probability of each predicted label using calibration and generated a calibration plot with `Sckit-learn` to observe how our model's probabilities are aligned with the real probabilities

- Used `Platt scaling` to improve our model's calibration

