# EIP4 

## Assignment1 
Defnitions:
1. Convolution: Convolution is a process of projecting/transforming/creating features from an input matrix(2D or 3D, usually an image) to another set of matrix ( 2D or 3D, which can be of any dimension usually driven by some empirical tests) which help in reducing parameters for training neural networks
2. Filters/Kernels: Filters/Kernels are feature extractors which are designed to extract basic features/building blocks in an image such as edges
3. Epochs: One epoch is the set of iterations where every training image has been passed through the neural network
4. 1x1 Convolution: This is convolution to reduce the number of channels, basically reduce dimensions of layers, less computation to process same information, used to make light deep neural networks without losing spacial information. (Still understanding the magic)
5. 3x3 Convolution: 3x3 kernels are designed to extract some particular features in an image such as edges 
6. Feature Maps: Feature maps are like the output after doing convolutions on an image
7. Activation Function: These are functions which decide which neuron fire after applying the function to the input from previous layers
8. Receptive Field: After doing all the convolution or convolutions, a pixel in  final output represents some representation of previous layers, the portion of the pixels of the previous layers it captures is receptive field of that particular pixel( I do not know whether this is correct or not)

The ouput of the code:

print(score)

[0.041036612204968015, 0.9901]

Accuracy: 0.9901

### Strategy: Using maxpool layers
