# READ-AND-WRITE-AN-IMAGE-USING-PYTHON
## AIM
To write a python program using OpenCV to do the following image manipulations.

i) Read, display, and write an image.

ii) Access the rows and columns in an image.

iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
Jupyter lab
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
# Developed By: Dineshkumar S
# Register Number: 212220230012
```
### To Read,display the image
```
import cv2
pic = cv2.imread("hot air baloon.jpg")
cv2.imshow('Scenery',pic)
cv2.waitKey(0)
```


### To write the image
```
import cv2
pic = cv2.imread("hot air baloon.jpg")
pic2 = cv2.imwrite('Scenery.jpg',pic)
cv2.imshow('Scenery',pic)
cv2.waitKey(0)
```



### Find the shape of the Image
```
import cv2
pic = cv2.imread('hot air baloon.jpg')
print(pic.shape)
```


### To access rows and columns
```
import cv2
import random
pic = cv2.imread("hot air baloon.jpg")
for i in range(100):
    for j in range(pic.shape[1]):
        pic[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("Scenery",pic)
cv2.waitKey(0)
```



### To cut and paste portion of image
```
import cv2
pic = cv2.imread('hot air baloon.jpg')
tag = pic[300:400,300:400]
pic[50:150,50:150] = tag
cv2.imshow('Scenery',pic)
cv2.waitKey(0)
```









## Output:

### i) Read and display the image
![Screenshot (13)](https://user-images.githubusercontent.com/75234807/163681012-d992cc71-2a74-4bc3-961f-ff2b33c363e4.png)

### ii)Write the image
![Screenshot (14)](https://user-images.githubusercontent.com/75234807/163681028-7b431a82-412e-491f-ac18-ef578090a65a.png)

### iii)Shape of the Image
![Screenshot (15)](https://user-images.githubusercontent.com/75234807/163681062-69aa33b2-785d-4bf9-b72d-d43ba6251bd3.png)

### iv)Access rows and columns
![Screenshot (16)](https://user-images.githubusercontent.com/75234807/163681093-6687b993-3883-48c2-a3e6-7921c94de34a.png)

### v)Cut and paste portion of image
![Screenshot (17)](https://user-images.githubusercontent.com/75234807/163681104-60612cdb-8f5a-47ca-820b-96c2708145f8.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
