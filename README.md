# CheckerBoardDetect
This python file computes the projection from a planar target to a real-world image in real-time.
by using the web-cam to capture images of a checkerboard which will track using OpenCV and then overlay another image on top of the image 
which is aligned with the checkerboard.
In effect plane-to-plane calibration to perform planar based augmented reality (AR).

Step 1: Planar Homographies
 Calibrate the real camera . 
 (i) compute the distortion (and intrinsic) parameters for your camera.
 (ii) undistort images from your camera such that the lines of the input checkerboard are straightened. 
 
Step 2: 
 Take an image of the checkerboard and undistort it. Now using the facilities provided by the OpenCV calib3d library generate a set of correspondences between the checkerboard and the undistorted image.
Using these correspondences compute the 3x3 homography (see notes on planar camera model) that maps points on the checkerboard to points on in the image. 

Step 3 : 
Using the warpprespective function and an image of choice, project the image such that it appears to lie in the plane of the checkerboard.

Note:
The image that needs to be overlapped needs to be saved with the name AR.jpg


Deepthi here!!!
