# Face-Recognition-Attendance-Management-System
Attendance Management System based on Face Recognition using Python  and OpenCv  

This project implements an attendance management system based on face recognition, designed to automate the process of taking attendance in classrooms or other environments where tracking attendance is necessary. The system leverages OpenCV and Tkinter for the graphical user interface (GUI) and uses the LBPH (Local Binary Pattern Histogram) algorithm for face recognition.

### Features
- Face Recognition for Attendance: Capture and recognize student faces to mark attendance automatically.
- Manual Attendance: Option to manually fill in the attendance if automatic recognition fails.
- User Interface: Intuitive UI built with Tkinter for seamless interaction.
- Model Training: Train the face recognition model using images of registered students.
- Data Handling: Store and manage student details, including name and enrollment number, in CSV files.


### Requirements
- Opencv( `pip install opencv-python` )
- Tkinter( Available in python )
- PIL ( `pip install Pillow` )
- Pandas( `pip install pandas` )

### What steps you have to follow??
- Download my Repository 
- Create a `TrainingImage` folder in a project.
- Open a `AMS_Run.py` and change the all paths with your system path
- Run `AMS_Run.py`.

### Project Structure

- After run you need to give your face data to system so enter your ID and name in box than click on `Take Images` button.
- It will collect 70 images of your faces, it save a images in `TrainingImage` folder
- After that we need to train a model(for train a model click on `Train Image` button.
- It will take 5-10 minutes for training(for 10 person data).
- After training click on `Automatic Attendance` ,it can fill attendance by your face using our trained model (model will save in `TrainingImageLabel` )
- it will create `.csv` file of attendance according to time & subject.
- You can store data in database (install wampserver),change the DB name according to your in `AMS_Run.py`.
- `Manually Fill Attendance` Button in UI is for fill a manually attendance (without facce recognition),it's also create a `.csv` and store in a database.

### Screenshots

### Basic UI
<img src="https://github.com/atul21mangla/Face-Recognition-Attendance_system/blob/e346794f91c9eff2d675ede234d39db581b3e7a1/images/Screenshot%202025-01-11%20221747.png">

### When it Recognises me
<img src="https://github.com/atul21mangla/Face-Recognition-Attendance_system/blob/e346794f91c9eff2d675ede234d39db581b3e7a1/images/Screenshot%202025-01-11%20221811.png">

### While filling automatic attendance
<img src="https://github.com/atul21mangla/Face-Recognition-Attendance_system/blob/e346794f91c9eff2d675ede234d39db581b3e7a1/images/Screenshot%202025-01-11%20222511.png">

<img src="https://github.com/atul21mangla/Face-Recognition-Attendance_system/blob/e346794f91c9eff2d675ede234d39db581b3e7a1/images/Screenshot%202025-01-11%20222754.png">


### Troubleshooting
- Face Detection Not Working: Ensure the camera is correctly set up and the students are properly framed for face recognition.
- No Images Captured: If images are not being captured, check if the TrainingImage/ folder is correctly configured and accessible.
- Model Training Error: Ensure the TrainingImageLabel/ folder exists and has write permissions for saving the trained model.


### Future Improvements
- Implementing live video-based attendance recording for real-time recognition.
- Enhancing the recognition accuracy by integrating advanced machine learning models.
- Adding multi-language support for broader accessibility.
- Developing mobile app integration for remote attendance tracking.
