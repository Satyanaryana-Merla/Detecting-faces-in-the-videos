# Detecting-faces-in-the-videos
This Python script utilizes the OpenCV library to perform real-time face detection and create an output video with rectangles drawn around detected faces.
Here's a description of what each part of the code does:1. **
Importing OpenCV**: The script starts by importing the OpenCV library, which is commonly used for computer vision tasks.2. **
Loading Pre-trained Face Detection Classifier**: It loads a pre-trained face detection classifier using the Haar Cascade classifier.
This classifier is specifically trained to recognize frontal faces in images.3. **
Getting Video Frame Dimensions**: The script retrieves the width and height of the video frames to configure the output video correctly.5. **
Defining Video Codec and Creating VideoWriter**: It defines the codec (XVID) and creates a VideoWriter object named 'out' to save the processed frames as an output video named 'output_video.avi' with a frame rate of 20 frames per second.6. **
Initializing Face Count**: The variable 'total_faces' is initialized to count the number of detected faces.7. **
Processing Frames in a Loop**: The script enters a loop to process each frame of the video.8. **
Reading Video Frame**: It reads a frame from the video using the video capture object.9.
**Converting Frame to Grayscale**: The frame is converted to grayscale, which is often used for face detection to simplify processing.10. **
Detecting Faces**: The Haar Cascade classifier is applied to detect faces in the grayscale frame.
Detected faces are stored as rectangles in the 'faces' variable.11. **
Drawing Rectangles Around Detected Faces**: For each detected face, the script draws a green rectangle around it using OpenCV's drawing functions.12. **
Writing Frame to Output Video**: The frame, with rectangles drawn around the detected faces, is written to the output video.13. **
Displaying the Processed Frame**: The processed frame is displayed in a window with the title 'Video'.14. **
Breaking the Loop**: The loop continues until the 'q' key is pressed.
When 'q' is pressed, the loop breaks, and the script proceeds to release video objects and close OpenCV windows.15. **
Releasing Resources**: The video capture object and VideoWriter object are released to free up system resources.16. **
Closing OpenCV Windows**: Any remaining OpenCV windows are closed.
In summary, this script reads a video file, applies face detection to each frame, draws rectangles around detected faces, and saves the processed frames as a new video.
It also displays the real-time video with face detection, allowing the user to exit the process by pressing the 'q' key.
The final output is an AVI video file ('output_video.avi') with detected faces highlighted by green rectangles.
