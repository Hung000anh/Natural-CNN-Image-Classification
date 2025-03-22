# Natural-CNN-Image-Classification

This repository contains a CNN-based image classification model trained on a dataset with 8 classes. The model uses Keras and TensorFlow for training and evaluation.

## Dataset Information

- **Total images in the dataset:** 6899
- **Total images in the training set:** 5516
- **Total images in the test set:** 1383
- **Number of classes:** 8

## Model Architecture

The model architecture is as follows:

1. **Convolutional Layers**:
   - Conv2D: (32 filters, 3x3 kernel)
   - MaxPooling2D: (2x2 pool size)
   - Conv2D: (64 filters, 3x3 kernel)
   - MaxPooling2D: (2x2 pool size)
   - Conv2D: (128 filters, 3x3 kernel)
   - MaxPooling2D: (2x2 pool size)

2. **Fully Connected Layers**:
   - Flatten
   - Dense: 512 neurons
   - Dense: 8 neurons (output layer with softmax activation for classification)


## Training Results

- **Training Accuracy:** 99.25%
- **Validation Accuracy:** 88.00%
- **Test Accuracy:** 86.77%

## Training Process

The model was trained for 10 epochs with the following results:

| Epoch | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy |
|-------|---------------|-------------------|-----------------|---------------------|
| 1     | 1.0091        | 71.26%            | 0.4991          | 81.45%              |
| 2     | 0.2488        | 90.29%            | 0.3752          | 88.18%              |
| 3     | 0.1263        | 95.22%            | 0.7213          | 83.27%              |
| 4     | 0.0965        | 96.99%            | 0.4475          | 88.36%              |
| 5     | 0.0397        | 98.69%            | 0.4762          | 89.36%              |
| 6     | 0.0537        | 98.35%            | 0.5417          | 86.82%              |
| 7     | 0.0432        | 98.69%            | 0.4694          | 89.55%              |
| 8     | 0.0248        | 99.23%            | 0.4748          | 88.64%              |
| 9     | 0.0313        | 99.03%            | 0.4735          | 88.82%              |
| 10    | 0.0121        | 99.68%            | 0.6406          | 88.00%              |


