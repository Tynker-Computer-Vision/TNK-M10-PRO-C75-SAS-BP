Add Epochs
===========

In this activity, you will learn to create the model.


<img src= "https://s3-whjr-curriculum-uploads.whjr.online/e211206b-5d3f-438b-bb19-02e242399c0a.gif" >


Follow the given steps to complete this activity:

1. Create the model

* Open the main.py file.

* Add the convolution layer using the `.add()` method.

* Use `Convo2D()` function to create the layer. 

* Inside the function pass `128` which is the number of filters or feature detectors to be used, `kernel_size=3` which is the size of each filter, `activation = 'relu'` is a function which helps Convo layers to extract complex features and `input_shape=(200,200,3)` which is the shape of image on which the image will be trained. 
 
    `age_model.add(Conv2D(128, kernel_size=3, activation='relu', input_shape=(200,200,3)))`

* Add a layer called `MaxPool2D` that reduces the dimensions of the image after the `Conv2D`layer.

    `age_model.add(MaxPool2D(pool_size=3, strides=2))`

* Compile the model using `compile()` and pass `optimizer='adam', loss='mse', metrics=['mae']` as parameters.

    `age_model.compile(optimizer='adam', loss='mse', metrics=['mae'])`
    
* Print the model summary using `summary()`

    `print(age_model.summary())`

* Train the model using `training_images`, and `training_ages` and save the information returned in a variable named `history`.

    `history = age_model.fit(training_images, training_ages, validation_data=(testing_images, testing_ages), epochs=10)`

* Save the model to a file named `age_model_50epochs.h`.

    `age_model.save('age_model_50epochs.h5')`
    
* Save and run the code to check the output.

