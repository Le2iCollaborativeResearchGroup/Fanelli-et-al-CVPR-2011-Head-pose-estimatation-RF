# Devesh 

---------------------------

Find the following information about this article:

    Title: Real Time Head Pose Estimation with Random Regression Forests
    Author: Fanelli, Gall, Van Gool
    Journal/Conference: CVPR
    Year: 2011

This CVPR paper is a short version of the following IJCV:
Fanelli, Dantone, Gall, Fossati and Van Gool, "Random forests for real time 3D face analysis", *International Journal in Computer Vision*

# Graphical Abstract

---------------------------

1. Problem: head pose estimation, meaning 6 parameters: head location (3) + orientation (3)
	- head location: 3 coordinates wrt reference frame
	- orientation: 3 rotation angles (roll, pitch, yaw)

2. Motivation:

- fast: real time
- reliable: over standard data sets and practice
- robust: occlusion, pose variations, expressions
- automatic: no manual initialization necessary (provided head is there, no detection scheme)
- computationally less expensive (compared to [4], no need for graphics hardware)

3. Application:

	- interactive software using head pose + movements (kinect games)
	- embedded on car (several projects on this already, refer Cansen)
	- identification
	- facial analysis

4. Existing Methods

	4.1 2-D
4.2 3-D

# Highlight

---------------------------

# Discussions

---------------------------

 # Questions

---------------------------

1. Why 2.5D output of the range scanner? (pg. 618) probably Cansen
2. What happens with multiple faces/objects in the field of view? (no head detection algorithm implemented)- multiple hypotheses possible? (they assume head has been detected, so perhaps not addressed or not aimed to be addressed in this paper/implementation)


