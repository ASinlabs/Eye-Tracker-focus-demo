<h1>Eye Tracker Application</h1>
<br />
The Eye Tracker Application is a project that tracks eye movement using a camera and changes the background of the application to match the color of the object you are looking at. The application displays four color boxes on the screen, and the color of the background changes to match the color of the box you are currently looking at.
<br />
<br />

<h2>Installation </h2>
<br />
<b>Clone the repository:</b> git clone https://github.com/xomacs/Eye-Tracker-focus-demo
<br />
<b>Install the required packages:</b> npm install
<br /><br />

<h2>Usage</h2>
Look at one of the four color boxes displayed on the screen.
The background of the application will change to match the color of the box you are looking at.
How it works
<br /> <br />
The Eye Tracker Application uses the OpenCV library to track the user's eye movement. It first captures a frame from the camera and applies various image processing techniques to detect the user's eye. Once the eye is detected, the application determines the position of the eye within the frame.
<br />
Next, the application checks which of the four color boxes the user is looking at. It does this by comparing the position of the eye with the position of the color boxes on the screen. If the position of the eye is within a certain threshold of one of the color boxes, the background of the application is changed to match the color of that box.
<br />
The color matching is done using the colorthief library, which extracts the dominant color from an image. The application takes a screenshot of the color box and passes it to the colorthief library to determine the dominant color. This color is then used to set the background of the application.
<br /><br />

<h2>Future improvements</h2>
Improve eye detection accuracy
Implement a calibration process to improve accuracy for individual users
Add support for more than four color boxes
Add support for custom colors
