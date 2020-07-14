# TrainYourOwnYOLO: Building a Custom Object Detector from Scratch

## 1. The Use Case: Helping National Parks Protect Endangered Species
My goal was to develop a use case for object detection. I decided to develop a pipeline that would help in identifying endengered animals from aerial shots (taken from drones or helicopters). The idea is to help national parks by using real-time object detection coupled with readily available drones in order to partly solve problem of poaching and animal extinction in general. 

I used the original code (mentioned below) to build 3 pipelines:

1. Build a pipeline with images taken from normal angles and score it;

2. Build a second pipeline with images taken from above, aeral views and again assess the performance of the model and compare it to the first pipeline;

3. Build a 3rd pipeline for aerial shots that we have taken from our drone and assess how the model is performing

After building the 3 pipelines, the goal is to link the object detector to a livestream broadcasted by my drone, to be able to process real-time footage:

[pipeline](/3_Inference/pipeline.png)

My whole work and a detailed step by step explanation can be found in this [Google Colab Notebook](https://colab.research.google.com/drive/1hJH0TXcwQEljgXfvd9DnYGNO2mgQxcKm?usp=sharing). 


## 2. Original Repository 
I here used and built on the original [repo](https://github.com/AntonMu/TrainYourOwnYOLO) by Anton Muehlemann.
This great repo simplified the building of a custom YOLO Object detector pipeline into 3 steps:

 1. [Image Annotation](/1_Image_Annotation/)
	 - Installing Microsoft's Visual Object Tagging Tool (VoTT)
	 - Annotating images
 2. [Training](/2_Training/)
 	- Downloading pre-trained weights
 	- Training the custom YOLO model on annotated images 
 3. [Inference](/3_Inference/)
 	- Detecting objects in new images and videos

I would recommend visiting the original repository for greater details or the author's [blog post](https://medium.com/@muehle/how-to-train-your-own-yolov3-detector-from-scratch-224d10e55de2).


