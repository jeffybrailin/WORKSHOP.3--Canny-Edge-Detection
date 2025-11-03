# WORKSHOP.3--Canny-Edge-Detection

## Name: Jeffy Brailin T
## Reg.No: 212223040076

## Code:

```
import cv2
import matplotlib.pyplot as plt
img = cv2.imread('jeffyimg.png.jpg',cv2.IMREAD_GRAYSCALE)
blurred =cv2.GaussianBlur(img, (5,5),0)
edges = cv2.Canny(blurred, 50, 150)
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```

## Output:

<img width="887" height="376" alt="image" src="https://github.com/user-attachments/assets/c6eee5dd-368d-4289-a960-3de562f35138" />
