# Histogram-of-an-images
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()

### Step2:
Print the image using imshow().



### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### Step5:
The Histogram of gray scale image and color image is shown.


## Program:
```python
# Developed By: Divadharshini.A
# Register Number: 212222240027






```
## Output:
### Input Grayscale Image and Color Image

 #import cv2
 #import matplotlib.pyplot as plt
 #gray_image = cv2.imread("i1")
 #color_image = cv2.imread("i3",-1)
 #cv2.imshow("Gray Image",gray_image)
 #cv2.imshow("Colour Image",color_image)
 #cv2.waitKey(0)
 #cv2.destroyAllWindows()


### Histogram of Grayscale Image and any channel of Color Image

import numpy as np
import cv2
Gray_image = cv2.imread("i1")
Color_image = cv2.imread("i3")
import matplotlib.pyplot as plt
gray_hist = cv2.calcHist([Gray_image],[0],None,[256],[0,256])
color_hist = cv2.calcHist([Color_image],[0],None,[256],[0,256])
plt.figure()
plt.imshow(Gray_image)
plt.show()
plt.title("Histogram")
plt.xlabel("Grayscale Value")
plt.ylabel("Pixel Count")
plt.stem(gray_hist)
plt.show()
plt.imshow(Color_image)
plt.show()
plt.title("Histogram of Color Image - Green Channel")
plt.xlabel("Intensity Value")
plt.ylabel("Pixel Count")
plt.stem(color_hist)
plt.show()
cv2.waitKey(0)



### Histogram Equalization of Grayscale Image.

import cv2
gray_image = cv2.imread("i1",0)
cv2.imshow('Grey Scale Image',gray_image)
equ = cv2.equalizeHist(gray_image)
cv2.imshow("Equalized Image",equ)
cv2.waitKey(0)
cv2.destroyAllWindows()


### Input Grayscale Image and Color Image

![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/9801f458-1295-4faf-87af-2e1380afbdb7)


![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/46ef8bc9-bd11-4550-930b-3137d5aabeae)


### Histogram of Grayscale Image and any channel of Color Image

![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/93e79803-f95d-4557-b9dc-be8c485061d1)


![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/23323c55-041d-49a9-8cc8-733c096d7202)

![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/338f813f-fa85-40e3-86e6-6337cc8adde5)

![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/4e2a1931-408e-4b86-af8a-db3d8454f9ab)


### Histogram Equalization of Grayscale Image.

![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/fd932d53-3972-4543-8cab-5bb909df78b9)

![image](https://github.com/divyadharshiniddanbarasu/Histogram-of-an-images/assets/119393424/58f64f5c-b22e-4b9d-b5d0-41a01ea9e485)


## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
