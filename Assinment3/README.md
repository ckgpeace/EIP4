# Assignment 3


### "I could not beat the base model :( "

1. Base model - Assignment_3_basemodel.ipynb
    #### Validation Accuracy - 83.18%
    #### Total params: 1,172,410

2. Changed model  -  Assignment_3_attempt11.ipynb
   #### Validation Accuracy - 82.32%
   #### Total params: 79,333

3. New Model Definition

``` python
# 11th attempt

# Keeping adam as optimizer
# Changing the image augmentaion
# Changing model architecture
# Adding GAP


model=Sequential()
model.add(SeparableConv2D(64, kernel_size=(3, 3), padding='same',  activation='relu', input_shape=(32,32,3))) #32x32x64 RF = 3
model.add(SeparableConv2D(64, kernel_size=(3, 3), activation='relu')) #30x30x64 #RF =5
model.add(BatchNormalization())
model.add(MaxPooling2D(pool_size=(2,2)))  #15x15x32 #RF = 6

model.add(SeparableConv2D(128, kernel_size=(3, 3), padding='same',  activation='relu', input_shape=(32,32,3))) #15x15x64 RF = 8
model.add(SeparableConv2D(128, kernel_size=(3, 3), activation='relu')) #13x13x64 RF = 10
model.add(BatchNormalization())
model.add(MaxPooling2D(pool_size=(2,2)))  #6x6x64 RF = 11

model.add(SeparableConv2D(256, kernel_size=(3, 3), padding='same',  activation='relu', input_shape=(32,32,3))) #6x6x128 RF = 13
model.add(BatchNormalization())

model.add(SeparableConv2D(10, kernel_size=(6, 6), activation='relu'))  #1x1x10

model.add(GlobalAveragePooling2D())

model.add(Activation('softmax'))

###### Compile the model
from keras.optimizers import Adam
from keras.callbacks import LearningRateScheduler
def scheduler(epoch, lr):
  return round(0.003 * 1/(1 + 0.319 * epoch), 10)

model.compile(optimizer=Adam(lr=0.003),loss='categorical_crossentropy',metrics=['accuracy'])
```

4. New model Epochs:

Epoch 1/50

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
390/390 [==============================] - 43s 111ms/step - loss: 1.5526 - acc: 0.4365 - val_loss: 2.7832 - val_acc: 0.3833
Epoch 2/50

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
390/390 [==============================] - 38s 97ms/step - loss: 1.1789 - acc: 0.5804 - val_loss: 1.8594 - val_acc: 0.5034
Epoch 3/50

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
390/390 [==============================] - 38s 97ms/step - loss: 1.0263 - acc: 0.6386 - val_loss: 1.3349 - val_acc: 0.5283
Epoch 4/50

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
390/390 [==============================] - 38s 97ms/step - loss: 0.9211 - acc: 0.6776 - val_loss: 1.2197 - val_acc: 0.5985
Epoch 5/50

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
390/390 [==============================] - 37s 96ms/step - loss: 0.8615 - acc: 0.6997 - val_loss: 0.9269 - val_acc: 0.6845
Epoch 6/50

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
390/390 [==============================] - 38s 96ms/step - loss: 0.8045 - acc: 0.7207 - val_loss: 0.8472 - val_acc: 0.7095
Epoch 7/50

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
390/390 [==============================] - 38s 96ms/step - loss: 0.7716 - acc: 0.7305 - val_loss: 0.7478 - val_acc: 0.7445
Epoch 8/50

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
390/390 [==============================] - 37s 96ms/step - loss: 0.7370 - acc: 0.7444 - val_loss: 0.8231 - val_acc: 0.7235
Epoch 9/50

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
390/390 [==============================] - 38s 96ms/step - loss: 0.7109 - acc: 0.7536 - val_loss: 0.7227 - val_acc: 0.7572
Epoch 10/50

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
390/390 [==============================] - 38s 96ms/step - loss: 0.6821 - acc: 0.7626 - val_loss: 0.7209 - val_acc: 0.7587
Epoch 11/50

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
390/390 [==============================] - 38s 96ms/step - loss: 0.6691 - acc: 0.7677 - val_loss: 0.6618 - val_acc: 0.7789
Epoch 12/50

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
390/390 [==============================] - 38s 97ms/step - loss: 0.6551 - acc: 0.7731 - val_loss: 0.6332 - val_acc: 0.7875
Epoch 13/50

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
390/390 [==============================] - 38s 97ms/step - loss: 0.6364 - acc: 0.7795 - val_loss: 0.6970 - val_acc: 0.7723
Epoch 14/50

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
390/390 [==============================] - 38s 97ms/step - loss: 0.6249 - acc: 0.7834 - val_loss: 0.6452 - val_acc: 0.7861
Epoch 15/50

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
390/390 [==============================] - 37s 96ms/step - loss: 0.6132 - acc: 0.7859 - val_loss: 0.6137 - val_acc: 0.7946
Epoch 16/50

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
390/390 [==============================] - 38s 97ms/step - loss: 0.6044 - acc: 0.7910 - val_loss: 0.6789 - val_acc: 0.7757
Epoch 17/50

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
390/390 [==============================] - 38s 97ms/step - loss: 0.5970 - acc: 0.7944 - val_loss: 0.6069 - val_acc: 0.7985
Epoch 18/50

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
390/390 [==============================] - 38s 96ms/step - loss: 0.5862 - acc: 0.7958 - val_loss: 0.5979 - val_acc: 0.8009
Epoch 19/50

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
390/390 [==============================] - 38s 97ms/step - loss: 0.5807 - acc: 0.7984 - val_loss: 0.6918 - val_acc: 0.7727
Epoch 20/50

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
390/390 [==============================] - 38s 97ms/step - loss: 0.5760 - acc: 0.8002 - val_loss: 0.6006 - val_acc: 0.7979
Epoch 21/50

Epoch 00021: LearningRateScheduler setting learning rate to 0.0004065041.
390/390 [==============================] - 38s 97ms/step - loss: 0.5658 - acc: 0.8060 - val_loss: 0.5971 - val_acc: 0.7951
Epoch 22/50

Epoch 00022: LearningRateScheduler setting learning rate to 0.000389661.
390/390 [==============================] - 38s 97ms/step - loss: 0.5590 - acc: 0.8056 - val_loss: 0.5765 - val_acc: 0.8085
Epoch 23/50

Epoch 00023: LearningRateScheduler setting learning rate to 0.0003741581.
390/390 [==============================] - 38s 97ms/step - loss: 0.5494 - acc: 0.8084 - val_loss: 0.5888 - val_acc: 0.8046
Epoch 24/50

Epoch 00024: LearningRateScheduler setting learning rate to 0.0003598417.
390/390 [==============================] - 38s 97ms/step - loss: 0.5448 - acc: 0.8111 - val_loss: 0.6500 - val_acc: 0.7860
Epoch 25/50

Epoch 00025: LearningRateScheduler setting learning rate to 0.0003465804.
390/390 [==============================] - 38s 96ms/step - loss: 0.5410 - acc: 0.8121 - val_loss: 0.5828 - val_acc: 0.8060
Epoch 26/50

Epoch 00026: LearningRateScheduler setting learning rate to 0.0003342618.
390/390 [==============================] - 38s 97ms/step - loss: 0.5416 - acc: 0.8125 - val_loss: 0.6226 - val_acc: 0.7933
Epoch 27/50

Epoch 00027: LearningRateScheduler setting learning rate to 0.0003227889.
390/390 [==============================] - 37s 96ms/step - loss: 0.5319 - acc: 0.8156 - val_loss: 0.5654 - val_acc: 0.8112
Epoch 28/50

Epoch 00028: LearningRateScheduler setting learning rate to 0.0003120774.
390/390 [==============================] - 37s 96ms/step - loss: 0.5241 - acc: 0.8176 - val_loss: 0.6037 - val_acc: 0.8022
Epoch 29/50

Epoch 00029: LearningRateScheduler setting learning rate to 0.000302054.
390/390 [==============================] - 38s 97ms/step - loss: 0.5265 - acc: 0.8166 - val_loss: 0.5583 - val_acc: 0.8125
Epoch 30/50

Epoch 00030: LearningRateScheduler setting learning rate to 0.0002926544.
390/390 [==============================] - 38s 98ms/step - loss: 0.5214 - acc: 0.8198 - val_loss: 0.5890 - val_acc: 0.8066
Epoch 31/50

Epoch 00031: LearningRateScheduler setting learning rate to 0.0002838221.
390/390 [==============================] - 38s 97ms/step - loss: 0.5147 - acc: 0.8204 - val_loss: 0.5553 - val_acc: 0.8165
Epoch 32/50

Epoch 00032: LearningRateScheduler setting learning rate to 0.0002755074.
390/390 [==============================] - 38s 97ms/step - loss: 0.5124 - acc: 0.8221 - val_loss: 0.5774 - val_acc: 0.8086
Epoch 33/50

Epoch 00033: LearningRateScheduler setting learning rate to 0.000267666.
390/390 [==============================] - 38s 97ms/step - loss: 0.5043 - acc: 0.8269 - val_loss: 0.5834 - val_acc: 0.8076
Epoch 34/50

Epoch 00034: LearningRateScheduler setting learning rate to 0.0002602585.
390/390 [==============================] - 37s 96ms/step - loss: 0.5057 - acc: 0.8248 - val_loss: 0.6080 - val_acc: 0.8043
Epoch 35/50

Epoch 00035: LearningRateScheduler setting learning rate to 0.00025325.
390/390 [==============================] - 38s 97ms/step - loss: 0.5063 - acc: 0.8246 - val_loss: 0.5798 - val_acc: 0.8095
Epoch 36/50

Epoch 00036: LearningRateScheduler setting learning rate to 0.0002466091.
390/390 [==============================] - 38s 97ms/step - loss: 0.4875 - acc: 0.8315 - val_loss: 0.5498 - val_acc: 0.8168
Epoch 37/50

Epoch 00037: LearningRateScheduler setting learning rate to 0.0002403076.
390/390 [==============================] - 37s 96ms/step - loss: 0.4944 - acc: 0.8284 - val_loss: 0.5349 - val_acc: 0.8214
Epoch 38/50

Epoch 00038: LearningRateScheduler setting learning rate to 0.0002343201.
390/390 [==============================] - 38s 97ms/step - loss: 0.4990 - acc: 0.8251 - val_loss: 0.5605 - val_acc: 0.8174
Epoch 39/50

Epoch 00039: LearningRateScheduler setting learning rate to 0.0002286237.
390/390 [==============================] - 38s 97ms/step - loss: 0.4889 - acc: 0.8297 - val_loss: 0.5569 - val_acc: 0.8158
Epoch 40/50

Epoch 00040: LearningRateScheduler setting learning rate to 0.0002231977.
390/390 [==============================] - 38s 97ms/step - loss: 0.4908 - acc: 0.8303 - val_loss: 0.5676 - val_acc: 0.8134
Epoch 41/50

Epoch 00041: LearningRateScheduler setting learning rate to 0.0002180233.
390/390 [==============================] - 38s 97ms/step - loss: 0.4834 - acc: 0.8334 - val_loss: 0.5564 - val_acc: 0.8157
Epoch 42/50

Epoch 00042: LearningRateScheduler setting learning rate to 0.0002130833.
390/390 [==============================] - 38s 98ms/step - loss: 0.4784 - acc: 0.8353 - val_loss: 0.5931 - val_acc: 0.8073
Epoch 43/50

Epoch 00043: LearningRateScheduler setting learning rate to 0.0002083623.
390/390 [==============================] - 38s 98ms/step - loss: 0.4801 - acc: 0.8338 - val_loss: 0.5670 - val_acc: 0.8117
Epoch 44/50

Epoch 00044: LearningRateScheduler setting learning rate to 0.0002038459.
390/390 [==============================] - 38s 98ms/step - loss: 0.4826 - acc: 0.8310 - val_loss: 0.5543 - val_acc: 0.8150
Epoch 45/50

Epoch 00045: LearningRateScheduler setting learning rate to 0.0001995211.
390/390 [==============================] - 38s 98ms/step - loss: 0.4766 - acc: 0.8348 - val_loss: 0.5644 - val_acc: 0.8154
Epoch 46/50

Epoch 00046: LearningRateScheduler setting learning rate to 0.0001953761.
390/390 [==============================] - 38s 97ms/step - loss: 0.4758 - acc: 0.8341 - val_loss: 0.6052 - val_acc: 0.8082
Epoch 47/50

Epoch 00047: LearningRateScheduler setting learning rate to 0.0001913998.
390/390 [==============================] - 38s 97ms/step - loss: 0.4743 - acc: 0.8342 - val_loss: 0.5661 - val_acc: 0.8167
Epoch 48/50

Epoch 00048: LearningRateScheduler setting learning rate to 0.0001875821.
390/390 [==============================] - 38s 98ms/step - loss: 0.4706 - acc: 0.8365 - val_loss: 0.5377 - val_acc: 0.8235
Epoch 49/50

Epoch 00049: LearningRateScheduler setting learning rate to 0.0001839137.
390/390 [==============================] - 38s 98ms/step - loss: 0.4684 - acc: 0.8370 - val_loss: 0.5483 - val_acc: 0.8180
Epoch 50/50

Epoch 00050: LearningRateScheduler setting learning rate to 0.000180386.
390/390 [==============================] - 38s 98ms/step - loss: 0.4678 - acc: 0.8379 - val_loss: 0.5325 - val_acc: 0.8232
Model took 1896.06 seconds to train

Accuracy on test data is: 82.32


