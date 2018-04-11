# **Finding Lane Lines on the Road** 

## **Overview**
-------------------------------------------------------------------------------------------------

When people drive, they use thier eyes to decide where to go.  The lines on the road that show
them where the lanes are act as thier constant reference for where to steer the vehicle. Naturally, 
one of the first things everyone would like to do in developing a self-driving car is to automatically 
detect lane lines using an algorithm.

This project will help to detect lane lines in images and videos that were taken from a camera at 
the center of a vehicle using Python and OpenCV. OpenCV means "Open-Source Computer Vision", 
which is a package that has many useful tools for analyzing images.  

## Getting started with the project
1. Step1
    Install python 3
1. Step 2
    Install Docker
1. Step 3
   run  ```docker pull udacity/carnd-term1-starter-kit``` 
   from [Starter-Kit] (https://github.com/udacity/CarND-Term1-Starter-Kit/blob/master/README.md)
   run ```docker run -it --rm -p 8888:8888 -v ${pwd}:/src udacity/carnd-term1-starter-kit```  
   in a repository with updated P1.inynb
1. Step 4
    Open P1.inynb in a Jupyter Notebook
1. Step 5
    Run all cells
    
##  Pipeline description 

My pipeline consisted of 5 steps:
 1. Step 1
     Convert the images to grayscale
2. Step 2
    Apply a Gaussian blur to the images
3. Step 3
    Use a [Canny transformation](https://en.wikipedia.org/wiki/Canny_edge_detector) to find edges on the images
4. Step 4
    Use a [Hough transformation](https://en.wikipedia.org/wiki/Hough_transform) to find the lines on the images
5. Step 5
    Merge the output of houghAction with the original image to show the lines on it.
