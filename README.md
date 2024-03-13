# Contour_-_Binary_image_with_cv2
![image](https://github.com/Shawon5030/Contour_and_Binary_image_with_cv2/assets/149573785/ddb237e5-5013-49df-8621-7c12c352501a)

# 1. Loading and Preprocessing Image:
The code loads an image using OpenCV (cv2.imread) from the specified file path. <br/>
<b/> Converts the loaded image to grayscale using cv2.cvtColor(). <br/>

# 2. Image Blurring:
Applies Gaussian blur to the grayscale image using cv2.GaussianBlur(). <br/>
This step helps to reduce noise and smoothen the image, making it easier for subsequent processing steps. <br/>

# 3. Thresholding:
Applies Otsu's thresholding method using cv2.threshold() to obtain a binary image. <br/>
Otsu's method automatically calculates an optimal threshold value based on the image histogram. <br/>
This step converts the grayscale image into a binary image where pixel values are either 0 or 255. <br/>

# 4. Finding Contours:
Uses cv2.findContours() to detect contours in the binary image. <br/>
Contours are the outlines of objects present in the image. <br/>
The function returns a list of contours and a hierarchy representing the relationship between contours. <br/>

# 5. Drawing Contours:
Copies the original image (image.copy()) to draw contours on a separate image. <br/>
Draws contours using cv2.drawContours() on the copied image. <br/>
The contours are drawn with a green color (0, 255, 0) and a thickness of 3 pixels. <br/>

# 6. Displaying Images:
Utilizes Matplotlib to display multiple images in a grid layout (subplots). <br/>
Displays the original image, grayscale image, binary image, and contour image in separate subplots. <br/>
The titles of subplots describe the type of image being displayed. <br/>
Axis ticks are turned off for better visualization. <br/>

# 7. Additional Points:
Grayscale conversion and blurring are common preprocessing steps before applying thresholding or contour detection algorithms. <br/>
Otsu's method is useful for automatic thresholding, particularly in cases where the distribution of pixel intensities is bimodal. <br/>
Contours can be used for various purposes such as object detection, shape analysis, and image segmentation. <br/>
