# Reconstruction-of-3D-points
### Structure From Motion (SFM)

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

#### Output:
![image-3D-Reconstruction](https://user-images.githubusercontent.com/43301609/84455800-1f6fd400-ac13-11ea-9c23-13243b3a59a3.png) 
![image](https://user-images.githubusercontent.com/43301609/84455868-53e39000-ac13-11ea-9ca5-f60012a546e7.png)




