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
### Developed By:JANANI.R
### Register Number: 212221230039

i) #To Read,display the image
```
import cv2s
import matplotlib.pyplot as plt
img=cv2.imread("coffee.jpeg",1)
cv2.imshow("cup",img)
cv2.waitKey(0)
```
ii) #To write the image
```
import cv2
image=cv2.imread("coffee.jpeg",1)
w=cv2.imwrite("cup",image)
cv2.cv2.imshow("coffee.jpeg",1)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```
import cv2
imgg=cv2.imread("coffee.jpeg",1)
print(imgg.shape)
```
iv) #To access rows and columns

```
import random
import cv2
A=cv2.imread("coffee.jpeg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("coffee.jpeg",A)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color_img = cv2.imread("coffee.jpeg",1)
tag = color_img[200:400,300:500]
color_img[300:500,200:400] = tag
cv2.imshow('Cut And Paste',color_img)
cv2.waitKey(0)
```


## Output:

### i) Read and display the image
![cf1](https://user-images.githubusercontent.com/94288340/225951171-167431d1-a685-4929-aae2-40c3248f47b5.png)

### ii)Write the image
![cf2](https://user-images.githubusercontent.com/94288340/225951245-c9048d10-525c-452f-afe9-ba93e120a2dd.png)

### iii)Shape of the Image
![cf3](https://user-images.githubusercontent.com/94288340/225951271-4db069e9-9933-4ad4-9da2-f58e8cf5ab12.png)

### iv)Access rows and columns
![cf4](https://user-images.githubusercontent.com/94288340/225951289-df9bfbdf-cdad-4885-8acf-d18e43b8e538.png)


### v)Cut and paste portion of image
![cf5](https://user-images.githubusercontent.com/94288340/225951318-c063826b-0832-46fe-b9f0-fbb391f15e92.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


