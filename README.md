![Screenshot 2023-08-29 083152](https://github.com/Yamunaasri/READ-AND-WRITE-IMAGE/assets/115707860/ee178edb-4456-4043-8bf2-c997f0d9efe6)# READ AND WRITE AN IMAGE
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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('waterb.jpg',1)
cv2.imshow('212222240117_Yamunaasri',color_image)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
img = cv2.imread('waterb.jpg', 1)
new_img = cv2.imwrite('waterb.jpg', img)
cv2.imshow('212222240117_yamunaasri', img)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```

import cv2
img = cv2.imread('waterb.jpg', 1)
print(img.shape)

```
iv) #To access rows and columns

```
import cv2
import random
img = cv2.imread('waterb.jpg', 1)
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
cv2.imshow('part image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```
import cv2
img = cv2.imread('waterb.jpg', 1)
tag = img[200:400, 200:400]
img[200:400,600:800] = tag
cv2.imshow('212222240117_Yamunaasri', img)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image
![Screenshot 2023-08-29 083152](https://github.com/Yamunaasri/READ-AND-WRITE-IMAGE/assets/115707860/af8c0696-c065-48e6-8450-e4c49614da04)


<br>
<br>

### ii)Write the image
![Screenshot 2023-08-29 083222](https://github.com/Yamunaasri/READ-AND-WRITE-IMAGE/assets/115707860/3b534907-2922-4018-a114-890382613f02)


<br>
<br>

### iii)Shape of the Image
![Screenshot 2023-08-29 084954](https://github.com/Yamunaasri/READ-AND-WRITE-IMAGE/assets/115707860/bad66dde-0db0-4c30-b6bd-190e4a30f4cc)

<br>
<br>

### iv)Access rows and columns
![Screenshot 2023-08-29 083246](https://github.com/Yamunaasri/READ-AND-WRITE-IMAGE/assets/115707860/3a412f8a-1082-4d57-b4bf-852ecaccc88c)

<br>
<br>

### v)Cut and paste portion of image
![Screenshot 2023-08-29 084800](https://github.com/Yamunaasri/READ-AND-WRITE-IMAGE/assets/115707860/abd50101-10ad-4d2a-956b-64b3e21ca707)

<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
