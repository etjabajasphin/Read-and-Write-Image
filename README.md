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
### Developed By: Shyam Kumar A
### Register Number: 212221230098
i) #To Read,display the image
```
import cv2
pic=cv2.imread("bird.jpg",1)
cv2.imshow("212221230098",pic)
cv2.waitKey(0)
cv2.destroyAllWindows() 
```
ii) #To write the image
```
import cv2
pic=cv2.imread("bird.jpg",1)
cv2.imshow("212221230098",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
iii) #Find the shape of the Image
```
import cv2
pic = cv2.imread('bird.jpg',1)
print(pic.shape)
```
iv) #To access rows and columns

```
import cv2
import random
pic=cv2.imread("bird.jpg",1)
for i in range(100):
    for j in range(pic.shape[1]):
        pic[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221230098",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) #To cut and paste portion of image
```
import cv2
pic=cv2.imread("bird.jpg",1)
crop=pic[300:400,300:400]
pic[50:150,50:150]=crop
cv2.imshow("212221230098",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image
![OUTPUT](SCR1.png)


### ii)Write the image
![OUTPUT](SCR2.png)

### iii)Shape of the Image
![OUTPUT](SCR3.png)


### iv)Access rows and columns
![OUTPUT](SCR4.png)

### v)Cut and paste portion of image
![OUTPUT](SCR5.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


