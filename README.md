# GestureVolumeControl

This program will control the volume of your computer depending on the distance between the tip of your index finger and the tip of your thumb.

To help us detect the hand landmarks mediapipe by Google has been used. It uses machine learning to track the movements of your palm using 21 reference points. You can find more about mediapipe here->(https://google.github.io/mediapipe/solutions/hands)

Download mediapipe with the following command- ```pip install mediapipe```

To access the computer's sound setting a library called pycaw developed by Andres Miras has been used. Python Core Audio Windows Library(pycaw), it works for both Python2 and Python3.You can find more about pycaw here->(https://github.com/AndreMiras/pycaw)

Download pycaw with the following command- ```pip install pycaw```

The palm is tracked using 21 reference points. These reference points are predefined. The reference points are as follows-

![image](https://user-images.githubusercontent.com/47482433/121740885-5bd25a80-cb1b-11eb-8501-9270fb396746.png)

We will be using landmarks numbered 4(thumb) and 8(index finger).

After executing the program a camera window will open up, you will be able to see your index fingertip adn thumb tip being tracked in this camera window. When the distance increases between those the fingertips the volume will increase and when the distance decreases the volume will decrease. This program also shows the frame rate in the top left corner of the camera window once the program is executed.

To increase the sensitivity of increase/decrease in volume bring the palm closer to the camera and to decrease the sensitivity take the plam away from the camera.

Libraries used-> cv2(opencv), math, numpy, time, mediapipe, ctypes, comtypes, pycaw.
