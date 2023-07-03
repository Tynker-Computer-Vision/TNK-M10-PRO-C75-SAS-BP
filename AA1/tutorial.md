Change the Activation Function 
==============================

In this activity, you will learn to change the activation function and how it affects the learning of the model.


<img src= "https://s3-whjr-curriculum-uploads.whjr.online/f90c517f-a9f6-459b-823f-d99343163332.png" width = "480" height = "220">


Follow the given steps to complete this activity:

1. Plot the graph

* Open the file  main.py.

* Change `activation` function to `'tanh' in all the Conv2() functions`.

    `age_model.add(Conv2D(128, kernel_size=3, activation='tanh', input_shape=(200,200,3)))`

    `age_model.add(Conv2D(128, kernel_size=3, activation='tanh'))`

    `age_model.add(Conv2D(256, kernel_size=3, activation='tanh'))`    

    `age_model.add(Conv2D(512, kernel_size=3, activation='tanh'))`

* Save and run the code to check the output.

