# Dog Breed Classifier

* Given an image of a dog, "Dog Breed Classifier" will identify an estimate of the canine’s breed.
* If supplied an image of a human, "Dog Breed Classifier" will identify the resembling dog breed.
* Used the ImageNet dataset for training.
* Augmented the training images by random resizing, horizontal fliping and rotating the training data set images.
* Augmented the validation and test images by center cropping.
* Used the CV2 library to build a human face detector.
* Used a pretrained VGG-16 model for detecting dogs in images.
* A plain vanilla CNN models built from scratch is used for classifying dog images.
* Also tried out the pre-trained resnet-50 models and fine tuned them to classify dog images.
* Was able to achieve Test Accuracy of 13% using the plain vanilla CNN network.
* Was able to achieve Test Accuracy of 81% using the ResNet50 pre-trained model using transfer learning.
* Implemented a final "run_app" method that predicts the dog breed given a dog image, predicts the most closeley matching dog breed if given a human image.
* Points of future improvements: Create a mobile app and call the "run_app" method to do classification from the images clicked from the mobile phone, try more pre-trained models and compare the results, train for more number of epochs and use a deeper network. 