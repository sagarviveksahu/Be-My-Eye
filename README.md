# Be-My-Eye

### Inspiration
We believe that visually impaired people deserve to live independently and pursue their dreams without barriers. Hence, we wanted to build a product for the visually impaired people which gives them a real-time update about the surroundings in terms of speech at all times, help them avoid obstacles and aid them with the power to write programs or documents by just speaking. We believe in to contribute and extend the entire visual impairment application to the opensource community. Also for the true positive captioned image datasets we would like it to be available for all the cloud systems and machine learning API's so that they have better accuracy since we will be providing a pre-processed and clean dataset.

### What it does
Be my eye can form the basis of the system to aid the visually impaired people. The biggest advantage of this product is the camera module is robust and can be a wearable camera, phone camera or a webcam too. This makes it affordable for all the visually impaired people to use. It has the following features:

Object detection: The real-time frames from the camera at all time will capture the surrounding and will signal the visually impaired person if he/she is moving closer to the object or the object is moving closer to the person. This will help the visually impaired people be safe and independent at all times and can avoid serious accidents.

Speech to text conversion: Like us, even the visually impaired people want to pursue their dreams. They want to utilize their brains to be a programmer, a writer or simply just make notes. But lack of vision creates a big barrier between them and their desires. Speech to text conversion feature will help the visually impaired people to speak out the programs and the program will be typed on the screen and the same goes with any document they would want to create.

Video captioning and speech conversion: Visual impairment should not limit them to be aware of the surroundings at all time. This feature will convert the surrounding details in speech so that they are updated about whats around them at all times.

### How we built it
We used the following methodologies to build all three features:

Object detection: We made the object detection using deep learning and OpenCV which is built on top of the tensor flow. We have trained the CNN on the dataset. Once we have our trained model ready we get the objects classified at every frame. We have handled multiple objects in one image. Once the objects are classified we simply draw a bounding box with the height and width details and get the details for xmin, xmax, ymin and ymax for bounding box at all times for every frame. We calculate the probability of colliding with the object and keep a threshold if it is crossed then signal the visually impaired person that he/she is about to collide. Technologies used : Google Tensorflow, Python 3.4, openCV

Speech to text conversion: We used the speech recognition library in python. We used the microphone as the source of input. Wait for a second to let the recognizer calibrate based on the surrounding noise level. Listen to the user's input and convert to text until the user says stop. We have also handled the error when the program does not understand what has been said. We also used speech to text conversion API provided by Microsoft Azure - BING speech API. Technologies used: Python 3.4, BING speech API by Microsoft Azure

Video captioning in real time streaming: We have two implementations for this feature: a. We used Microsoft cognitive image analysis API to get captions for every frame from live input video stream of the camera then convert the caption generated for a particular frame will be converted to speech which will then help the user to understand the surrounding. Technologies used: Python 3.4, Face API, emotions API, computer vision API using Microsoft Azure b. We trained our own neural network: We used VGGnets to calculate the features of images using CNN and convert it to LSTM RNN. Mapping was from 4096 dimensions to 256 dimensions to predict correct captions for images. We want to train models for 150 epochs and test on 25 epochs with every epoch the cost decreases. Technologies used: Tensorflow, Keras, Python

### Challenges we ran into
Learning to code computation-heavy programs with and without the use of GPUs. Integrating modules to unify the project. Fixing errors which were new to StackOverflow.

### Accomplishments that we're proud of
Think of an idea, designing, implementing and deploying in 36 hours. Learning a dozen of APIs, implementing deep learning and computer vision powering it with high-performance computing. Above all keeping up the team spirit and a constant smile to be a part of thrilling learning experience of Coding. Collaborating with engineers from Microsoft, Google, Rubrik, NVIDIA, Fulcrum GT, Facebook, Edge, Qualtrics, Schlumberger, IMO. Hopefully to be a great next addition in one of these and have our dream job.

### What we learned
We learnt a couple of Microsoft Azure APIs, Google Cloud Platform, Tensorflow paving our way towards Machine Learning, deep learning, computer vision and HPC. A rich experience of hacking and learning new technologies. And being proud of Computer Science Community to develop an application for social help and giving encouragement to people with vision impairment.

### What's next for Be My Eye
We have a lot many different modules to extend in Be My Eye. An interactive system which can help a dumb/deaf and a blind to converse overcoming the physical disabilities through technology. Implementing features like operating computers, mobile through speech and other assistive technologies like integrated cameras, wearables to make their day to day life tasks easier. We are extremely happy to contribute to healthcare and empowering the community by making the application widely available.

### Built With
Microsoft-cognitive-image-analyzing-api
Microsoft-cognitive-text-to-speech-api
Microsoft Azure
Google Cloud Platform
Tensorflow
Caffe
Computer-vision
Opencv
Python
Machine-learning
Deep-learning
Natural-language-processing
