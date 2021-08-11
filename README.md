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
