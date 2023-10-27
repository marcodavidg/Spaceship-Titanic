# Spaceship-Titanic
Kaggle competition about binary classification. 
https://www.kaggle.com/competitions/spaceship-titanic/overview

The model is implemented in Pytorch and it's designed for binary classification tasks. Here's its description:
  - Hidden Layers: The core of the model consists of a sequence of fully connected (linear) layers, followed by batch normalization, ReLU activation, and dropout. The model is structured as follows:
    - Input Layer: A linear layer with input_size input features and 64 output features.
    - Batch Normalization: A batch normalization layer applied to the 64 output features.
    - ReLU Activation: A Rectified Linear Unit (ReLU) activation function is applied after batch normalization.
    - Dropout: A dropout layer with a dropout probability of 0.5 is used to prevent overfitting.

    - This sequence of layers is repeated for a total of four times with increasing output feature dimensions (64, 128, 64, 32).

  - Output Layer: The final linear layer has 32 input features and 1 output feature. This is the output layer for binary classification.

    - Sigmoid Activation: A sigmoid activation function is applied to the output of the final linear layer. Sigmoid is commonly used for binary classification to squash the output to the range [0, 1], which can be interpreted as the probability of belonging to the positive class.

The model's architecture includes batch normalization and dropout layers to improve training stability and prevent overfitting. It is suitable for binary classification tasks where you want to predict a binary outcome (e.g., 0 or 1). The Sigmoid activation function in the final layer ensures that the model's output is within the [0, 1] range, which can be interpreted as a probability.


