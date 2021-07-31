# Tensorflow-Object-Detection-From-Scratch
![](https://github.com/Kareem-negm/Tensorflow-Object-Detection-From-Scratch/blob/main/images/final.jpg)
## Instrucures:
- If you face any Error make an issue and I will try to help you but please google it first and if you get the solution put it in the [Error Guide](https://github.com/Kareem-negm/Tensorflow-Object-Detection-From-Scratch-/blob/main/Error%20Guide.md) here you can see the common errors 


# 1. Installation and Setup

- **install python and Anaconda** 

follow this link to install [ananconda](https://repo.anaconda.com/archive/)

- **install Microsoft Visual Studio and C++ Build Tools**

follw this link to install [Visual studio ](https://visualstudio.microsoft.com/vs/community/)
after install visual studio install `desktop development with c++` packge inside the VS 

- **install CUDA Toolkit 10.1 original Archive to speed up your training time and used GPU during the training processing**

follw this link to install [CUDA Toolkit](https://developer.nvidia.com/cuda-10.1-download-archive-base)

- **install CUDNN also recommended I recoommend CUDNN  for you**

you can install [Download cuDNN](https://developer.nvidia.com/rdp/cudnn-archive)

note:you shold insure that the cuDNN version is maches with your TensorFlow version 
you can check from [here](https://www.tensorflow.org/install/source_windows)


- **Install Protoc for Protocol Buffers from the official Github Repo [protoc-3.17.3-win64](https://github.com/protocolbuffers/protobuf/releases/download)**

when you extract the folder I recomend to add it in the followin path you creat `C:\additondalpackges\research`  


dont's miss to add protoc bin path to the system envairnment `PC-properties -advanced system setting -environment variable `

- **Install Tensorflow Object Detection API for use with Python**
clone this repo here https://github.com/tensorflow/models in Git command 
and move your command insid the model folder `cd model ` then write this command `protoc object_detection/protos/*.proto --python_out-.` enter then `copy object_detection/packages/tf2/serup.py .` enter 
then ` python -m pip install .` this will install all of the dependacies like OpenCV , Tensroflw and the other library that we need for our object detection library 

 
# 2. Collecting  Images Using Your Webcam

You can collect the images in the way you prefer, but always remember that the data used for training is similar to the type of data in the test case and similar to the reality that you will deploy the model on, otherwise the detection will be very difficult and inaccurate

# 3.Labelling Images for Object Detection using LabelImg

LabelImg is a graphical image annotation tool.
It is written in Python and uses Qt for its graphical interface.
Annotations are saved as XML files in PASCAL VOC format, the format used by ImageNet. Besides, it also supports YOLO and CreateML formats.
you can learn more about LabelImg and how can use it thro the official [LabelImg](https://github.com/tzutalin/labelImg) Repo

![](https://raw.githubusercontent.com/tzutalin/labelImg/master/demo/demo3.jpg)
