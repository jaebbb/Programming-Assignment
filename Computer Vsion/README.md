## Task 0. Implement a function that convolves image with a given kernel. (20 pt)  
Hint: https://en.wikipedia.org/wiki/Kernel_(image_processing)  


## Task 1. Detect Edges from the given image (lane.png) using the convolution function you implemented in Task 0 (20 pt)  
![image](https://user-images.githubusercontent.com/52495256/83962621-c6820200-a8d9-11ea-93e0-b6f608891c5a.png)  
Hint: You can use any edge detectors such as Sobel, Laplacian or Canny edge detectors.  


## Task 2. Thresholding the edge images. (10 pt)  
![image](https://user-images.githubusercontent.com/52495256/83962634-eca7a200-a8d9-11ea-86ee-559b2a6e20de.png)  
  
## Task 3. Perform a RANSAC algorithm to detect lines which consti- tutes the lane on the Edge Image, and Draw the lines on the image. 
All the examples below are good results for this task.(50 pt)  
![image](https://user-images.githubusercontent.com/52495256/83962641-0517bc80-a8da-11ea-8cf7-f5cbb14a002d.png)  

Hint: https://en.wikipedia.org/wiki/Random_sample_consensus Hint: you can use cv2.line() to draw a line on the image.  
