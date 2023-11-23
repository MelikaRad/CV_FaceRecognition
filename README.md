## Face Recognition
Recognozing faces in input images or video frames in python using OpenCV, YuNet face detection model, and recognition models and tools.
  
The main task of this project:  
given an image of a person with known identity, recognize the person in an input video and draw a green box around the recognized person, as well as drawing red boxes around other faces with non-matching identities.

for simplicity, we first apply the recognition methods on single images, and after that, we apply it on video frames.

#### Project Workflow 
1. Load a face detection model such as YuNet.
2. Detect faces in both the image of a person with a known identity and the image of people with unknown identities.
3. Load a face recognition model for subsequent recognition steps.
4. Crop the detected faces and align them.
5. Obtain face features from facial images.
6. Calculate the identity discrepancy between the known face and unknown faces using the normL2 distance and determine whether or not they are matched using a threshold.
7. Draw bounding boxes obtained from the face detection step, and determine their colors.

After applying these steps on images, the recognition task can be extended to videos, where the recognition task must be applied to each frame of the video. In this project, a video of Christiano Ronaldo was used, and his face was recognized in each frame, with green bounding boxes drawn around his face and red bounding boxes drawn around other faces.
