﻿# **Advanced-Lane-Finding**
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

<img src="videos/Screenshot.JPG" width="480" alt="Combined Image" />

# INTRODUCTION

Built an advanced lane-finding algorithm using distortion correction, image rectification, color transforms, and gradient thresholding. Identified lane curvature and vehicle displacement. Overcame environmental challenges such as shadows and pavement changes

In this project, I have used computer vision techniques to identify lane boundaries and compute the estimate the radius of curvature given a frame of video of the road.  

To achieve this, the following steps are taken:
- Computed the camera calibration matrix and distortion coefficients of the camera lens used given a set of chessboard images taken by the same camera
- Used the aforementioned matrix and coefficient to correct the distortions given by the raw output from the camera
- Use color transforms, and sobel algorithm to create a thresholded binary image that has been filtered out of unnecessary information on the image 
- Apply perspective transform to see a “birds-eye view” of the image as if looking from the sky 
- Apply masking to get the region of interest, detect lane pixels, 
- Determine the best fit curve for each lane the curvature of the lanes
- Project the lane boundaries back onto the undistorted image of the original view 
- Output a visual display of the lane boundaries and other related information 

