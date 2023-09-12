# Face Detection using OpenCV by Linda Paz

This repository contains a Python script for real-time face detection using the OpenCV library. It captures video from the default camera (0) and applies a Haar Cascade classifier to detect faces in the frames.

## Dependencies

- OpenCV

## Usage

1. Make sure you have Python and OpenCV installed on your system.
2. Download the `haarcascade_frontalface_default.xml` file from the [OpenCV GitHub repository](https://github.com/opencv/opencv/tree/master/data/haarcascades).
3. Place the `haarcascade_frontalface_default.xml` file in the same directory as the Python script.
4. Run the script. It will open the default camera feed and draw rectangles around detected faces in real-time.

## How it Works

The script uses the `cv2.CascadeClassifier` to load the Haar Cascade classifier for face detection. It then opens the default camera using `cv2.VideoCapture(0)`.

In the main loop, it reads frames from the camera feed, converts them to grayscale, and applies the face detection using `face_cascade.detectMultiScale()`. Detected faces are then outlined with rectangles.

Press the 'Esc' key to exit the program.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify this code for your own purposes.

## Acknowledgments

Special thanks to the OpenCV community for providing the Haar Cascade classifier files.
