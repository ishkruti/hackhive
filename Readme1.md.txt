An End-to-End Real-Time Face Identification and Attendance System using Convolutional Neural Networks

This repository contains the official implementation of the paper titled:

## [An End-to-End Real-Time Face Identification and Attendance System using Convolutional Neural Networks](https://ieeexplore.ieee.org/document/9029001)

This system offers an end-to-end face identification and attendance solution using Convolutional Neural Networks (CNN). It processes CCTV footage or a video of the class to mark the attendance of the entire class simultaneously. The system demonstrates robustness against common challenges such as occlusion (partially visible/covered faces), orientation, alignment, and luminescence of the classroom.

## Libraries
1. Tensorflow 1.14
2. Numpy
3. OpenCV
4. MTCNN
5. Sklearn
6. xlsxwriter, xlrd
7. scipy
8. pickle

## How to Use

### Installation
1. Install the required libraries (Conda environment preferred).
2. Download the pre-trained model from [here](https://drive.google.com/open?id=1EXPBSXwTaqrSC0OhUdXNmKSh9qJUQ55-) and copy it to the main directory.
3. Ensure the below directory structure is maintained (manually create folders named "attendance" and "output" in the main directory as shown in the "Main" directory structure).
4. To verify installation, run 'user_interface.py'.

### Create Dataset
1. Run 'user_interface.py'.
2. Click on the 'Create' button.
3. Select 'webcam' if you wish to create a live dataset (leave all other fields empty).
4. Click 'Continue' to start streaming webcam feed.
5. Press 's' to save face images (take approximately 80-100 images).
6. Press 'q' to exit.
7. Repeat for other datasets.

### Training
1. Run 'user_interface.py'.
2. Click on the 'Train' button.
3. Training duration may vary (depending on system configuration).
4. Once training is completed, a 'classifier.pkl' file will be generated.

### Run
1. Run 'user_interface.py'.
2. Click on the 'Run' button.
3. Select 'Webcam' from the list and leave all fields blank.
4. Click 'Mark Attendance'.
5. Attendance sheet will be generated automatically with the current date/time.