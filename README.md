## Aruco tutorial


Setup instructions:

1. Create a new conda environment w/ python 3.8 (optional but highly recommended)
```
conda create -n aruco_tutorial python=3.8
conda activate aruco_tutorial
```
2. Install requirements
```pip install -r requirements.txt```
3. Run `camera_calibration.py`. This will calibrate your camera with the images in the `images/` folder. Those images are obviously going to be wrong, since I took them using my webcam and not whatever camera you're using, so your pose estimation will probably be off unless take your own pictures.
4. Run `aruco_pose_estimation.py`. This will display the pose of the aruco marker if it is within the camera frame, and will also display the orientation axes.
