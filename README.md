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

4. Existing Methods:
  4.1 2-D
	- brightness
	- tracking features
	- annotation
  4.2 3-D
	- require manual initialization 
	- cannot handle large pose variations
	- not real time
	- computationally expensive
	- occlusions (nose tip required for [4])
  4.3 Breitenstein et al. [4]
	- [reference](http://dash.harvard.edu/bitstream/handle/1/4100250/Breitenstein_Real-time.pdf?sequence=2)
 


# Highlight

---------------------------
1. [Video](https://www.youtube.com/watch?v=sxUkGGGtRBU&spfreload=10)

# Discussions

---------------------------

1. Random regression forests
	- subsample data set, also features? i.e. for a feature set [x1,…,xn] train a decision tree with only [x2,x3]?
2. Add a smoothness constraint in the pose determination? 
since the method is real time, assuming the head is detected in each consecutive frame, the pose should vary smoothly i.e. have a smooth transition between frames. If the video is observed, around the 1:05 mark, the normal vectors jumps. This is because the computation is for each frame, independently of the previous. 

 # Questions

---------------------------

1. Why 2.5D output of the range scanner? (pg. 618) probably Cansen
2. What happens with multiple faces/objects in the field of view? (no head detection algorithm implemented)- multiple hypotheses possible? (they assume head has been detected, so perhaps not addressed or not aimed to be addressed in this paper/implementation)


