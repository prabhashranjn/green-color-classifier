# green-color-classifier
Classify green color from satellite image
Then, import the modules as well. Read the image and convert the BGR image to HSV(Hue, Saturation, Value) image using the cvtColor() function in the OpenCV module
Now, choose the color which you want to detect and get the lower and higher HSV values using the HSV color map shown below. In OpenCV, Hue has values from 0 to 180,
Saturation, and Value from 0 to 255. Thus, OpenCV use HSV values ranges between (0–180, 0–255, 0–255).
H is taken according to the x-axis, S is taken according to the y-axis, and V is always taken in the range between (20–255).
Using the HSV values, we need to find the mask using the inRange() function in the OpenCV module and assign it to the variable(mask)
bitwise_and() function we can get the detected color image that we chose by passing the BGR image as the first and second argument and
the third argument will be the mask and assign it to a variable(detected_img)
The detected_img will be the final output of the program and display using imshow() function in the OpenCV module.
and the following code will be in detecting the red and green colors only
