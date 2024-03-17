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


## Desktop Application

The desktop application serves as a tool for creating a student database using deep learning techniques. It is built using the Tkinter library in Python, providing a user-friendly interface for capturing student data through video. The application utilizes deep learning algorithms to process the captured video, extract facial features, and store the data securely.

### Features:
- *Data Capture*: Users can capture student data by recording their video through the application.
- *Deep Learning Integration*: The application leverages deep learning models to extract facial features from the captured video.
- *Data Storage*: Extracted facial features are stored securely in a database, ensuring the privacy and integrity of student information.
- *User-Friendly Interface*: The Tkinter-based interface makes it easy for users to navigate and interact with the application.

## Web Application

The web application serves as a client-facing interface, accessible through both desktop and mobile devices. It is designed to be used by teachers for attendance management and summary viewing. The web app integrates with the desktop application's database to provide real-time attendance tracking and analysis.

### Features:
- *Login System*: Teachers can log in to the web application using their credentials.
- *Class Selection*: After logging in, teachers can select the class they wish to manage attendance for.
- *Attendance Taking*: The application allows teachers to take attendance by capturing video through the device's camera. It uses facial recognition to match students with the database.
- *Attendance Summary*: Teachers can view attendance summaries for individual students and the entire class.
- *Data Export*: Attendance data can be exported and mailed to the teacher for record-keeping purposes.
- *Responsive Design*: The web application is designed to be responsive, ensuring optimal user experience across various devices and screen sizes.

Both applications work in tandem to provide a comprehensive solution for student attendance management, combining the power of deep learning for data extraction and web technologies for user interaction and accessibility.


# Automated Attendance System

This repository contains the source code for an Automated Attendance System developed using Convolutional Neural Networks (CNN) for real-time face identification. The system consists of two main applications: a desktop application and a web application.

## Desktop Application

### Libraries Used

1. *Tensorflow 1.14*: TensorFlow is an open-source machine learning framework developed by Google. It is used for deep learning tasks, such as facial recognition.

2. *Numpy*: NumPy is a fundamental package for scientific computing with Python. It provides support for numerical computations and data manipulation.

3. *OpenCV*: OpenCV (Open Source Computer Vision Library) is a popular computer vision library used for image processing tasks, including capturing video frames, facial detection, and image manipulation.

4. *MTCNN*: MTCNN (Multi-task Cascaded Convolutional Networks) is a deep learning model used for face detection and alignment, often used as a pre-processing step for face recognition tasks.

5. *Scikit-learn*: Scikit-learn is a machine learning library in Python that provides tools for data mining and data analysis, potentially used for facial recognition or data analysis tasks.

6. *XlsxWriter, xlrd*: XlsxWriter is used for writing data to Excel files, while xlrd is used for reading data from Excel files.

7. *Scipy*: Scipy is a scientific computing library used for advanced numerical computations.

8. *Pickle*: Pickle is used for serializing and deserializing Python objects, likely used for storing and retrieving deep learning models and student data.

## Web Application

### Libraries Used

1. *Flask*: Flask is a lightweight web framework for Python, used to create routes, handle requests, and render HTML templates.

2. *Multiprocessing*: Multiprocessing is used to run multiple tasks concurrently, such as capturing video and uploading images.

3. *CV2 (OpenCV)*: OpenCV is used for capturing video from the device's camera and processing video frames for facial recognition.

4. *Datetime*: Datetime is used for timestamping and organizing attendance data.

5. *MongoConnection*: This custom module facilitates connections to a MongoDB database for storing and retrieving attendance data.

6. *Base64*: Base64 is used for encoding images before storing them in the database.

7. *SMTPlib, Email*: SMTPlib and Email are used for sending attendance data to teachers via email.

These libraries are essential components of both the desktop and web applications, enabling functionalities such as facial recognition, data storage, email communication, and more.
