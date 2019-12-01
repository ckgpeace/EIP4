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

Accuracy: 0.9901 (From model9 in the code using 2 Maxpool layers)

## Assignment2

### Total params: 14,060
### Trainable params: 13,848
### Non-trainable params: 212

### Test Accuracy = [0.019574204561067746, 0.9945]


### Epochs:

Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 11s 184us/step - loss: 0.5410 - acc: 0.8466 - val_loss: 0.1032 - val_acc: 0.9813
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 6s 96us/step - loss: 0.2521 - acc: 0.9244 - val_loss: 0.0552 - val_acc: 0.9886
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 6s 97us/step - loss: 0.2002 - acc: 0.9402 - val_loss: 0.0442 - val_acc: 0.9908
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1690 - acc: 0.9460 - val_loss: 0.0405 - val_acc: 0.9903
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1524 - acc: 0.9503 - val_loss: 0.0340 - val_acc: 0.9906
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1415 - acc: 0.9509 - val_loss: 0.0279 - val_acc: 0.9934
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 6s 98us/step - loss: 0.1325 - acc: 0.9527 - val_loss: 0.0275 - val_acc: 0.9926
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1259 - acc: 0.9527 - val_loss: 0.0274 - val_acc: 0.9920
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1188 - acc: 0.9546 - val_loss: 0.0279 - val_acc: 0.9917
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1136 - acc: 0.9543 - val_loss: 0.0274 - val_acc: 0.9923
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 6s 98us/step - loss: 0.1119 - acc: 0.9550 - val_loss: 0.0238 - val_acc: 0.9928
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1085 - acc: 0.9555 - val_loss: 0.0289 - val_acc: 0.9925
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1056 - acc: 0.9557 - val_loss: 0.0205 - val_acc: 0.9945
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1018 - acc: 0.9560 - val_loss: 0.0270 - val_acc: 0.9920
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 6s 99us/step - loss: 0.0987 - acc: 0.9581 - val_loss: 0.0240 - val_acc: 0.9934
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 6s 99us/step - loss: 0.0966 - acc: 0.9587 - val_loss: 0.0196 - val_acc: 0.9941
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 6s 98us/step - loss: 0.0981 - acc: 0.9572 - val_loss: 0.0247 - val_acc: 0.9931
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 6s 98us/step - loss: 0.0968 - acc: 0.9564 - val_loss: 0.0214 - val_acc: 0.9940
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 6s 96us/step - loss: 0.0964 - acc: 0.9563 - val_loss: 0.0192 - val_acc: 0.9944
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 6s 98us/step - loss: 0.0932 - acc: 0.9574 - val_loss: 0.0196 - val_acc: 0.9945
