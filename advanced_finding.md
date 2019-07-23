# Advanced Lane Finding

## Camera Calibration

we use chessboards to calibrate our camera. Chessboards are great for calibration because their general high contrast pattern, a
makes it easy to detect patterns. And since we know what an undistorted chessboard looks like. So using the chessboard images taken
from the camera and our known undistorted chessboard we can measure the distortion and use that to correct the images. We use a transform from 
cv2 to undistort the images.
we first read in the calibration images of the chessboard. Using the real coordinates of a  chessboard and store them in objpoints. We use a opencv function
to find the corners in the disorted images and store them all in imgpoints. We then use an in built function in opencv to find the camera coefficient matrices. 
These will then be used to undistort an image with another in built opencv function
![](camera_calibration.png)

And this is an example of using the calibration coefficients to a test image
![](undistorted_img.png)
## Pipeline (test images)
### Color transforms

## Pipeline (video)

## Discussion