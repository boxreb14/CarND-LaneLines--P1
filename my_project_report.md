# **Finding Lane Lines on the Road** 

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps as mentioned in cell 7 of P1 notebook. First, I converted the images to grayscale, then I used the gaussian blur for smoothness then used the canny edge detection and after that I calculated the region of interest and calculated the hough lines using the given function and plotted them.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by taking all the points on left lane and right lane and applying a polyfit function to get a 1st order polynomial to find a line.

The output lines are included in test_images folder as output.



### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when lines will curve, shadows are present on the road and lane lines are of different color other than white.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to use color spaces so that lane lines of other color can also be identified better.
