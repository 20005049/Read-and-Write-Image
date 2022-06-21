## EXP NO:01
## DATE:
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
```python
# Developed By:Sri Harish M
# Register Number : 212220230047
# To Read,display the image
import numpy as np
import cv2
img = cv2.imread('tiger.jpg',1)
cv2.imshow('Bike',img)
cv2.waitKey(0)
# To write the image
cv2.imwrite('tiger1.jpg',img)
# Find the shape of the Image
print(img.shape)
# To access rows and columns
import random
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j]= [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('tiger',img)
cv2.waitKey(0)
# To cut and paste portion of image
bw2=cv2.imread("tiger.jpg",1)
tag=bw2[30:100,30:120]
bw2[50:120,120:210]=tag
cv2.imshow("cutting portion",bw2)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## Output:

### i) Read and display the image

![ss1](https://user-images.githubusercontent.com/75241366/160880834-85acd9de-48d3-41f4-bde6-0b7fe1bdf3a1.jpg)

### ii)Write the image
![ss2](https://user-images.githubusercontent.com/75241366/160880852-d7092e2b-9dc2-4e1c-9db7-81c459dca475.jpg)



### iii)Shape of the Image
![ss2](https://user-images.githubusercontent.com/75241366/160880869-418b6102-62cb-4eae-9f23-6488d19f59fc.jpg)


### iv)Access rows and columns
![ss3](https://user-images.githubusercontent.com/75241366/160880890-42412bcf-647c-4cf7-9f0f-0f9022f6d1a8.jpg)


### v)Cut and paste portion of image
![ss4](https://user-images.githubusercontent.com/75241366/160880909-279cd630-8793-40e5-a724-577b13f53dba.jpg)


## Result:
Thus the images are read, displayed, and written successfuLly using the python program.


