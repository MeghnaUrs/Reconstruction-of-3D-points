# Reconstruction-of-3D-points
### Structure From Motion (SFM)
SFM is an imaging technique used to reconstruct 3D points using 2D points from multiple viewpoints. 

#### SFM Pipeline Program Outline:
- Initiate SIFT detector
- Find the key points and descriptors with SIFT
- Apply FLANN for feature matching
- Store all the good matches as per Lowe's ratio test
- Find 2D points corresponding to good matches
- Store points retrieved from the good matches
- Find essential matrix and mask to remove outliers
- Recover rotation and translation matrices from the essential matrix
- Convert image coordinates to normalized coordinates
- Find Extrinsic matrix of second camera, first camera aligned with world co-ordinates
- Find projection matrix as a product of intrinsic and extrinsic matrix
- Remove outliers
- Find 4D homogeneous points and convert to 3D points

#### Outputs:
<br />
<br />
<p align="center">
  <img width="460" height="300" src="https://user-images.githubusercontent.com/43301609/84455800-1f6fd400-ac13-11ea-9c23-13243b3a59a3.png">
</p>
<p align="center">
  <img width="460" height="300" src="https://user-images.githubusercontent.com/43301609/84455868-53e39000-ac13-11ea-9ca5-f60012a546e7.png">
</p>

#### Requirements:
###### Windows development environment (Anaconda Navigator). You will need the following to run the scripts:
```
OpenCV
Numpy
Glob
MeshLab - To visualize the reconstructed points

SIFT is patented, you might need to choose (reinstall) appropriate opencv version
pip install opencv-contrib-python==3.4.2.16

```




