Validation Loss  of the Model
==============================


In this activity, you will learn to plot the graph of epoch and loss.




<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/10546785/pasted-from-clipboard.png" width = "480" height = "220">




Follow the given steps to complete this activity:


1. Plot the graph

* Open the file  main.py.

 *  Declare variable `val_loss` and add `history.history['val_loss]` to get the loss value.


    `val_loss = history.history['val_loss']`


* Plot the `validation` `loss` at each `epoch` using `history` using `plt.plot`.


    `plt.plot(epochs, val_loss, 'r', label='Validation loss')`


    `plt.title('Training and validation loss')`


    `plt.xlabel('Epochs')`


    `plt.ylabel('Loss')`


    `plt.legend()`


    `plt.show()`


* Save and run the code to check the output.
