# Dog Breed Classifier

* "Dog Breed Classifier" detects the breed of a dog in the supplied image. If supplied image contains a human face, it will try to find a dog breed that closely matching the face of the human in the image.
* Used the ImageNet dataset for training the classifier.
* Augmented the training images by random resizing, horizontal fliping and rotating the training data set images.
* Augmented the validation and test images by center cropping.
* Used the CV2 library to build a human face detector.
* Used a pre-trained VGG-16 model for detecting dogs in images.
* A plain vanilla CNN models built from scratch is used for classifying dog images.
* Also tried out the pre-trained resnet-50 models and fine tuned them to classify dog images.
* Was able to achieve Test Accuracy of 13% using the plain vanilla CNN network.
* Was able to achieve Test Accuracy of 81% using the ResNet50 pre-trained model using transfer learning.
* Implemented a final "run_app" method that predicts the dog breed given a dog image, predicts the most closely matching dog breed if given a human image.
* Points of future improvements: Create a mobile app and call the "run_app" method to do classification from the images clicked from the mobile phone, try more pre-trained models and compare the results, train for more number of epochs and use a deeper network. 