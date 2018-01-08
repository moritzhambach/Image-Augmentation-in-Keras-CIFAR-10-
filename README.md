# Image-Augmentation-in-Keras-CIFAR-10-
Using image augmentation to reach 90.3% accuracy on CIFAR_10 with a simple CNN. 

Machine learning works best when there is plenty of training data (in this case images), since this prevents overfitting of the model. If the training data is limited, one can artificilly increase it by image augmentation. Here additional images are created by rotating, shifting, zooming or other operations on the original training image.
In my case, I reach ver 90 percent classificaion accuracy on CIFAR_10, a dataset with 50 000 training images in 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship and truck). I tried different operations, the best seemed to be rotations, horizontal flipping and vertical or horizontal shifts.






