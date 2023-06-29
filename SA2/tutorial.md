Add Epoch
===========

In this activity, you will learn to create the model.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/10553773/pasted-from-clipboard.png" width = "480" height = "220">


Follow the given steps to complete this activity:

1. Create the model

* Open the main.py file.

* import `Sequential` from `keras.models`.

    `from keras.models import Sequential`


* Initialize the `age_model` using `sequential()`.

    `age_model = Sequential()`

* Add the convolution layer using the `.add()` method.

* Use `Convo2D()` function to create the layer. 

* Inside the function pass `128` which is the number of filters or feature detectors to be used, `kernel_size=3` which is the size of each filter, `activation = 'relu'` is a function which helps Convo layers to extract complex features and `input_shape=(200,200,3)` which is the shape of image on which the image will be trained. 
 
    `age_model.add(Conv2D(128, kernel_size=3, activation='relu', input_shape=(200,200,3)))`

* Add a layer called `MaxPool2D` that reduces the dimensions of the image after the `Conv2D`layer.

    `age_model.add(MaxPool2D(pool_size=3, strides=2))`

* Add the convolution layers with different numbers of filters and add `MaxPool2D` layers.

    `age_model.add(Conv2D(128, kernel_size=3, activation='relu'))`

    `age_model.add(MaxPool2D(pool_size=3, strides=2))`
              
    `age_model.add(Conv2D(256, kernel_size=3, activation='relu'))`

    `age_model.add(MaxPool2D(pool_size=3, strides=2))`

    `age_model.add(Conv2D(512, kernel_size=3, activation='relu'))`
    
    `age_model.add(MaxPool2D(pool_size=3, strides=2))`

* Convert the output array returned from the `Feature Learning Layers` to `1D` using array `Flatten()`.

    `age_model.add(Flatten())`

* Remove extra node in the CNN using `Dropout()`.

    `age_model.add(Dropout(0.2))`

* Compile the model using `compile()` and pass `optimizer='adam', loss='mse', metrics=['mae']` as parameters.

    `age_model.compile(optimizer='adam', loss='mse', metrics=['mae'])`
    
* Print the model summary using `summary()`

    `print(age_model.summary())`

* Fit the model using `training_images`, `training_ages` and save the returned information in `history` variable.

    `history = age_model.fit(training_images, training_ages, validation_data=(testing_images, testing_ages), epochs=10)`

* Save the model to file named `age_model_50epochs.h`.

    `age_model.save('age_model_50epochs.h5')`
    
* Save and run the code to check the output.

