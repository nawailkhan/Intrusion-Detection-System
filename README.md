# Intrusion Detection System
# Introduction
Intruder detection systems are essential for ensuring the security of homes, offices, and other premises. Here, I will explore how to build an intruder detection system using OpenCV, a popular computer vision library, and email notifications. The system will use a webcam to capture video frames, analyze them for intruders, and send email notifications when an intruder is detected.

# Key Concepts
1. OpenCV: OpenCV (Open Source Computer Vision Library) is an open-source computer vision and machine learning software library. It provides various functions and algorithms to process images and videos.

2. Email Notifications: Email notifications are a common way to receive alerts or updates. In this system, we will use the Simple Mail Transfer Protocol (SMTP) to send email notifications when an intruder is detected.

3. Motion Detection: Motion detection is the process of detecting changes in the position of objects relative to their surroundings. In our system, we will use motion detection to identify potential intruders in the video frames.

4. Contours: Contours are the boundaries of objects in an image. In our system, we will use contours to identify and draw rectangles around potential intruders.

# Code Structure
The code provided consists of several functions and a main loop. Let's break down the code structure:

1. send_email(image_paths): This function sets up the email parameters, attaches images of the intruder, and sends the email using the SMTP protocol.

2. check_intruder(): This function checks if an intruder is present by analyzing the contours of the objects in the video frames.

3. click_event(event, x, y, flags, param): This function handles mouse events and allows the user to select a region of interest (ROI) for motion detection.

4. draw, frame1, rect: These global variables are used to store the state of the system, including the current frame, the ROI, and the drawing status.

5. cap: This variable represents the webcam capture object.

6. while cap.isOpened(): This is the main loop of the system. It captures video frames, performs motion detection, checks for intruders, and sends email notifications.

# Conclusion
I explored how to build an intruder detection system using OpenCV and email notifications featuring the key concepts such as motion detection, contours, and email notifications. By implementing this system, you can enhance the security of your premises and receive timely alerts when an intruder is detected.
