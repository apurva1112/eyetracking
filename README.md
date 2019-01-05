# eyetracking
upload eye-tracking code here

1. You can download the dlib's pre trained shape detector from here: http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2

2.This code is the implementation of this paper: https://pdfs.semanticscholar.org/81d5/c4b49fe17aaa3af837745cafdedb066a067d.pdf

# Description
This code does live tracking of eye pupil and plays a siren if the eyes are closed.

# Requisites
This code has been run and tested on following python libraries:
1.dlib                   -  v19.15.0  2.imutils                -  v0.4.6  3.numpy                  -  v1.15.0  4.opencv-contrib-python  -  v3.4.2.17  5.pygame                 -  v1.9.4  6.scpiy                  -  v1.1.0

# Documentation
Inside the while loop, the webcam continuously captures images, the eye image processing is done and the required actions are carried out. The line "time.sleep(1.0)" ensures that a single image is captured in every 2 seconds. If this is not done, the white pupil locator on image will be unstable. The functions sound_alarm_on(path) and sound_alarm_off() are used to play and stop the alarm respectively when called.
