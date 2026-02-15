# Assignment 2 Q4: Effect of Batch Normalization in Deep CNNs

## Problem Definition

Study the effect of Batch Normalization on training stability,
activation statistics, and classification performance.

## Dataset

- Tiny-ImageNet-10
- Train / Validation / Test split

## Model Architectures

- DeepCNN without BatchNorm
- DeepCNN with BatchNorm after each convolution

## Methodology

- Optimizer: Adam
- Learning rate: 0.001
- Epochs: 10 to 12
- Activation mean & variance tracked at 5th layer

## Results

| Model   | Accuracy | Precision | Recall | F1    |
| ------- | -------- | --------- | ------ | ----- |
| No BN   | 0.523    | 0.529     | 0.523  | 0.517 |
| With BN | 0.597    | 0.625     | 0.597  | 0.585 |

## Key Observations

- BatchNorm improves accuracy and stability
- Activation variance remains bounded with BN
- Faster convergence observed
