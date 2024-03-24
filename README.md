# person-reidentification
Person re-identification (re-ID) is a computer vision task that involves identifying individuals across different cameras or scenes. OpenCV (Open Source Computer Vision Library) is a popular library for computer vision tasks, including person re-identification



# Mini Project Report on
 

# PERSON RE-IDENTIFICATION IN VIDEOS
 

Submitted in partial fulfilment of the requirement for the award of the degree of

BACHELOR OF TECHNOLOGY

IN

COMPUTER SCIENCE & ENGINEERING


Submitted by:

Student Name :Anurag MandalUniversity Roll No. : 2021573









 


Department of Computer Science and Engineering 
Graphic Era (Deemed to be University) 
Dehradun, Uttarakhand 
December-2023 





 
	
CANDIDATE’S DECLARATION 


I hereby certify that the work which is being presented in the project report entitled “PERSON RE IDENTIFICATION IN VIDEOS” in partial fulfillment of the requirements for the award of the Degree of Bachelor of Technology in Computer Science and Engineeringof the Graphic Era (Deemed to be University), Dehradun 

	

	Name: Anurag Mandal	 University Roll no.: 2021573	
		










Table of Contents  
 
	Chapter No.  	       Description 	     Page No. 
	Chapter 1                                 Introduction   	1-3
	Chapter 2                                 Literature Survey                     4-5
	Chapter 3                                 Methodology 	6-11
	Chapter 4                                 Result and Discussion 	12-15
	Chapter 5                                 Conclusion and Future               16 
		                                    Work  
                                                                         References	 17





















 
# Chapter 1 
Introduction

1)Definition

Person Re-identity (Re-ID): A specialised computer vision assignment focused on figuring out and monitoring people across multiple frames or camera perspectives in a video sequence.
2)Significance in Video Analytics
Enhanced Surveillance: Person Re-ID enhances surveillance systems through imparting the potential to tune people seamlessly thru one-of-a-kind areas included through surveillance cameras
Security Applications: It performs a essential role in safety packages, assisting within the identification of individuals of interest in public spaces, airports, and other excessive-protection environments.

5)Challenges Addressed:
Variations in Appearance: Person Re-ID offers with demanding situations inclusive of adjustments in lighting situations, varying poses, and occlusions, making it a complicated but essential undertaking in video analytics.
6)Role of OpenCV
OpenCV Library: OpenCV, a widely used open-supply laptop imaginative and prescient library, affords vital equipment for photograph and video evaluation, making it a key player in growing character re-identification structures.
Facial Recognition Modules: OpenCV contains facial reputation modules, leveraging algorithms and models for correct face detection and recognition.
7)Key Process Steps
Face Detection: Utilizing OpenCV for face detection, identifying and localizing faces inside every body of a video series.
Feature Extraction: Employing face popularity modules to extract unique facial features, creating extraordinary face encodings.
Matching and Tracking: Comparing face encodings throughout frames to suit and track people as they circulate through one-of-a-kind camera perspectives.

8)Technological Enhancements
Deep Learning Integration: Integration of deep learning architectures, which include Convolutional Neural Networks (CNNs), to beautify feature extraction and recognition accuracy














# Chapter 2
Literature Survey
1)Traditional methods:
Early approaches to human ReID typically rely on artifacts, such as color histograms and texture patterns. These methods have struggled with scalability and robustness in real-world settings due to their inability to capture the complex relationships between individuals across locations

2)Deep learning Example:
Recent years have seen a paradigm shift towards deeper learning for individual ReID. Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) have shown good performance in feature extraction and sequence mapping, respectively These architectures assume a high degree of representation, enabling efficient matching of camera views in various fields.

3)Data types and references:
The development and evaluation of human ReID algorithms rely heavily on standardized data sets and benchmarks. Widely used datasets, such as MARKET-1501 and DukeMTMC, facilitate fair comparison of methods. Evaluation criteria such as cumulative matching characteristic (CMC) curves provide insight into how the algorithm performs at different rank levels.

4)Domain adaptation and transfer learning:
Application of the personal ReID model to real-world scenarios requires robustness to domain changes. Domain optimization and transfer learning methods have emerged to address this challenge, enabling models trained on a data set to generalize effectively to new and unseen areas

5)More ways to work:
To increase the discriminatory power of human ReID systems, researchers are increasingly examining multiple data types. Combining visual cues with other techniques such as deep or contextual information from textual descriptions can significantly improve the accuracy and reliability of the system
 









# Chapter 3 
Methodology

The provided code uses the face_recognition library with OpenCV to generate face recognition and predicted names and ages of individuals in a live video stream Here is a point-by-point breakdown of the methods used is.
1. Library Resources:
• The code comes with important libraries: cv2 for recording and processing video, and face_recognition for facial recognition.
2. Image load:
• Uploads face images for recognition, including the user’s photos and friends’ photos.
3. Forward encodings:
• Calculates face encodings for each input image using the face_recognition.face_encodings function.
4. Video Recording System:
• Start video recording using cv2.VideoCapture(0) to record video from the default camera.
5. Forward Translation Loop:
• Enters a continuous loop to capture frames from the video stream.
6. Know the face:
• Pressing the 'q' key enables face recognition by setting recognize_faces to True.
• Pressing the 'w' key disables face recognition by setting recognize_faces to False.
7. Front Introduction:
• Uses the face_recognition.face_locations function to locate face locations in the current frame.
8. Encoding and face comparison:
• Registers faces in the current frame and compares them to previously computed face codes of the user and his friends.
• Displays the character (name) of the detected person and displays it in the frame.
9. Age Prediction:
• Provides an age value based on the characters of the confirmed person and displays it next to the name.
10. Drawing and Display Boxes:
• Draw a square around a known face and indicates the name and predicted age of the person in the picture.
11. Communication Management:
• The loop continues until the ‘a’ key is pressed, at which point the loop is broken.








# Chapter 4 
Result and Discussion


1. Optional libraries:
• The face_recognition library is a high-quality wrapper to the Dlib library, making it easier to use. However, Dlib can be resource intensive and may not be the most efficient way to detect real face time on some systems. Consideration of other libraries, such as OpenCV’s DNN module with pre-trained face recognition models, can provide better performance.
2. Face recognition debate:
• The code uses a straightforward approach to face detection by comparing face codes. This approach involves fixed identification of individuals and may not be scalable for situations with large dynamic frontal databases. Implementing a more flexible system with additional facial recognition would increase the flexibility of the system.
3. Age of Age Prediction:
• The code includes a special age prediction. However, age estimation from facial photographs is a difficult task and may not achieve accurate results. Integrating a dedicated age estimation algorithm or using pre-trained models to predict age can improve the age prediction.
4. Real-time detection:
• The code allows the user to turn face detection on and off using the ‘q’ and ‘w’ keys. While this feature offers flexibility, adding more sophisticated stimuli or scenarios to activate facial recognition could enhance the user experience and make the system more interactive greater than
5. User Interface:
• The code uses plain text overlays to indicate the name and projected age of the known person. Implementing a more attractive and informative user interface, perhaps using a graphical interface library, can enhance the overall user experience.
6. Efficiency:
• The current implementation handles both forward rules and comparisons for each frame,

 








# Chapter5
Conclusion and Future Work

conclusion:
The code provided lays the foundation for a simple face recognition system using the face_recognition library and OpenCV. It can capture video images, recognize faces, compare them to pre-set facial codes, and display names predicted as individuals of known ages but there are areas for improvement such as library selection, scalability , user interface and performance.
Highlights:
1. Powers:
• The code effectively integrates the face_recognition library for face recognition and recognition.
• Provides a basic means of real-time facial recognition when the capability to detect is activated and deactivated.
2. Areas for improvement:
• choosing the face_recognition library can be critical; Finding alternatives can improve system performance.
• Face recognition logic assumes a fixed set of individuals, which limits scalability. A more dynamic detection system is desirable for real-world situations.
• Age is the most important prognostic factor; Integrating a dedicated age estimation model can increase accuracy.
• User interface can be improved for visual appeal and user interaction.
Future work:
1. Algorithmic improvements:
• Explore and integrate more advanced facial recognition algorithms, which can use deep learning techniques to improve accuracy and performance.
2. Dynamic Database Management:
• Implement strategies to dynamically update and expand the frontal database for a growing number of individuals without requiring changes to the code.
3. Integration of age estimation models:
• Use of unique pre-trained models for age prediction to improve the accuracy and reliability of age estimates.

  REFERENCES 
  
1)The reference was taken from youtube videos for the primary help
For eg: setting up of ANACONDA in my windows laptop and then launching jupyter notebook in my pc,for this the reference was taken from a youtube video link:https://www.youtube.com/watch?v=bkOEYmyMtEU

2)The reference for downloading dlib,cmake and face recognition was done by another youtube video link:https://www.youtube.com/watch?v=h6GSZ19yuXc&list=LL&index=1

3)The rest of the code was written autonomously with little help with another youtube video link:https://www.youtube.com/watch?v=JZZr0PjZsIk

