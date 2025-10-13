# karthikeyanpachiyappan-Record-IMPLEMENTATION-OF-EROSION-AND-DILATION
# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import required libraries (OpenCV, NumPy) and load the image in grayscale

### Step2:
Define a structuring element (kernel) for morphological operations.

### Step3:
Apply erosion using cv2.erode() on the image with the defined kernel.

### Step4:
Apply dilation using cv2.dilate() on the image with the same kernel.

### Step5:
Display and compare the original, eroded, and dilated images.
 
## Program
## Developed by:KARTHIKEYAN P
### Reg NO: 212223230102
``` 
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
```
image = np.zeros((600, 600), dtype=np.uint8)
cv2.putText(image,text='KARTHI',org=(50,300),fontFace=cv2.FONT_HERSHEY_SIMPLEX,fontScale=5,color=(255,255,255),thickness=25,lineType=cv2.LINE_AA)
plt.imshow(image,cmap='gray')
plt.axis('off') 
plt.show()
```
```
kernel = np.ones((10, 10), np.uint8)
eroded_image = cv2.erode(image, kernel, iterations=1)
```
```
plt.imshow(eroded_image,cmap='gray')
plt.title("Eroded Image")
plt.axis('off')
```
```
dilated_image = cv2.dilate(image, kernel, iterations=1)
```
```
plt.imshow(dilated_image,cmap='gray') 
plt.title("Dilated Image")
plt.axis('off')
```
## Output:

### Display the input Image
<img width="554" height="496" alt="Screenshot 2025-10-13 111346" src="https://github.com/user-attachments/assets/1fae756d-836f-4d83-8577-ec956cb86cd0" />

### Display the Eroded Image
<img width="641" height="516" alt="Screenshot 2025-10-13 111642" src="https://github.com/user-attachments/assets/15132d0f-07bf-449b-b264-191648c048e8" />

### Display the Dilated Image
<img width="674" height="525" alt="Screenshot 2025-10-13 111706" src="https://github.com/user-attachments/assets/83a8ce0a-b5e1-40a5-9a5b-7ea5f6a18b89" />

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
