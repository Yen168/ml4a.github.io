---
layout: guide
title: "convnetClassifier"
---
### What is it?

ConvnetClassifier is an [openFrameworks](http://www.openframeworks.cc) application, part of the [ml4a-ofx collection](https://github.com/ml4a/ml4a-ofx/), which lets you train a classifier to recognise whatever objects, persons, postures, drawings and other visuals you show it through your webcam. 

{:.center}
![convnetClassifier gif](http://andreasrefsgaard.dk/wp-content/uploads/2016/12/ConvnetClassifier.gif)

ConvnetClassifier has been used by [Bjørn Karmann](http://bjoernkarmann.dk/) in his [Objectifier](http://bjoernkarmann.dk/objectifier) project, which empowers people to train objects in their daily environment to respond to their unique behaviours.

<center>
<iframe src="https://player.vimeo.com/video/195086230" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</center>


## Training instructions

1. Make sure your camera sees your intended visuals for class 1. Press "r" to toggle recording of training examples.

2. Press [2] to switch the class label and press [r] to record examples of a different class.

3. Repeat this for class 3 or however many distinct things you intend to classify. Remember to change the classes by pressing the numeric keys accordingly. 

4. Press [t] to train the model.

5. Show the webcam different visuals and see what class the model predicts.

The video below takes you through the steps of the training process.

<center>
<iframe src="https://player.vimeo.com/video/197502261" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</center>


## Setup and training considerations
ConvnetClassifier is a very versatile application that can be used in a wide variety of setups. However, to optimise correct classification, some simple rules of thumbs are:

* Ensure variety in your training data: Say you want to classify whether someone is holding an object in their hands, try to record training samples that shows the person holding the object in different postures and positions, close to the camera, far from the camera, in both hands etc. 

* Keep your settings stable when using small training samples: Training in different sets of lighting conditions and hereafter attempting to classify in yet another environment might prove difficult. The same is true for camera positions and angles, backgrounds, etc. Unless you intentionally want a classifier that is can handle different settings (which would require more training examples), you can save yourself a lot of sweat by keeping your physical setup stable. 

* If the classification is not accurate enough, try to record more training examples. Alternatively you can try different classifier algorithms: Choose between different algorithms by pressing [tab] and retrain you model by pressing [t].

 








