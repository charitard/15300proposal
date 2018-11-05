# Proposal: 3D Reconstruction from multiple viewpoint footage
 
## Description
There is an increasing need for geometric 3D models in the movie or games industry, mapping or taking street data and others. The objective of this research project is to identify the various approaches to generating sparse 3D reconstructions using the Structure from Motion (SfM) algorithms and the methods to generate dense 3D reconstructions using the Multi View Stereo (MVS) algorithms. This research project is falls under work done with Platform Pittsburgh under Professor Srinivasa G. Narasimhan.

## Project Goals
The objective of this project would be to try to implement Masatoshi Okutomi and Takeo Kanade paper: ”A Multiple-Baseline Stereo” which deals with depth determination using multiple cameras, and the multiple view video reconstruction algorithm in the CarFusion paper, developed this year in CMU. Our implementations will rely on a data from cameras taken from the Forbes and Fifth intersection. Stereo confidence measures give an indication about the certainty of the matching. The main aim of using confidence measures is to filter the erroneous disparity estimations at the end of the matching process. However, they can also be incorporated at the initial step of the matching process to obtain accurate estimations before the cost aggregation. Different stereo confidence measurements will be used and compared such as Zero Mean Normalized Cross Correlation (ZMNCC), Sum of Square differences measurement (SSD) and possibly others.
 * 75% goal - implement Okutomi and Kanade algorithm
 * 100% goal - implement CarFusion algorithm
 * 125% goal - speed up implementation or look for more efficient reconstruction methods

## Literature
 * Multiple View Geometry in Computer Vision by Richard Hartley, Andrew Zisserman
 * <https://www.ri.cmu.edu/publications/carfusion-combining-point-tracking-and-part-detection-for-dynamic-3d-reconstruction-of-vehicle/>
 * <https://www.cs.cmu.edu/~ph/869/papers/kanade-okutomi.pdf/>

## Resources
Not yet decided

## 1st Technical Milestone for 15-300
Complete 16-720 homework #4 on 3D reconstruction in MATLAB, do a surbey of existing code bases for computer vision 3D reconstruction

## Bi-weekly Milestonres for 15-400
February 1st: decide on what packages to use for feature detection and video synchronization part of the pipeline
 
February 15th: implement feature detection and point correspondence between images in video frames
 
March 1st: implement 3d reconstruction from multiple viewpoints using static image sets

March 22nd: compare success rates for static image reconstruction with different image feature detectors and confidence measures
 
April 5th: implement 3d reconstruction from multiple viewpoints using video footage - multiple images with extra time parameter, based off paper CarFusion: Combining Point Tracking and Part Detection for Dynamic 3D Reconstruction of Vehicle
 
April 19th: optimize implementation
 
May 3rd: optimize implementation
