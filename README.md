# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
<br>


### Step2:
Create the Text using cv2.putText.
<br>

### Step3:
Create the structuring element.
<br>

### Step4:
Use Opening operation
<br>

### Step5:
Use Closing Operation
<br>

 
## Program:
Developed by:JEEVAGOWTHAM S
Register Number:212222230053

# Import the necessary packages:
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
```



# Create the Text using cv2.putText:
```
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
cv2.putText(img1,'JEEVAGOWTHAM',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='magma')
plt.title('Input Text'), plt.xticks([]), plt.yticks([])
plt.show()
```



# Create the structuring element:
```
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```



# Use Opening operation:
```
image1=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernel1)
plt.imshow(image1,cmap='gray')
plt.title('OPENING'), plt.xticks([]), plt.yticks([])
plt.show()
```




# Use Closing Operation:
```
image1=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel1)
plt.imshow(image1,cmap='gray')
plt.title('CLOSING'), plt.xticks([]), plt.yticks([])
plt.show()
```





## Output:

### Display the input Image:
![Screenshot 2023-10-18 081938](https://github.com/JeevaGowtham-S/OPENING--CLOSING/assets/118042624/8d82ec9c-4e98-40d4-b1ba-777042ea3a40)

<br>
<br>
<br>
<br>
<br>
<br>

### Display the result of Opening
![Screenshot 2023-10-18 082527](https://github.com/JeevaGowtham-S/OPENING--CLOSING/assets/118042624/f532686f-a03b-4dd6-8215-36395f643ee1)

<br>
<br>
<br>
<br>
<br>
<br>

### Display the result of Closing
![Screenshot 2023-10-18 082607](https://github.com/JeevaGowtham-S/OPENING--CLOSING/assets/118042624/aafe4464-fd47-411f-a8a2-71e08612cef7)

<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
