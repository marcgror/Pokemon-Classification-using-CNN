# Pokemon-Classification-using-CNN
## Introduction
In this project I will try to train and design a CNN for classifying pokemons from images.
Initially, I tried to approach the task by using the 808 existing pokemons as different classes, with very few images per class. Obviously, I soon realized that this was a very hard (impossible?) approach. Then, I ended reducing the number of classes to only 5 (finally 7), collecting more images per class and using Image Augmentation to gain more training data.

Image Augmentation works by applying transformations, as rotations, flips or zooming, to the training data, to finally increase the amount of train data available for fedding the CNN, while having a more different data that could end in a more generalized model.
## Data
ATM, the pokemons to classify are:
- Bulbasaur
- Pikachu
- Mew
- Mewtwo
- Vulpix
- Palkia
- Kyogre

The data (images) used in the project are available in the 'data' folder, divided in train, validation and test folders. Train and validation have 7 folders, one per class/pokemon, with a total of 100 training images and 28 validation images, counting all the classes (not for each class). These images have been extracted from Internet, and the reason for working with very few images is that I wanted to use Image Augmentation to generate more training and validation data, and that I didn't want to download manually hundreds or thousands of pokemon images.

Finally, in the test folder one can find 8 images that will be used to predict the class once the model is trained.
## Results
Once trained, the model correctly predicted the pokemon shown in each one of the test images. There is no doubt that this is a very, very simple model, but I wanted to see how Image Augmentation works in case you don't have acces to hundreds or thousands of images per class, in contrast with famous datasets like MINST or Fashion-MNIST.
## Future work
I am thinking in periodically add new pokemons/classes, with the same ratio of images, to see how it impacts in the performance of the model. 