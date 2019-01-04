# webcam-image-classifier
Fun project with Keras and cv2 to capture images from my webcam, feeding them to a Convolutional NN and doing live predictions from the webcam video stream

Project consist of 2 notebooks for Black & White and Color images as I want to experiment with them differently, each notebook begins with a cell allowing you to capture images from a webcam by pressing "r" on your keyboard, the capture stops when you reach 1000 pics or you press the "e" key

You can save then the pictures (already transformed to a normalised numpy array) to disk in pickle format and load them all at once into memory.
After some image preprocessing, the pictures are used to train a Convolutional Neural Network built in keras, the model is then used live while displaying the current video stream from the webcam to show live prediction for the object you are pointing at.

I've transferred the code for the B/W version to Google CoLab https://colab.research.google.com/drive/17aZ-79nP_TE6CbJMVi2kfKEexrMHMrgX in order to do the training on cloud, once the model is trained I save it back to my machine and do the live prediction, unfortunately the training data needs to be re-uploaded every session
