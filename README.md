# American Sign Language Classification using CNN

## Description
- Four models - AlexNet, ResNet-18, MobileNetV2 and DivisiveNet are trained for ASL classification.
- A new CNN architecture - DivisiveNet is developed.
    - Divides the input image continuously until a single dimensional vector is obtained.
    - The single dimesnional vector is further divided using a series of dense layers until 36 output units are produced.
    - Uses batch normalisation, Leaky ReLU after each convolutions and dense layer.
    - Log softmax is used for classification output.
- All the layers except the final dense layer in the SOTA models are freezed for transfer learning.

## Dataset
- ASL dataset from Kaggle: [https://www.kaggle.com/datasets/ayuraj/asl-dataset](https://www.kaggle.com/datasets/ayuraj/asl-dataset).

## Code
- [Assignment-2.ipynb](./Assignment-2.ipynb) - Contains code for training and evaluating AlexNet, ResNet-18, and DivisiveNet.
- [Assignment-2-mobilenet.ipynb](./Assignment-2-mobilenet.ipynb) - Contains code for training and evaluating MobileNetV2.
- [Assignment-2-overfit-custom.ipynb](./Assignment-2-overfit-custom.ipynb) - Contains code for training and evaluating DivisiveNet without early stopping.
