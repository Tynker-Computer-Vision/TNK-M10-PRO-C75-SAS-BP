Interchange the X and Y Axes
==============================

In this activity, you will learn to plot the graph of by inter changing the X and Y axes.


<img src= "https://s3-whjr-curriculum-uploads.whjr.online/66de92c2-adc7-494f-8f38-7b0cf563c055.png" width = "480" height = "220">


Follow the given steps to complete this activity:


1. Plot the graph


* Open the file main.py.


*Use `plt` to  plot the graph..

    `plt.plot(x,y,'color', label)`

* Change the `X` to  and `Y` axis while plotting the graph.

    `plt.plot(loss, epochs,  'y', label='Training loss')`

* Change the `X` and `Y` axis in the graph.

    `plt.plot(val_loss, epochs, 'r', label='Validation loss')`

    `plt.title('Training and validation loss')`


* Change the X and Y labels in the plot.

    `plt.ylabel('Epochs')`

    `plt.xlabel('Loss')`

* Save and run the code to check the output.