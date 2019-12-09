# Assignment4A

All the 104 images are annotated as per guidelines @ https://ia.inkers.ai/

# Assignment4B

### Epoch 42 achieved 90.2% validation accuracy using Resnet20-v1

Epoch 42/50
Learning rate:  0.0002130833
391/391 [==============================] - 31s 79ms/step - loss: 0.2132 - acc: 0.9750 - val_loss: 0.5174 - val_acc: 0.9021

Note: List of all epochs are present below

### Test accuracy: 0.8968

### Strategy
1. Changed the learning rate in default model
2. Change the filter size in the default model
3. Change batch size in default model
4. Use image augmentation

### NOTE: Gradcam images in the gradcam folder in the assignment4 folder


### All Epoch for the model run
### ------------------------------------------------------------------------------------------------------------------
Using real-time data augmentation.
Epoch 1/50
Learning rate:  0.003
391/391 [==============================] - 39s 101ms/step - loss: 1.7552 - acc: 0.4703 - val_loss: 2.2848 - val_acc: 0.4093

Epoch 00001: val_acc improved from -inf to 0.40930, saving model to /content/saved_models/cifar10_ResNet20v1_model.001.h5
Epoch 2/50
Learning rate:  0.0022744503
391/391 [==============================] - 30s 77ms/step - loss: 1.2132 - acc: 0.6551 - val_loss: 1.3032 - val_acc: 0.6282

Epoch 00002: val_acc improved from 0.40930 to 0.62820, saving model to /content/saved_models/cifar10_ResNet20v1_model.002.h5
Epoch 3/50
Learning rate:  0.0018315018
391/391 [==============================] - 30s 77ms/step - loss: 1.0100 - acc: 0.7307 - val_loss: 1.6597 - val_acc: 0.5474

Epoch 00003: val_acc did not improve from 0.62820
Epoch 4/50
Learning rate:  0.0015329586
391/391 [==============================] - 31s 80ms/step - loss: 0.8894 - acc: 0.7715 - val_loss: 1.0645 - val_acc: 0.7155

Epoch 00004: val_acc improved from 0.62820 to 0.71550, saving model to /content/saved_models/cifar10_ResNet20v1_model.004.h5
Epoch 5/50
Learning rate:  0.0013181019
391/391 [==============================] - 31s 79ms/step - loss: 0.8046 - acc: 0.7983 - val_loss: 1.3296 - val_acc: 0.6707

Epoch 00005: val_acc did not improve from 0.71550
Epoch 6/50
Learning rate:  0.0011560694
391/391 [==============================] - 31s 78ms/step - loss: 0.7444 - acc: 0.8199 - val_loss: 0.9661 - val_acc: 0.7560

Epoch 00006: val_acc improved from 0.71550 to 0.75600, saving model to /content/saved_models/cifar10_ResNet20v1_model.006.h5
Epoch 7/50
Learning rate:  0.0010295127
391/391 [==============================] - 31s 80ms/step - loss: 0.6844 - acc: 0.8365 - val_loss: 1.0145 - val_acc: 0.7446

Epoch 00007: val_acc did not improve from 0.75600
Epoch 8/50
Learning rate:  0.0009279307
391/391 [==============================] - 31s 79ms/step - loss: 0.6442 - acc: 0.8517 - val_loss: 0.9258 - val_acc: 0.7697

Epoch 00008: val_acc improved from 0.75600 to 0.76970, saving model to /content/saved_models/cifar10_ResNet20v1_model.008.h5
Epoch 9/50
Learning rate:  0.0008445946
391/391 [==============================] - 31s 79ms/step - loss: 0.6085 - acc: 0.8625 - val_loss: 0.7579 - val_acc: 0.8103

Epoch 00009: val_acc improved from 0.76970 to 0.81030, saving model to /content/saved_models/cifar10_ResNet20v1_model.009.h5
Epoch 10/50
Learning rate:  0.0007749935
391/391 [==============================] - 31s 80ms/step - loss: 0.5789 - acc: 0.8687 - val_loss: 1.0242 - val_acc: 0.7418

Epoch 00010: val_acc did not improve from 0.81030
Epoch 11/50
Learning rate:  0.0007159905
391/391 [==============================] - 32s 81ms/step - loss: 0.5426 - acc: 0.8809 - val_loss: 0.6856 - val_acc: 0.8294

Epoch 00011: val_acc improved from 0.81030 to 0.82940, saving model to /content/saved_models/cifar10_ResNet20v1_model.011.h5
Epoch 12/50
Learning rate:  0.000665336
391/391 [==============================] - 31s 78ms/step - loss: 0.5182 - acc: 0.8867 - val_loss: 0.6338 - val_acc: 0.8529

Epoch 00012: val_acc improved from 0.82940 to 0.85290, saving model to /content/saved_models/cifar10_ResNet20v1_model.012.h5
Epoch 13/50
Learning rate:  0.0006213753
391/391 [==============================] - 30s 78ms/step - loss: 0.4913 - acc: 0.8967 - val_loss: 0.6383 - val_acc: 0.8470

Epoch 00013: val_acc did not improve from 0.85290
Epoch 14/50
Learning rate:  0.0005828638
391/391 [==============================] - 31s 78ms/step - loss: 0.4704 - acc: 0.9026 - val_loss: 0.7744 - val_acc: 0.8179

Epoch 00014: val_acc did not improve from 0.85290
Epoch 15/50
Learning rate:  0.0005488474
391/391 [==============================] - 31s 78ms/step - loss: 0.4532 - acc: 0.9061 - val_loss: 0.6440 - val_acc: 0.8546

Epoch 00015: val_acc improved from 0.85290 to 0.85460, saving model to /content/saved_models/cifar10_ResNet20v1_model.015.h5
Epoch 16/50
Learning rate:  0.0005185825
391/391 [==============================] - 30s 78ms/step - loss: 0.4366 - acc: 0.9121 - val_loss: 0.6598 - val_acc: 0.8481

Epoch 00016: val_acc did not improve from 0.85460
Epoch 17/50
Learning rate:  0.000491481
391/391 [==============================] - 31s 78ms/step - loss: 0.4157 - acc: 0.9185 - val_loss: 0.6297 - val_acc: 0.8582

Epoch 00017: val_acc improved from 0.85460 to 0.85820, saving model to /content/saved_models/cifar10_ResNet20v1_model.017.h5
Epoch 18/50
Learning rate:  0.0004670715
391/391 [==============================] - 30s 78ms/step - loss: 0.4012 - acc: 0.9223 - val_loss: 0.6057 - val_acc: 0.8632

Epoch 00018: val_acc improved from 0.85820 to 0.86320, saving model to /content/saved_models/cifar10_ResNet20v1_model.018.h5
Epoch 19/50
Learning rate:  0.0004449718
391/391 [==============================] - 30s 77ms/step - loss: 0.3875 - acc: 0.9261 - val_loss: 0.5520 - val_acc: 0.8737

Epoch 00019: val_acc improved from 0.86320 to 0.87370, saving model to /content/saved_models/cifar10_ResNet20v1_model.019.h5
Epoch 20/50
Learning rate:  0.000424869
391/391 [==============================] - 31s 78ms/step - loss: 0.3776 - acc: 0.9284 - val_loss: 0.6052 - val_acc: 0.8605

Epoch 00020: val_acc did not improve from 0.87370
Epoch 21/50
Learning rate:  0.0004065041
391/391 [==============================] - 30s 78ms/step - loss: 0.3625 - acc: 0.9339 - val_loss: 0.5787 - val_acc: 0.8730

Epoch 00021: val_acc did not improve from 0.87370
Epoch 22/50
Learning rate:  0.000389661
391/391 [==============================] - 31s 78ms/step - loss: 0.3517 - acc: 0.9363 - val_loss: 0.6693 - val_acc: 0.8509

Epoch 00022: val_acc did not improve from 0.87370
Epoch 23/50
Learning rate:  0.0003741581
391/391 [==============================] - 30s 78ms/step - loss: 0.3379 - acc: 0.9408 - val_loss: 0.6696 - val_acc: 0.8542

Epoch 00023: val_acc did not improve from 0.87370
Epoch 24/50
Learning rate:  0.0003598417
391/391 [==============================] - 31s 79ms/step - loss: 0.3240 - acc: 0.9447 - val_loss: 0.5945 - val_acc: 0.8733

Epoch 00024: val_acc did not improve from 0.87370
Epoch 25/50
Learning rate:  0.0003465804
391/391 [==============================] - 30s 77ms/step - loss: 0.3188 - acc: 0.9468 - val_loss: 0.5871 - val_acc: 0.8762

Epoch 00025: val_acc improved from 0.87370 to 0.87620, saving model to /content/saved_models/cifar10_ResNet20v1_model.025.h5
Epoch 26/50
Learning rate:  0.0003342618
391/391 [==============================] - 30s 78ms/step - loss: 0.3096 - acc: 0.9492 - val_loss: 0.5257 - val_acc: 0.8879

Epoch 00026: val_acc improved from 0.87620 to 0.88790, saving model to /content/saved_models/cifar10_ResNet20v1_model.026.h5
Epoch 27/50
Learning rate:  0.0003227889
391/391 [==============================] - 31s 79ms/step - loss: 0.3034 - acc: 0.9506 - val_loss: 0.5465 - val_acc: 0.8863

Epoch 00027: val_acc did not improve from 0.88790
Epoch 28/50
Learning rate:  0.0003120774
391/391 [==============================] - 31s 80ms/step - loss: 0.2917 - acc: 0.9534 - val_loss: 0.5962 - val_acc: 0.8746

Epoch 00028: val_acc did not improve from 0.88790
Epoch 29/50
Learning rate:  0.000302054
391/391 [==============================] - 31s 79ms/step - loss: 0.2860 - acc: 0.9559 - val_loss: 0.6169 - val_acc: 0.8731

Epoch 00029: val_acc did not improve from 0.88790
Epoch 30/50
Learning rate:  0.0002926544
391/391 [==============================] - 31s 80ms/step - loss: 0.2777 - acc: 0.9577 - val_loss: 0.5740 - val_acc: 0.8814

Epoch 00030: val_acc did not improve from 0.88790
Epoch 31/50
Learning rate:  0.0002838221
391/391 [==============================] - 31s 79ms/step - loss: 0.2704 - acc: 0.9599 - val_loss: 0.5899 - val_acc: 0.8799

Epoch 00031: val_acc did not improve from 0.88790
Epoch 32/50
Learning rate:  0.0002755074
391/391 [==============================] - 31s 78ms/step - loss: 0.2633 - acc: 0.9619 - val_loss: 0.6250 - val_acc: 0.8748

Epoch 00032: val_acc did not improve from 0.88790
Epoch 33/50
Learning rate:  0.000267666
391/391 [==============================] - 31s 79ms/step - loss: 0.2619 - acc: 0.9621 - val_loss: 0.6094 - val_acc: 0.8767

Epoch 00033: val_acc did not improve from 0.88790
Epoch 34/50
Learning rate:  0.0002602585
391/391 [==============================] - 31s 79ms/step - loss: 0.2482 - acc: 0.9656 - val_loss: 0.5834 - val_acc: 0.8802

Epoch 00034: val_acc did not improve from 0.88790
Epoch 35/50
Learning rate:  0.00025325
391/391 [==============================] - 31s 79ms/step - loss: 0.2458 - acc: 0.9664 - val_loss: 0.5912 - val_acc: 0.8811

Epoch 00035: val_acc did not improve from 0.88790
Epoch 36/50
Learning rate:  0.0002466091
391/391 [==============================] - 30s 78ms/step - loss: 0.2437 - acc: 0.9676 - val_loss: 0.6027 - val_acc: 0.8827

Epoch 00036: val_acc did not improve from 0.88790
Epoch 37/50
Learning rate:  0.0002403076
391/391 [==============================] - 31s 78ms/step - loss: 0.2384 - acc: 0.9675 - val_loss: 0.5487 - val_acc: 0.8914

Epoch 00037: val_acc improved from 0.88790 to 0.89140, saving model to /content/saved_models/cifar10_ResNet20v1_model.037.h5
Epoch 38/50
Learning rate:  0.0002343201
391/391 [==============================] - 31s 79ms/step - loss: 0.2322 - acc: 0.9706 - val_loss: 0.5697 - val_acc: 0.8853

Epoch 00038: val_acc did not improve from 0.89140
Epoch 39/50
Learning rate:  0.0002286237
391/391 [==============================] - 30s 78ms/step - loss: 0.2278 - acc: 0.9712 - val_loss: 0.5880 - val_acc: 0.8885

Epoch 00039: val_acc did not improve from 0.89140
Epoch 40/50
Learning rate:  0.0002231977
391/391 [==============================] - 31s 79ms/step - loss: 0.2226 - acc: 0.9732 - val_loss: 0.5553 - val_acc: 0.8899

Epoch 00040: val_acc did not improve from 0.89140
Epoch 41/50
Learning rate:  0.0002180233
391/391 [==============================] - 31s 79ms/step - loss: 0.2183 - acc: 0.9738 - val_loss: 0.5929 - val_acc: 0.8841

Epoch 00041: val_acc did not improve from 0.89140
Epoch 42/50
Learning rate:  0.0002130833
391/391 [==============================] - 31s 79ms/step - loss: 0.2132 - acc: 0.9750 - val_loss: 0.5174 - val_acc: 0.9021

Epoch 00042: val_acc improved from 0.89140 to 0.90210, saving model to /content/saved_models/cifar10_ResNet20v1_model.042.h5
Epoch 43/50
Learning rate:  0.0002083623
391/391 [==============================] - 31s 79ms/step - loss: 0.2107 - acc: 0.9757 - val_loss: 0.5998 - val_acc: 0.8880

Epoch 00043: val_acc did not improve from 0.90210
Epoch 44/50
Learning rate:  0.0002038459
391/391 [==============================] - 31s 78ms/step - loss: 0.2086 - acc: 0.9759 - val_loss: 0.5954 - val_acc: 0.8886

Epoch 00044: val_acc did not improve from 0.90210
Epoch 45/50
Learning rate:  0.0001995211
391/391 [==============================] - 30s 78ms/step - loss: 0.2037 - acc: 0.9776 - val_loss: 0.5865 - val_acc: 0.8891

Epoch 00045: val_acc did not improve from 0.90210
Epoch 46/50
Learning rate:  0.0001953761
391/391 [==============================] - 31s 78ms/step - loss: 0.2018 - acc: 0.9779 - val_loss: 0.5864 - val_acc: 0.8917

Epoch 00046: val_acc did not improve from 0.90210
Epoch 47/50
Learning rate:  0.0001913998
391/391 [==============================] - 31s 79ms/step - loss: 0.1998 - acc: 0.9789 - val_loss: 0.5728 - val_acc: 0.8941

Epoch 00047: val_acc did not improve from 0.90210
Epoch 48/50
Learning rate:  0.0001875821
391/391 [==============================] - 31s 79ms/step - loss: 0.1988 - acc: 0.9779 - val_loss: 0.6774 - val_acc: 0.8701

Epoch 00048: val_acc did not improve from 0.90210
Epoch 49/50
Learning rate:  0.0001839137
391/391 [==============================] - 31s 78ms/step - loss: 0.1925 - acc: 0.9808 - val_loss: 0.5202 - val_acc: 0.9012

Epoch 00049: val_acc did not improve from 0.90210
Epoch 50/50
Learning rate:  0.000180386
391/391 [==============================] - 31s 79ms/step - loss: 0.1888 - acc: 0.9816 - val_loss: 0.5661 - val_acc: 0.8968

Epoch 00050: val_acc did not improve from 0.90210


