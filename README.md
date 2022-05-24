# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Step1: Import the necessary packages.

### Step2:
Step2: Create the Text using cv2.putText.



### Step3:
Step3: Create the structuring element.


### Step4:
Step4: Erode and Dilate the image.


### Step5:
Step5: End Program.


 
## Program:

``` Python
NAME:V.A.JITHENDRA
REF NO:212221230043
# Import the necessary packages

import cv2
import numpy as np
import matplotlib.pyplot as plt


# Create the Text using cv2.putText
image= np.zeros((100,400),dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image,'JITHENDRA',(5,70), font,2,(255),5,cv2.LINE_AA)
cv2.imshow("Name",image)


# Create the structuring element
kernel1 = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))



# Erode the image
erodeImage = cv2.erode(image,kernel1)
cv2.imshow("Erode Image",erodeImage)




# Dilate the image

dilationImage = cv2.dilate(image,kernel1)
cv2.imshow("Dilated Image",dilationImage)



cv2.waitKey(0)
cv2.DestroyAllWindows




```
## Output:

### Display the input Image
![NAME](https://user-images.githubusercontent.com/94226297/169949022-3d57e2c6-6d9b-4713-a504-f7b21790c564.png)


### Display the Eroded Image
![ERODE](https://user-images.githubusercontent.com/94226297/169949046-60f8376d-45fa-4d69-b347-9ad940490461.png)


### Display the Dilated Image

![DILATED](https://user-images.githubusercontent.com/94226297/169949064-4c448b35-4625-4683-a64d-21fa279b7aeb.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
