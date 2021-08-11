# Fashion_MNIST-End-to-End-Using-Streamlit
Trained Convolutional Neural Network on Fashion MNIST dataset.
### **Data Description**
This is a dataset of 60,000 28x28 grayscale images of 10 fashion categories,
along with a test set of 10,000 images. 
The classes are:

Label	Description:

{
0: T-shirt/top,

1: Trouser,

2: Pullover,

3: Dress,

4: Coat,

5: Sandal,

6: Shirt,

7: Sneaker,

8: Bag,

9: Ankle boot}

Returns:
  Tuple of NumPy arrays: (x_train, y_train), (x_test, y_test).

**x_train**: uint8 NumPy array of grayscale image data with shapes
  (60000, 28, 28), containing the training data.

**y_train**: uint8 NumPy array of labels (integers in range 0-9)
  with shape (60000,) for the training data.

**x_test**: uint8 NumPy array of grayscale image data with shapes
  (10000, 28, 28), containing the test data.

**y_test**: uint8 NumPy array of labels (integers in range 0-9)
  with shape (10000,) for the test data.
### **Model Summary**
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
input_8 (InputLayer)         [(None, 28, 28, 1)]       0         
_________________________________________________________________
conv2d_27 (Conv2D)           (None, 28, 28, 32)        320       
_________________________________________________________________
batch_normalization_26 (Batc (None, 28, 28, 32)        128       
_________________________________________________________________
tf.nn.relu_26 (TFOpLambda)   (None, 28, 28, 32)        0         
_________________________________________________________________
max_pooling2d_20 (MaxPooling (None, 14, 14, 32)        0         
_________________________________________________________________
conv2d_28 (Conv2D)           (None, 14, 14, 64)        18496     
_________________________________________________________________
batch_normalization_27 (Batc (None, 14, 14, 64)        256       
_________________________________________________________________
tf.nn.relu_27 (TFOpLambda)   (None, 14, 14, 64)        0         
_________________________________________________________________
max_pooling2d_21 (MaxPooling (None, 7, 7, 64)          0         
_________________________________________________________________
conv2d_29 (Conv2D)           (None, 7, 7, 128)         73856     
_________________________________________________________________
batch_normalization_28 (Batc (None, 7, 7, 128)         512       
_________________________________________________________________
tf.nn.relu_28 (TFOpLambda)   (None, 7, 7, 128)         0         
_________________________________________________________________
max_pooling2d_22 (MaxPooling (None, 3, 3, 128)         0         
_________________________________________________________________
conv2d_30 (Conv2D)           (None, 3, 3, 128)         147584    
_________________________________________________________________
batch_normalization_29 (Batc (None, 3, 3, 128)         512       
_________________________________________________________________
tf.nn.relu_29 (TFOpLambda)   (None, 3, 3, 128)         0         
_________________________________________________________________
flatten_6 (Flatten)          (None, 1152)              0         
_________________________________________________________________
dense_24 (Dense)             (None, 256)               295168    
_________________________________________________________________
dropout_10 (Dropout)         (None, 256)               0         
_________________________________________________________________
dense_25 (Dense)             (None, 128)               32896     
_________________________________________________________________
dropout_11 (Dropout)         (None, 128)               0         
_________________________________________________________________
dense_26 (Dense)             (None, 64)                8256      
_________________________________________________________________
dense_27 (Dense)             (None, 32)                2080      
_________________________________________________________________
dense_28 (Dense)             (None, 10)                330       
=================================================================
Total params: 580,394
Trainable params: 579,690
Non-trainable params: 704
