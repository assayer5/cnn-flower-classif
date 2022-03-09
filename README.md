
# Project: Image Classification with Neural Networks

### Overview
Classified ~100 different flower types with a convolutional neural network. Images were drawn from 5 public data sets to generate a [Kaggle image classification competition](https://www.kaggle.com/c/tpu-getting-started/overview). Model scored an accuracy of 0.8025 on the validation set and an accuracy of 0.7624 on the Kaggle test set.


### Language
Python

### Packages Used
numpy, tensorflow, keras

### Data Preparation, Parameters
- data augmentation: random flip, contrast, brightness, saturation
- epochs: 40
- batch size: 64*8
- learning rate: 0.01 for 8 epochs, decay to 0.0005
- early stopping: no improvement in loss after 3 epochs

### Architecture
- base model for feature extraction: Xception
- model head for classification: global average pooling, drop out 30%, 2 dense layers, softmax output layer

### Resources
[Kaggle](https://www.kaggle.com/)

[Petals to the Metal - Flower Classification on TPU](https://www.kaggle.com/c/tpu-getting-started/overview)
