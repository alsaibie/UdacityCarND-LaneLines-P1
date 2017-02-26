#**Finding Lane Lines on the Road** 

##This is the writeup for the first project of the Self Driving Nanodegree Term1 Course: Computer Vision and Deep Learning

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"
[image2]: ./test_images/solidWhiteCurve.jpg "Solid White Curve"
[image3]: ./test_images/solidWhiteRight.jpg "Solid White Right"
[image4]: ./test_images/solidYellowCurve.jpg "Solid Yellow Curve"
[image5]: ./test_images/solidYellowCurve2.jpg "Solid Yellow Curve2"
[image6]: ./test_images/solidYellowLeft.jpg "solidYellowLeft"
[image7]: ./test_images/whiteCarLaneSwitch.jpg "whiteCarLaneSwitch"
[image8]: ./test_images/out/solidWhiteCurve.jpg "Solid White Curve _ Out"
[image9]: ./test_images/out/solidWhiteRight.jpg "Solid White Right _ Out"
[image10]: ./test_images/out/solidYellowCurve.jpg "Solid Yellow Curve _ Out"
[image11]: ./test_images/out/solidYellowCurve2.jpg "Solid Yellow Curve2 _ Out"
[image12]: ./test_images/out/solidYellowLeft.jpg "solidYellowLeft _ Out"
[image13]: ./test_images/out/whiteCarLaneSwitch.jpg "whiteCarLaneSwitch _ Out"

---

### Reflection

###1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consists of 7 steps. First I import the image and convert it to grayscale. Then I apply a gaussian smoothing filter. Then detect edges using a canny edge detector. I then create a mask for the area of interest where the highway lines are likely to reside. I perform a hough transform to detect the lines within the masked area and then output (draw) the lines on the original image. 

The pipeline is tested on the given 6 test images. The test images are shown alongside the images with the lines annotated. 
<img src="./test_images/solidWhiteCurve.jpg" width="425"/> <img src="image2.png" width="425"/> 


| ![alt text][image2] | ![alt text][image8] |

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


###2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


###3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...