
<!-- Project is Under Devlopment -->

#Fall Detection using YOLO and Machine Learning

This project is a fall detection system that uses the You Only Look Once (YOLO) object detection algorithm and machine learning techniques to detect whether a person has fallen or not.

##Requirements
The following libraries are required to run this project:
OpenCV
NumPy
scikit-learn
Keras
TensorFlow
You can install these libraries using pip:

## Command to install required libraries
pip install opencv-python numpy scikit-learn keras tensorflow

##Dataset
The dataset used to train the machine learning model consists of videos of people falling and performing daily activities. The videos were collected from various sources, such as YouTube, and manually annotated to label each frame as either a fall or a non-fall event.

##YOLO Object Detection
The YOLO algorithm is used to detect people in each frame of the video. The YOLOv3 implementation from the Darknet project is used, which can be found at https://github.com/pjreddie/darknet.

##Machine Learning
After detecting people in each frame of the video, features are extracted from each person using a pre-trained convolutional neural network (CNN). The features are then fed into a support vector machine (SVM) classifier to determine if the person has fallen or not.

##Usage
To use this fall detection system, run the following command:

python detect_fall.py --video <path-to-video>
This will detect falls in the specified video and output the results to the console.

##References

Redmon, Joseph, and Ali Farhadi. "YOLOv3: An incremental improvement." arXiv preprint arXiv:1804.02767 (2018).
Chollet, François. "Deep learning with Python." Manning Publications Co. (2018).
https://github.com/pjreddie/darknet
