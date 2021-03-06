# No Internet game using RL, Selenium and PyAuto gui:

This repo contains my version of the already implemented Dino game played using Deep-Q Learning.
As a few others have already implemented this project, I did the same and defnitely learnt a lot.

## Unique Functionalitites:

* ***Bug-free code***; the other repos had ***many inconsistencies*** that had to be resolved.
* ***Added duck function*** by using PyAutoGUI
  * Accessing the duck function directly created a problem of the website scrolling down. Therefore, we used PyAutoGUI to resolve this issue. Also, we used a boolean variable to keep track of the same. 
* Trained the model and adjusted the hyperparameters to better suit the performance of the model.
* Created a ***simpler version of Double DQN***, but we haven't realeased it as it requires more work.
* ***Removed irrelevant and redundant functions***; Simpler pipeline used for processing the images.

## Tools & Technologies:
* Python 3.6 >
* JavaScript 
* Selenium 
* OpenCV
* PyAutoGUI
* Tensorflow
* Google Chrome

### Selenium:
Selenium is a portable framework for testing web applications. However, selenium was not used for testing; it was used to ***access*** the website where the game was hosted. Using selenium to access is all good, but we also used it to play the game by, in a way, ***interfacing*** between the script file and the website.

We used Selenium's Chrome driver to access and control the website through Google Chrome. 

### OpenCV:
OpenCV (Open Source Computer Vision Library) is an open source computer vision and machine learning software library. 
We used OpenCV to:
* ***Grab relevant screenshots*** from the screenshot captured by Selenium.
* Process these screenshots
* Convert to tensors for the model
* And, output the grabbed images at run-time

### Model:
We implemented a ****Deep-Q network*** using Keras & Tensorflow by taking the stacked-processed image as input and outputted a probability of actions.


