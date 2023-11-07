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
Developed by:S VAISHNAV NANDA
Register Number:212222240112

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
cv2.putText(img1,'VAISHNAV',(5,70),font,2,(255),5,cv2.LINE_AA)
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
![Screenshot from 2023-11-07 14-14-11](https://github.com/VaishnavNanda/OPENING--CLOSING/assets/118707051/8f6147c4-b2f4-4785-a542-e2f60a9cdb1e)



<br>
<br>
<br>
<br>
<br>
<br>

### Display the result of Opening
![Screenshot from 2023-11-07 14-14-20](https://github.com/VaishnavNanda/OPENING--CLOSING/assets/118707051/efabecd4-e635-4b6a-b582-8215344d4d3d)


<br>
<br>
<br>
<br>
<br>
<br>

### Display the result of Closing
![Screenshot from 2023-11-07 14-14-28](https://github.com/VaishnavNanda/OPENING--CLOSING/assets/118707051/49c5faf8-97d6-4cf9-b378-20693e5fec49)


<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
