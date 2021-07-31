# Wednesday 7/28 - Neural Style Transfer
On wednesday, we used Tensor Flow to perform a neural style transfer, following the 4 steps I have outlined below. Using the same approach, I used a collection of new images to practice neural style transfer.

###___Content Image:___

#####Danny DeVito
![img_41.png](img_41.png)

###___Style images:___

#####Owl Prints (Charley Harper)
![img_40.png](img_40.png)

#####Marilyn Monroe Print (Andy Warhol)
![img_39.png](img_39.png)

### Define and extract content and style representations
The first step for neural style transfer was to build a model to define (and later extract) features from the style images. In class, we utilized a pretrained image classification network - VGG19 - to define the images' contents. To build the extraction model, I chose which layers to use for content and style and built a model to implement said layers. After running the model, I was left with Gram matrices for the content and style images. These matrices work by calculating the outer product of the feature vector with itself at each location and allow us to represent style in a highly transposable manner.

### Implementing the style transfer algorithm
To run gradient descent, I first needed to define it within a `tf.Variable` object, define a function to keep pixel values between 0 and 1, and create two weighted optimizers to calculate the model's total loss. With this in place, I defined a function using `tf.GradientTape` at a rate of 100 training steps per epoch over 10 epochs. This produced the following results:
![img_42.png](img_42.png)
![img_43.png](img_43.png)

### Apply regularization term on the high frequency components

#####As demonstrated in the images below, preprocessing the original images into the stylized format creates alot of variancec in the images. In order to reduce this, I reran the model I outlined above with regularization layers encoded within it. 

![img_45.png](img_45.png)
![img_46.png](img_46.png)
![img_47.png](img_47.png)
![img_48.png](img_48.png)
![img_49.png](img_49.png)
![img_50.png](img_50.png)

##### With regularization, the stylized image my model produced was:
![img_51.png](img_51.png)
