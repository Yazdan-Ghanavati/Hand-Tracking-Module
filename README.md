# Hand Tracking Module
This is a computer vision project, which is specifically developed in order to detect and track human hands.
All the code is written in python and available in the repo for public.

## Libraries
* OpenCV 4.5.3.56
* Mediapipe 0.8.3

## what is Mediapipe hand solution?
In 2019, Google released a deep learning module called Mediapipe which allows users to detect and track various 
body parts in their computer vision projects with a frame rate of 30. This library runs on CPU and does not
require GPU for processing and is currently the fastest method of detection in the market.
This specific module is able to find hands in a frame and return a list of 21 landmarks which allows user to have
access to the position of each point. These kind of information could be used for healthcare purposes and lead to
design and develop various telemedicine applications.

![image](https://github.com/Yazdan-Ghanavati/Hand-Tracking-Module/assets/137007531/b92816db-7867-4a0f-95a4-b7e659a5ab34)

![image](https://github.com/Yazdan-Ghanavati/Hand-Tracking-Module/assets/137007531/c6f9436b-07cf-45fc-abdf-9eb3a9db46bf)

## Functions
This module is consisted of various functions which are listed below:
* findHands
* fingersUp
* findDistance

### findHands
This function will get the input image from webcam and process it in order to find all the hands in the frame.
Although, it can detect everything, it will only print based on the limitations that user set for it. Finally,
it will return a list of hands and also a landmark list for each of them including position of every landmark in all
3 directions.  


### fingersUp
This function will detect whether a finger is open or closed by comparing the Y-value of the tip of each finger with
its first knuckle. However, for the thumb finger, based on calculating the right or left hand, it will focus on the 
X axis value.
This function could also be used in treatment of Osteoarthritis which requiers opening and closing hands with
specific timing.


![image](https://github.com/Yazdan-Ghanavati/Hand-Tracking-Module/assets/137007531/375a49fd-822d-430a-ae3d-888d3668b64d)

![Screenshot (78)](https://github.com/Yazdan-Ghanavati/Hand-Tracking-Module/assets/137007531/646e3f27-a20d-4b93-968d-c2218b4adf5b)


### findDistance
This is an extremely important function which can calculate the distance between two landmarks. This function can
be applied to various projects. For instance: system volume change, Zooming pictures, etc.




