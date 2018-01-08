# Image Augmentation in Keras (CIFAR-10)
Using image augmentation to reach 90.3% accuracy on CIFAR_10 with a simple CNN. 

Machine learning works best when there is plenty of training data (in this case images), since this prevents overfitting of the model. If the training data is limited, one can artificilly increase it by image augmentation. Here additional images are created by rotating, shifting, zooming or other operations on the original training image.
In my case, I reach over 90 percent classificaion accuracy on CIFAR_10, a dataset with 50 000 training images in 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship and truck). I tried different operations, the best seemed to be rotations, horizontal flipping and vertical or horizontal shifts.
The model is a VGG-type convolutional network with 6 conv layers and one dense fully connected layer before the output. Apart from image augmentation, batch normalisation (in each layer) and dropout in the dense layer is used. 

The results without image augmentation: 82.8% test accuracy, clearly overfitting!








