# Scrudium
Criminal Identification using AI through CCTV footage
A system to capture face, expression and
gesture of targeted persons (Criminals) through distributed CCTV System and
maintaining it in a database along with time and location stamp. The database
so compiled to be used to identify suspects from video clips of crime related
CCTV footages captured series of CCTV Systems located on routes and close to
scene of crime.

# Objectives

- Recognize criminal activities and mishappenings through captured live CCTV footage.
- Provide immediate information to the responsible authorities about such activities.
- Recognize the criminal associated with those activities through face recognition.
- Determine the emotion, age, and gender of the person associated with those activities.

## Merits of the Proposed System

- Stop criminal activities immediately and reduce the delay in alerting the authorities.
- Reduce the loss of property, money, and minimize fatality and crime rate.
- Capture the culprit within a short period.
- Provide the culprit’s details such as gender and age to the concerned authorities.
- Reduce the tedious job of continuous monitoring of live CCTV footage, including remote places with no frequent monitoring.

## Approach

- Use activity, face, and emotion recognition to predict activity and suspect details and alert authorities.
  
### Activity Recognition

- Train various CCTV captured video footage obtained from online sources and mark various events under respective attributes such as Abuse, Burglary, Assault, etc.

### Face Recognition

- Train the face recognition module using obtained face data of a person from criminal records.
- Recognize known faces on live video footage.
- For effective recognition, the person needs to be at a minimum distance of 5 meters in the live video footage.

### Emotion, Age, and Gender Recognition

- Capture emotion, age, and gender of a person in the CCTV footage.
- Determine emotion under predefined emotions such as happy, sad, angry, etc.
- Predict age and gender for further investigation if required.

## Scrudium

- Integrated system running all recognition modules in parallel.
- Named as Scrudium (Scrutiny + Medium) to monitor live CCTV footage 24/7 and send analyzed data to authorities through a shared medium.

### How Scrudium works?

- Take input from live CCTV camera stream and run all integrated recognition modules simultaneously.
- Identify each activity and associated person's face.
- Determine emotion, age, and gender.
- View and examine recognized attributes on the Scrudium platform.

### How are the authorities alerted?

- Store details of detected activities or suspects in the database.
- Acquire details from the database in real-time as per requirement.

## Firebase as Database

- Firebase provides a real-time database and backend as a service.
- Store all recognized activity and criminal details for real-time access.

## Criminal Activity Recognition

- Use ResNet50 alternative of Convolutional Neural Network model for recognizing criminal activities.
- Train the model using transfer learning on obtained weights.
- Generate fine-tuned classifier and serialized label binarizer for recognition.
![s1](https://github.com/kundamnikhil/Scrudium/assets/43941418/7230ee1e-7d8a-47e7-8057-7aa630eb1e60)

## Face Recognition Module Architecture

- Use Support Vector Machine for face recognition.
- Detect and localize faces in frames.
- Compute embeddings for faces in the dataset.
- Predict the class of recognized faces in the video or live stream.

## Emotion, Age, and Gender Recognition

- Use haarcascade frontal face emotion classifier and WideResNet CNN model for emotion, age, and gender recognition.
- Classify emotions projected by suspects.
- Predict age and gender of suspects in the stream.

## Scrudium Android Application

- Developed using Android Studio.
- Integrated with the database.
- Provides an interface containing details for each incident occurred.

![s2](https://github.com/kundamnikhil/Scrudium/assets/43941418/a621c91a-2b2b-4b55-9495-97cd688aadbf)


This structured approach ensures efficient detection, recognition, and alerting of criminal activities, enhancing security and safety measures.


![s4](https://github.com/kundamnikhil/Scrudium/assets/43941418/fd916b09-c726-40aa-80d0-a972677f1af4)
![s3](https://github.com/kundamnikhil/Scrudium/assets/43941418/023f27f6-61d2-4073-b206-f8e5698f3e8a)
![s5](https://github.com/kundamnikhil/Scrudium/assets/43941418/ec93732d-e27b-436f-9760-45df9e358ebb)
