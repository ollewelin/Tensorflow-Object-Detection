# Tensorflow-Object-Detection
Tensorflow Object Detection from video source instead if the test image1.jpg image2.jpg 
with video.avi instead

 Ubuntu 16.04 

A tedious installation process..

 First I was need to plug in a NVIDIA graphic card 
 then install NVIDIA stuff.. 
 CUDA 9.0 (Pitfall 1. not CUDA 9.2)
 then install
 cuDNN 7.0.5.15 (Pitfall 2. not the latest 7.1.14.18)
 
 install 
 OpenCV 3.4 
 with 
 CMakeGUI
take several houers

 then install
 Tensorflow
 https://www.tensorflow.org/install/install_linux
 Pitfall 3. replace command 
`$ sudo apt-get install cuda-command-line-tools`
 do instead
 `$ sudo apt-get install cuda-command-line-tools-9-0`
 Pitfall 4. replace command 
 `(tensorflow) olle@olle-Aspire-M3800:~/tensorflow/tensorflow$ pip install --upgrade tensorflow-gpu`
 with 
 `$(tensorflow) olle@olle-Aspire-M3800:~/tensorflow/tensorflow$ pip install --upgrade tensorflow-gpu==1.8.0.`
 when testing Tensorflow installation

`$ sudo apt-get install python-opencv`

 I was follow the installation from the 
 https://github.com/tensorflow/models/tree/master/research/object_detection

 but modify the code a little for video.avi input instead of image1.jpg ...
 
 starting the program 
 
 put a video.avi file in the working folder
 
 python object_detection_tutorial.py
 
 https://www.youtube.com/watch?v=j9EDPkt-_H8
