# Coin-Detection
USD Money detection program that can determine the type and measurement of the currency in front of it. <br>
<br>
## Main Topics Used:
● Camera Calibration  <br>
● Masking Image  <br>
● ARUCO Detection  <br>
● ORB Feature Detection  <br>
 <br>
## Basic Procedure:
1. Code performs camera calibration for distortion coefficients and k matrix
2. Take image input for measurement and finds Aruco Marker in image
3. Use Aruco Marker as reference for measurement (must know Marker’s length)
4. Perform masking to find contours within image and create bounding box for each notable figure
5. For each bounding box, find length and width of each box to find object’s dimension based on reference measurements
6. Create new image by cropping each bounding box
7. Use Orb Detection on crop image and compare it to list of inputted images
8. Image that best matches crop image is that object’s “Identity”
9. Write object’s identity on original image

## Results:
![](https://github.com/tk2558/Coin-Detection/blob/main/Results%20for%20image%20with%20many%20objects.gif))
