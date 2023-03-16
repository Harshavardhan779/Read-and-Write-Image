# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: Harshavardhan
### Register Number: 21222240114
i) #To Read,display the image
```python
### Developed By: HARSHAVARDHAN
### Register Number: 212222240114
import cv2
spd_mn=cv2.imread('flower.jpeg',1)
cv2.imshow('HARSHA(220007173)',spd_mn)
cv2.waitKey(0)
  

```
ii) #To write the image
```python
### Developed By: HARSHAVARDHAN
### Register Number: 212222240114

import cv2
A=cv2.imread("flower.jpeg",1)
cv2.imwrite("flower.jpeg",A)
cv2.imshow("(HARSHA)212222240114",A)
cv2.waitKey(0)




```
iii) #Find the shape of the Image
```python
### Developed by : Harshavardhan
### Reference no:21222240114

import cv2 
colorImage = cv2.imread('flower.jpeg',1)
print(colorImage.shape)



```
iv) #To access rows and columns

```python
### Developed by : Harshavardhan
### Reference no:21222240114
import random
import cv2
A=cv2.imread("flower.jpeg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("HARSHA(212222240114)",A)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```python
### Developed by:Harshavardhan
### Reference no: 21222240114

import cv2
color_img = cv2.imread('flower.jpeg',1)
tag = color_img[20:80,20:80]
color_img[90:150,90:150] = tag
cv2.imshow('Cut And Paste',color_img)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image


![OUTPUT](/Screenshot%20from%202023-03-15%2011-13-52.png)

### ii)Write the image
![OUTPUT](/write.png)
<br>
<br>

### iii)Shape of the Image
![OUTPUT](/Screenshot%20from%202023-03-16%2010-50-22.png)
<br>
<br>

### iv)Access rows and columns
![OUTPUT](/access.png)
<br>

<br>

### v)Cut and paste portion of image

![OUTPUT](/cut.png)
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


