# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import opencv.

### Step2:
Read the original Image.

### Step3:
Store the required conversion of the image in a variable.

### Step4:
Show the image stored in the given variable.

### Step5:
Destroy all the windows and end the program.

## Program:
```python
# Developed By:NIROSHA.S
# Register Number:212222230097
```
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('mn.jpeg')
cv2.imshow('Original Image',houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# ii)Convert HSV to RGB and BGR
```
import cv2
houseHSVImage = cv2.imread('mn.jpeg')
cv2.imshow('Original HSV Image',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('mn.jpeg')
cv2.imshow('Original HSV Image',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('mn.jpeg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
# v) Split and merge HSV Image
```
import cv2
image = cv2.imread('mn.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow

```
## Output:
### i) BGR and RGB to HSV and GRAY

![mn1](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/834d7ba0-9ae5-4c28-b563-4383a83fb17f)

![mn2](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/1175366b-e476-420b-8a71-1570069904ed)

![mn3](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/3b1dd6c6-9165-4edb-badb-41198b4ae0b0)

![mn4](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/de09eed1-f323-4ea1-9c7f-910d23bbc5d6)

### ii) HSV to RGB and BGR

![mn5](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/d892fd81-d3cd-4519-b318-0bbf3af4d85d)

![mn6](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/60930772-96d2-41d7-b120-20b35e318b80)

![mn7](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/62d3c42c-9321-4e8b-8f3f-746c0b070c47)

### iii) RGB and BGR to YCrCb

![mn8](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/a5c6c5b5-27f9-45c1-87a1-92c1b537e74d)

![mn9](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/83a7bad4-8f57-42a9-aff3-eb080c990589)

![mn10](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/57948076-95cd-41e4-8528-a0ad1c44d678)

### iv) Split and merge RGB Image

![mn11](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/52d3e764-65f0-4f75-8052-2289cba9cd1f)

![mn12](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/b38c0997-34e6-441b-a4c0-6268c694f436)

![mn13](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/cb7c28ce-84b5-4aa3-b9b5-b518e5ab3516)

![mn14](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/9f7ad491-2d8e-4f27-bb22-21a5d6707e13)

### v) Split and merge HSV Image

![mn15](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/1fba489c-4ba9-43f2-acd2-330a4444c653)

![mn16](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/3cf21528-ce47-4f12-9bc9-734057902b91)

![mn17](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/65f02b45-c09e-48d1-b45f-86692f8f2f5e)

![mn18](https://github.com/Niroshassithanathan/COLOR-CONVERSION/assets/121418437/b87eab95-a073-46f7-b66d-014a103558e6)

## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
