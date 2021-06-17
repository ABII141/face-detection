# face-detection
Simple Face Detection

1.install and import libraries
The first thing you’ll need to do is install the OpenCV library.
Although not required for face detection, we’re going to use Matplotlib to give us more control over the images we display during our face recognition demo.
To make sure you have Matplotlib installed, run the following command on your terminal:

2.import the required image
Before detecting a face within an image in OpenCV, you need to import the image.
The imread() method from the OpenCV module can be used to import an image.
To plot an image, you can use the imshow() method .
You can use whatever image you want, as long as it has a human face.

3.detecting face
Now that we’ve read our image, let’s try to detect the face from the image you imported. To demonstrate face detection, we are going to plot a rectangle around the detected face. OpenCV actually contains several objects that can be used to detect  face , eyes and smile. We’re going to focus on face detection only.
use this function - get_face() 
Inside the method, you first copy the image object into a local variable. then, you call the detectMultiScale() method using the fd object you created in the last script. The fd object (face detector) returns x and y coordinates and the widths and heights of all the faces in an image. The rectangle() method can then be used to plot rectangles around all the detected faces. After that, the final image, with the drawn rectangles, is returned to the calling function. Here’s the full `get_face() method'
Once you have the method defined, you simply need to call the get_face() method with the OpenCV image object you have imported.
The image returned by the get_face() method can be plotted via the imshow() .
a rectangle was successfully drawn around the detected face and the output shows that the face has been detected successfully.
