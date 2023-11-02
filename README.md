![OpenCV LOGO](https://cdn.analyticsvidhya.com/wp-content/uploads/2021/07/88112cattura-1.jpg)

# Bienvenue au workshop OpenCV

Have you ever seen facial recognition systems in movies and wanted to recreate them ? Well, it's now possible quickly and easily with OpenCV !

In this worshop, you will learn how to use OpenCV to recognize faces and maybe more...
Remenber that in order to finish this workshop, you will need a webcam.
Try intalling dlib before the workshop.
**Don't sign up for this workshop if you don't have a webcam**

See [here](https://docs.opencv.org/4.x/d6/d00/tutorial_py_root.html) for the OpenCV / python documentation.

## Before starting

Before you start your workshop, make sure that you have installed OpenCV for python.

```shell
pip install opencv-python
```

## Step 1

Start by creating a `main.py` file at the root of your folder.
Import OpenCV using:
```python
import cv2
```

Find how to open your webcam and display it in a new OpenCV window.

## Step 2

Find how to change the settings of the window, like the FPS and size.
Try to find how to quit the window by pressing the `Esc` key.

## Step 3

Find how to take a screenshot from your webcam, when you press `Enter`, and save it as `<your_name>.jpg` in a `photos` folder.

## Step 4

Find how to draw a green rectangle on your window.

## Step 5

Install the face_recognition module and dlib with the commands:
```shell
pip install face_recognition
pip install dlib
```
Note that the dlib is quite long to install.

Load the face recognition model from OpenCV called `haarcascade_frontalface_default.xml` into a variable called `face_cascade`.
Download the file `shape_predictor_68_face_landmarks.dat` from this repository and put it a the root of your folder.

With dlib, create a variable called `detector`, to store the frontal face detector.

## Step 6

With the detector, find a way to identify all the faces on screen.
With what you did in the [step 4](#Step-4), you should be able to draw a green rectangle around all the faces on screen.

## Step 7

Load your photo from earlier with the function `face_recognition.load_image_file()` and encode-it with `face_recognition.face_encoding()`

Now compare the face(s) from the screen and the one from your photo.
Try to write a certain text over your head, and another if the face isn't recognized.

## To go further

Congratulation for finishing this workshop !

If you want to go further, you can learn how to recognize other body parts.

## Mini project

Try to clean your code by making it smart.
The goal here is to load every images from the `photos` folder, and check if they are on screen.
If so, you should be able to write the name of each person on screen based on their picture.
Feel free to experiment and don't forget to be creative !
