# OPENING--AND-CLOSING
# NAME: NARENDHARAN M
# REG NO: 212223230134
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages




### Step2:
<br>Create the Text using cv2.putText



### Step3:
<br>Create the structuring element



### Step4:
<br>Use Opening operation



### Step5:
<br>Use Closing Operation


 
## Program:
```

import cv2
import numpy as np
import matplotlib.pyplot as plt
image = np.zeros((500, 500, 3), dtype=np.uint8)
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, 'Open and Close', (100, 250), font, 1, (255, 255, 255), 2, cv2.LINE_AA)
kernel = np.ones((3, 3), np.uint8)
plt.subplot(1, 3, 1)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.title("Input Image")
plt.axis('off')
plt.subplot(1, 3, 2)
plt.imshow(cv2.cvtColor(opened_image, cv2.COLOR_BGR2RGB))
plt.title("Opening Operation")
plt.axis('off')
plt.subplot(1, 3, 3)
plt.imshow(cv2.cvtColor(closed_image, cv2.COLOR_BGR2RGB))
plt.title("Closing Operation")
plt.axis('off')

```





## Output:

### Display the input Image
<img width="301" height="232" alt="image" src="https://github.com/user-attachments/assets/d3cae9f2-526f-4f03-9979-edfd5df5fd85" />


### Display the result of Opening
<img width="223" height="226" alt="image" src="https://github.com/user-attachments/assets/82fe129c-b9c2-4c1f-be1c-e597555511f5" />
>

### Display the result of Closing
<img width="238" height="247" alt="image" src="https://github.com/user-attachments/assets/a382f2c7-4fa7-48cf-bf84-d5b7ffa9cc2d" />


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
