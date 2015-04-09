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

Problem: head pose estimation, meaning 6 parameters: head location (3) + orientation (3)
	head location: 3 coordinates wrt reference frame
	orientation: 3 rotation angles (roll, pitch, yaw)

Motivation:

- fast
- reliable
- robust
- automatic
- computationally less expensive (no need for graphics hardware)



# Highlight

---------------------------

# Discussions

---------------------------

 # Questions

---------------------------

1. Why 2.5D output of the range scanner? (pg. 618) probably Cansen
2. What happens with multiple faces/objects in the field of view? (no head detection algorithm implemented)- multiple hypotheses possible? (they assume head has been detected, so perhaps not addressed or not aimed to be addressed in this paper/implementation)


