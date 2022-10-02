# Handwriting-Recognition-using-Convolutional-Neural-Network
Prediction of User-Drawn Digits using Convolutional Neural Networks inside a web-app, created using Flask MicroFramework for Python. <br>
The web-app allows the user to draw a digit on a virtual canvas and predicts the drawn digit using Keras-API and Tensorflow in python.

#### Updated README:
As of May 2020, more than half of the functions are either out-dated / depreciated. The project was created in 2017, and the supporting library versions for the dependencies are as follows:
> tensorflow: v0.10.0 <br>
> keras: v1.1.0 <br>
> scikit-learn: v0.19.0 <br>
> numpy: v1.14.1
## Structure:
The project uses the MNIST database of handwritten digits, with normalized sizes. The dataset is divided into 4 parts - Training Images, Training Labels, Test Images and Test Labels. <br>
The keras model created is stored in the *model.h5* file (HDF5 type). For each prediction, the model is loaded into the flask web-app through the *load.py* file inside the model folder. <br>
The pattern drawn on the canvas is converted into output.png. *app.py* loads the image, applies normalization (converting the image into 28x28 pixels), which is then passed into the *predict* method of the model. The value is then returned to the *index.html* page.
