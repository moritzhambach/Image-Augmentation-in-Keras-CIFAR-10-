# Image Augmentation in Keras (CIFAR-10)
Using image augmentation to reach 90.3% accuracy on CIFAR_10 with a simple CNN. 

Machine learning works best when there is plenty of training data (in this case images), since this prevents overfitting of the model. If the training data is limited, one can artificilly increase it by image augmentation. Here additional images are created by rotating, shifting, zooming or other operations on the original training image.
In my case, I reach over 90 percent classificaion accuracy on CIFAR_10, a dataset with 50 000 training images in 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship and truck). I tried different operations, the best seemed to be rotations, horizontal flipping and vertical or horizontal shifts.
The model is a VGG-type convolutional network with 6 conv layers and one dense fully connected layer before the output. Apart from image augmentation, batch normalisation (in each layer) and dropout in the dense layer is used. 

The results without image augmentation: 82.8% test accuracy, clearly overfitting!

![alt text](https://user-images.githubusercontent.com/33765868/34697327-e6a67af6-f4d2-11e7-88ad-3c81b4615cdc.png)

With Image augmentation (rotation, horizontal flip, shifts): 90.3% test accuracy, still rising after 100 epochs (ca. 2h training)

![alt text](https://user-images.githubusercontent.com/33765868/34697363-0fc85b52-f4d3-11e7-882c-f779cf96b846.png)
