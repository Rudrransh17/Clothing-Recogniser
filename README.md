# Clothing Recognizer

This project aims to develop a Clothing Recognizer using the Fashion MNIST dataset. The Fashion MNIST dataset, available at [https://github.com/zalandoresearch/fashion-mnist](https://github.com/zalandoresearch/fashion-mnist). Each image is assigned to one of the following labels:

Label   | Description
--------|------------
0       | T-shirt/top
1       | Trouser
2       | Pullover
3       | Dress
4       | Coat
5       | Sandal
6       | Shirt
7       | Sneaker
8       | Bag
9       | Ankle boot

## Dataset

The Fashion MNIST dataset contains grayscale images, where the pixel values range from 0 to 255. To prepare the data for training, the pixel values were scaled to a range of 0 to 1.

## Model Architecture

The model used for this project consists of the following layers:

1. Flatten Layer: Flattens the 28x28 input images into a 784-dimensional vector.
2. Dense Layer: A fully connected layer with a specified number of neurons.
3. Softmax Dense Layer: The output layer with 10 neurons, using the softmax activation function.

## Training and Evaluation

The model was trained with different configurations of neurons and epochs, and the accuracy metric was recorded for each configuration. The recorded accuracy results are as follows:

|Neurons\Epoch| 5      | 10     | 15     | 20     |
|---------|--------|--------|--------|--------|
| 128     | 0.8761 | 0.8852 | 0.8842 | 0.8854 |
| 256     | 0.8711 | 0.8802 | 0.8818 | 0.8924 |
| 512     | 0.8795 | 0.8838 | 0.8908 | 0.8899 |
| 1024    | 0.8701 | 0.8798 | 0.893  | 0.8958 |

The accuracy results were compared for different configurations of neurons and epochs, providing insights into the model's performance.

## Model Notebook

For further details on the model development and training, please refer to the [model.ipynb](model.ipynb) notebook.

## Future Development

The project is still under development, with the next target being the inclusion of Conv2D and MaxPooling layers to enhance the model's performance.
