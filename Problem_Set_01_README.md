# Problem Set 01 - Chest X-Ray Classification Using CNN

## Overview
This project uses a Convolutional Neural Network (CNN) to classify chest X-ray images into two classes:
- NORMAL
- PNEUMONIA

## Dataset
- Training images: 5,216
- Validation images: 16
- Test images: 624
- Number of classes: 2

## Approach
1. Loaded the chest X-ray dataset.
2. Resized images to 150 × 150 pixels.
3. Normalized pixel values by dividing by 255.
4. Built a CNN with convolutional and max-pooling layers.
5. Used ReLU activation in hidden layers.
6. Used sigmoid activation in the output layer.
7. Used Adam optimizer.
8. Used binary cross-entropy loss.
9. Trained the model for 10 epochs.
10. Evaluated the model using the test dataset.
11. Generated a classification report and confusion matrix.

## CNN Architecture
- Conv2D: 32 filters
- MaxPooling
- Conv2D: 64 filters
- MaxPooling
- Conv2D: 128 filters
- MaxPooling
- Flatten
- Dense: 128 neurons
- Dropout
- Output: 1 neuron

## Results
- Final training accuracy: 98.87%
- Test accuracy: 71.96%

Classification report:
- NORMAL precision: 0.97
- NORMAL recall: 0.26
- PNEUMONIA precision: 0.69
- PNEUMONIA recall: 0.99

## Findings
The CNN achieved very high training accuracy but lower test accuracy, indicating possible overfitting. The model was very good at identifying PNEUMONIA images but had difficulty identifying some NORMAL images.

## Conclusion
A CNN model was successfully developed for chest X-ray classification and achieved 71.96% test accuracy. Further improvement could be achieved using data augmentation, regularization, a larger validation set, or transfer learning.
