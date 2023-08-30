# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
<br>
Import opencv.

### Step2:
<br>
Read the original Image.

### Step3:
<br>
Store the required conversion of the image in a variable


### Step4:
<br>
Show the image stored in the given variable.

### Step5:
<br>
Destroy all the windows and end the program

## Program:
```python
# Developed By: Jeswanth S
# Register Number: 212221230042
```
# i) Convert BGR and RGB to HSV and GRAY
```
# BGR TO HSV
import cv2
image =cv2.imread('black.jpg')
cv2.imshow('original',image)
b_h=cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR_HSV',b_h)
cv2.waitKey(0)
cv2.destroyAllWindows

# BGR TO GRAY
import cv2
image =cv2.imread('black.jpg')
cv2.imshow('original',image)
b_g=cv2.cvtColor(image,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR_GRAY',b_g)
cv2.waitKey(0)
cv2.destroyAllWindows

# RGB TO HSV
import cv2
image =cv2.imread('black.jpg')
cv2.imshow('original',image)
r_h=cv2.cvtColor(image,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB_HSV',r_h)
cv2.waitKey(0)
cv2.destroyAllWindows

# RGB TO GRAY
import cv2
image =cv2.imread('black.jpg')
cv2.imshow('original',image)
r_g=cv2.cvtColor(image,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB_GRAY',r_g)
cv2.waitKey(0)
cv2.destroyAllWindows
```





# ii)Convert HSV to RGB and BGR
```
# HSV TO RGB
import cv2
ori=cv2.imread('black.jpg')
cv2.imshow('Original',ori)
h_r=cv2.cvtColor(ori,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV_RGB',h_r)
cv2.waitKey(0)
cv2.destroyAllWindows

# HSV TO BGR
import cv2
ori=cv2.imread('black.jpg')
cv2.imshow('Original',ori)
h_b=cv2.cvtColor(ori,cv2.COLOR_HSV2BGR)
cv2.imshow('HSV_BGR',h_b)
cv2.waitKey(0)
cv2.destroyAllWindows
```




# iii)Convert RGB and BGR to YCrCb
```# RGB TO YCrCb
import cv2
ori=cv2.imread('black.jpg')
YCrCb_image = cv2.cvtColor(ori, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB_YCRCB',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows

# RGB TO YCrCb
import cv2
ori=cv2.imread('black.jpg')
YCrCb_image = cv2.cvtColor(ori, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR_YCRCB',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows
```




# iv)Split and Merge RGB Image
```
import cv2
img = cv2.imread('black.jpg')
img1= cv2.resize(img, (270,190))
cv2
b,g,r = cv2.split(img1)
cv2.imshow("RED MODEL", r)
cv2.imshow("GREEN MODEL", g)
cv2.imshow("BLUE MODEL ", b)
merger = cv2.merge([b,g,r])
cv2.imshow("MERGED IMAGE", merger )
cv2.waitKey(0)
cv2.destroyAllWindows()
```


# v) Split and merge HSV Image
```
import cv2
img = cv2.imread('black.jpg')
img1= cv2.resize(img, (270,190))
hsv = cv2.cvtColor(img1 , cv2.COLOR_BGR2HSV)
cv2.imshow("INITIAL_HSV ", hsv)
h,s,v = cv2.split(hsv)
cv2.imshow("RED MODEL", h)
cv2.imshow("GREEN MODEL", s)
cv2.imshow("BLUE MODEL ", v)
merger = cv2.merge([h,s,v])
cv2.imshow("MERGED IMAGE", merger )
cv2.waitKey(0)
cv2.destroyAllWindows()





```
## Output:
### i) BGR and RGB to HSV and GRAY
<br>
<img width="643" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/5b96d0a0-8dd7-41f2-a520-82759bb3a6ce">
<img width="641" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/46f9ac3b-b672-4411-af8e-9476c6b05f44">



<img width="642" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/2f6ba8f2-b74a-4b67-a905-390ba90f2702">


<br>

### ii) HSV to RGB and BGR
<br>
<img width="625" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/72385458-f09e-41f8-a0d0-f83d4d357f45">
<img width="643" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/550abc99-892d-4f44-89f5-33f06fc1369a">



<br>

### iii) RGB and BGR to YCrCb
<br>
<img width="639" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/6a45442e-519a-46c3-8829-6c16cfb1bd00">

<img width="643" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/b0633a4c-a1eb-49c4-993e-2dd42921b280">

<br>

### iv) Split and merge RGB Image
<br>
<img width="354" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/9088f649-528c-43f4-b7f6-9a0428eb16bf">


<br>

### v) Split and merge HSV Image
<br>
<img width="392" alt="image" src="https://github.com/Jeswanth21001768/COLOR-CONVERSION/assets/94155480/a37259f2-ab9d-45e5-96bc-b10c729c691d">
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
