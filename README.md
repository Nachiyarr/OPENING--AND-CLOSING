# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Read the image

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: ALAGU NACHIYAR K
Register NO: 212222240006
```
``` Python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText
img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'JANANI.V.S', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)

# Create the structuring element
struct_ele = np.ones((9, 9), np.uint8)

# Use Opening operation
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)

# Use Closing Operation
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)

# Close all windows
cv2.destroyAllWindows()
```
## Output:

### Display the input Image
![WhatsApp Image 2024-04-23 at 10 36 25_ab61cb9d](https://github.com/Nachiyarr/OPENING--AND-CLOSING/assets/113497340/26dfbe1d-c829-4126-89a4-e496f66aa910)


### Display the result of Opening
![WhatsApp Image 2024-04-23 at 10 36 45_069da64a](https://github.com/Nachiyarr/OPENING--AND-CLOSING/assets/113497340/fe12a7a1-89ad-410b-9715-6f8a89eb328a)



### Display the result of Closing
![WhatsApp Image 2024-04-23 at 10 37 33_89462e7e](https://github.com/Nachiyarr/OPENING--AND-CLOSING/assets/113497340/0cfd6df1-ed35-4ed7-9510-1fdba7d9ed08)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
