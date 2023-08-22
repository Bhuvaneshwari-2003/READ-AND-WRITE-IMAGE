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
```
#Developed By: BHUVANESHWARI.S
#Register Number: 212221240010

#To Read,display the image

#Color image:

import cv2
blk_wd=cv2.imread('Logo.jpg',1)
cv2.imshow('Avengers',blk_wd)
cv2.waitKey(0)

#Grayscale image: 

import cv2
b_w=cv2.imread('Logo.jpg',0)
cv2.imshow('Avengers',b_w)
cv2.waitKey(0)

# To write the image

import cv2
blk_wd=cv2.imread('Logo.jpg',1)

cv2.imwrite('Avengers real.jpg',blk_wd)


# Find the shape of the Image

import cv2
blk_wd=cv2.imread('Logo.jpg',1)

print(blk_wd.shape)

# To access rows and columns

import cv2
blk_wd=cv2.imread('Logo.jpg',1)

import random
for i in range(450):
    for j in range(blk_wd.shape[1]):
        blk_wd[i][j] = [random.randint(0,235),random.randint(0,225),random.randint(0,205)]
cv2.imshow('Avengers Part',blk_wd)
cv2.waitKey(0)

# To cut and paste portion of image

import cv2
blk_wd=cv2.imread('Logo.jpg',1)

tag = blk_wd[300:400:,300:400]
blk_wd[50:150,50:150] = tag
cv2.imshow('Avengers cut part',blk_wd)
cv2.waitKey(0)
```


## Output:

### i) Read and display the image
colour image:
![1](https://github.com/Bhuvaneshwari-2003/READ-AND-WRITE-IMAGE/assets/94828604/6c5ccfac-e80e-47b5-82e6-e1371c1e1adb)
Grayscale Image:


### ii)Write the image
![31](https://github.com/Bhuvaneshwari-2003/READ-AND-WRITE-IMAGE/assets/94828604/0bd5a703-52f2-4b4a-9012-e94a0403fd93)
![32](https://github.com/Bhuvaneshwari-2003/READ-AND-WRITE-IMAGE/assets/94828604/f6ef0b3a-b3a1-4694-8fe6-cf193ce1aa77)


### iii)Shape of the Image
![4](https://github.com/Bhuvaneshwari-2003/READ-AND-WRITE-IMAGE/assets/94828604/5d4c295b-5a76-416e-902b-6728f0cbd539)


### iv)Access rows and columns
![5](https://github.com/Bhuvaneshwari-2003/READ-AND-WRITE-IMAGE/assets/94828604/8e8a2f1c-0e86-4453-9376-91ed29c9b402)


### v)Cut and paste portion of image
![6](https://github.com/Bhuvaneshwari-2003/READ-AND-WRITE-IMAGE/assets/94828604/84a4b6c2-e565-4306-8d05-aa80438cac68)

## Result:
Thus the images are read, displayed, and written successfully using the python program.
