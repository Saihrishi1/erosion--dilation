# Implementation-of-Erosion-and-Dilation
# NAME SAI HRISHI M
# REF NO 212224240140
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
import the neccesary packages



### Step2:
create the text using cv2.put Text


### Step3:
create the structuting element


### Step4:
Erodde the image


### Step5:
Dilate the image


 
## Program:

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```


# Create the Text using cv2.putText
```
# Create a blank image
image = np.zeros((500, 500, 3), dtype=np.uint8)
```


# Create the structuring element
```
# Display the input image
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB for displaying
plt.title("Input Image with Text")
plt.axis('off')
```


# Erode the image
```
# Create a simple square kernel (3x3)
kernel = np.ones((3, 3), np.uint8)
# Apply erosion (shrinking effect)
eroded_image = cv2.erode(image, kernel, iterations=1)
# Display the eroded image
plt.imshow(cv2.cvtColor(eroded_image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB
plt.title("Eroded Image")
plt.axis('off')
```



# Dilate the image
```
# Apply dilation (expanding effect)
dilated_image = cv2.dilate(image, kernel, iterations=1)
# Display the dilated image
plt.imshow(cv2.cvtColor(dilated_image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB
plt.title("Dilated Image")
plt.axis('off')

```





## Output:

### Display the input Image
<img width="433" height="462" alt="image" src="https://github.com/user-attachments/assets/738b9d58-6154-4111-9efa-57e218b9a10e" />


### Display the Eroded Image
<img width="438" height="463" alt="image" src="https://github.com/user-attachments/assets/14ebaf01-b552-4ebc-9bdb-d44417496cfd" />


### Display the Dilated Image
<img width="436" height="468" alt="image" src="https://github.com/user-attachments/assets/78d4d30c-3222-4e28-9387-fdb5c7a22a66" />


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
