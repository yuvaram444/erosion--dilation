# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary pacakages
<br>

### Step2:
Create the text using cv2.putText
<br>

### Step3:
Create the structuring element
<br>

### Step4:
Erode the image
<br>

### Step5:
Dilate the Image
<br>

 
## Program:
```
NAME : YUVARAM S
REG NO : 212224230315
```
# Import the necessary packages
```
import cv2
import numpy as np
from matplotlib import pyplot as plt
```
# Create the Text using cv2.putText
```
# Load the image
img1=np.zeros((100,700),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL

# Create the text using cv2.putText
cv2.putText(img1,'YUVARAM S' ,(5,70),font,4,(255),2,cv2.LINE_AA)
```
# Create the structuring element
```
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(5,5))
```
# Erode the image
```
img_dilate=cv2.dilate(img1,kernel1)
img_erode=cv2.erode(img1,kernel1)
```
# Dilate the image
```
plt.figure(figsize=(12, 5))
plt.subplot(1,3,1)
plt.imshow(img1,cmap='gray')
plt.subplot(1,3,2)
plt.imshow(img_dilate,cmap='gray')
plt.subplot(1,3,3)
plt.imshow(img_erode,cmap='gray')
```
## Output:

### Display the input Image
<br>
<br>
<br>

<br>![Screenshot 2025-05-06 155910](https://github.com/user-attachments/assets/bfbfbf28-5839-4378-8c22-692882c7e93f)

<br>
<br>

### Display the Eroded Image
<br>
<br>
<br>

<br>![Screenshot 2025-05-06 160155](https://github.com/user-attachments/assets/c0b58698-0644-4971-a9e3-7221bd690c79)

<br>
<br>

### Display the Dilated Image
<br>
<br>
<br>

<br>![Screenshot 2025-05-06 160208](https://github.com/user-attachments/assets/cfa0d26e-5c72-4e19-8315-67b8894ed46c)

<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
