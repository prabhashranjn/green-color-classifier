import cv2
import numpy as np
bgr_img = cv2.imread('1638597199940.png')
hsv_img = cv2.cvtColor(bgr_img , cv2.COLOR_BGR2HSV)


lower_hsv = np.array([86, 31, 4])
higher_hsv = np.array([220, 88, 50])
mask = cv2.inRange(hsv_img, lower_hsv, higher_hsv)

detected_img = cv2.bitwise_and(bgr_img,bgr_img,mask=mask)

cv2.imshow('image',detected_img)
cv2.waitKey(0)
