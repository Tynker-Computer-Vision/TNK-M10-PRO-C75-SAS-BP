Create Trainig and Testing Data
================================

In this activity, you will split the ages and images array into training data set and testing data set and print their lengths.


<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/10553773/pasted-from-clipboard.png" width = "480" height = "220">


Follow the given steps to complete this activity:

1. Split the data

* Open the file  main.py.

* Create variables `training_images, testing_images, training_ages, testing_ages` to store the images and ages after they are split.

* Call the function `train_test_split()`and pass `images` and , `ages` as parmeters of the function.

    `training_images, testing_images, training_ages, testing_ages = train_test_split(images, ages)`


* Print the length of these variables.
 
    `print("::::::::::::::::::::::::::::::::::::::::::::")`


    `print("Number of training images ", len(training_images))`


    `print("Number of testing images ", len(testing_images))`


    `print("Number of training ages ", len(training_ages))`


    `print("Number of training ages ", len(testing_ages))`


    `print("::::::::::::::::::::::::::::::::::::::::::::")`


* Save and run the code to check the output.
