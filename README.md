# Opening-and-Closing

# Aim :

To implement Opening and Closing using Python and OpenCV.

# Software Required :

1. Anaconda - Python 3.7
2. OpenCV

# Algorithm :

## Step 1 :

Import the necessary packages.

## Step 2 :

Create the Text using cv2.putText

## Step 3 :

Create the structuring element.

## Step 4 :

Use Opening operation.

## Step 5 :

Use Closing Operation.
 
# Program:

## DEVELOPED BY : ABRIN NISHA A
## REGISTER NO : 212222230005

### Import the necessary packages :

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

### Create the Text using cv2.putText :

```python
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'U Bhavya',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```

### Create the structuring element :

```python
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```
### Use Opening operation :

```python
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```
### Use Closing Operation :

```python
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()
```
# Output :

## Display the input Image :
![Screenshot 2023-05-10 143459](https://github.com/Abrinnisha6/Opening-and-Closing/assets/118889454/fa98eeb3-13ba-47df-a102-7d8bf3ed89d1)


## Display the result of Opening :

![Screenshot 2023-05-10 143855](https://github.com/Abrinnisha6/Opening-and-Closing/assets/118889454/c7b25613-a3e7-4721-a4df-97689d8eb7bd)


## Display the result of Closing :

![Screenshot 2023-05-10 143937](https://github.com/Abrinnisha6/Opening-and-Closing/assets/118889454/a9d51400-65c1-4495-bc8e-7f82b670b312)


# Result :

Thus the Opening and Closing operation is used in the image using python and OpenCV.
