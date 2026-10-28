# Image Capture and Video Processing Using OpenCV

---

## Aim

To write a Python program using OpenCV to capture an image from the webcam and perform the following operations:

1. Write the frame as a JPG file  
2. Display the video  
3. Display the video by resizing the window  
4. Rotate and display the video  

---

## 🛠️ Software Used

- Anaconda – Python 3.7  
- Jupyter Notebook / VS Code  
- OpenCV (`cv2`)  

---

## ⚙️ Algorithm

### Step 1:
Import the required libraries and initialize the webcam using `cv2.VideoCapture()`.

### Step 2:
Capture frames continuously from the webcam.

### Step 3:
Save a frame as a JPG image using `cv2.imwrite()`.

### Step 4:
Display the live video stream using `cv2.imshow()`.

### Step 5:
Resize the frame and rotate it using OpenCV functions, then display the processed frames.

---

## 💻 Program
```
import cv2

img = cv2.imread('webcam.jpg')

cv2.imshow('Webcam Image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
```
import cv2
from google.colab.patches import cv2_imshow

img = cv2.imread('webcam.jpg')

cv2_imshow(img)
```
```
import cv2
from google.colab.patches import cv2_imshow

img = cv2.imread('webcam.jpg')

resized_img = cv2.resize(img, (640, 480))

cv2_imshow(resized_img)
```
```
import cv2
from google.colab.patches import cv2_imshow

img = cv2.imread('webcam.jpg')

rotated_img = cv2.rotate(img, cv2.ROTATE_90_CLOCKWISE)

cv2_imshow(rotated_img)
```

### Developed By:
**Name:** Janesha S

### Register No:
212225240056 

---

## Output

### i) Write the frame as JPG image
Captured image is saved as `webcam.jpg`

### ii) Display the image
Live webcam video is displayed

<img width="395" height="209" alt="image" src="https://github.com/user-attachments/assets/7dd6c203-77cc-4304-b7e7-2117178d1778" />

### iii) Display the image by resizing the window
Video is shown in resized resolution (640 × 480)

<img width="589" height="447" alt="image" src="https://github.com/user-attachments/assets/7083f8e6-6529-40ed-bbdd-6548e50d5fbf" />

### iv) Rotate and display the image
Video is displayed after rotation (90° clockwise)

<img width="208" height="396" alt="image" src="https://github.com/user-attachments/assets/47aeca1f-29dd-4dd5-ac1a-04009b21e6f3" />

---

## Result

Thus, the image is successfully captured from the webcam and various video processing operations such as saving, displaying, resizing, and rotating are performed using OpenCV.
