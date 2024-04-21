# OPENING-AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
### Step2:
Create the Text using cv2.putText
### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by: Sri Varshan P
Register Number:212222240104
```
### Display the input Image
```py
import cv2
import numpy as np

img=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'Sri Varshan',(5,70), font,2,(255),5,cv2.LINE_AA)
cv2.imshow('Sample', img)
cv2.waitKey(0)
```
### Create the structured element
```py
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```py
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```py
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image

![image](https://github.com/PSriVarshan/OPENING--AND-CLOSING/assets/114944059/39919453-0f91-407a-96de-8fe5b284000d)


### Display the result of Opening

![image](https://github.com/PSriVarshan/OPENING--AND-CLOSING/assets/114944059/aec1018a-86f0-49c6-93f2-b897e93d5167)


### Display the result of Closing

![image](https://github.com/PSriVarshan/OPENING--AND-CLOSING/assets/114944059/8e22855a-131b-4d87-b27d-a6209e5e8b25)


## Result

### Thus the Opening and Closing operation is used in the image using python and OpenCV.
