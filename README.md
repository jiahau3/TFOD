# Tensorflow Object Detection
These notebooks demonstrate how to leverage models from TensorFlow Model Zoo to do object detection. It's based on this <a href="https://github.com/nicknochnack/TFODCourse">repo</a>. The workflow is as follows. A user labels customized object characterstics by using LabelImg tool. They are the labels of images that captured by user's image capture equipment. After finshing labelling, images are compressed for using Colab to train. The detail shows in this <a href="https://github.com/jiahau3/TFOD/blob/main/1.%20Image%20Collection.ipynb">notebook</a>.
To perform object detection, TensorFlow Object Detection API is implemented. Taking advantage of transfer learning, the pre-trained model is used from <a href="https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md">TensoFlow Model Zoo</a>. Model SSD MobileNet V2 FPNLite 320x320 is chosen for its high process speed without losing too much accuracy. 
## Steps
<br />
<b>Step 1.</b> Clone this repository: https://github.com/nicknochnack/TFODCourse
<br/><br/>
<b>Step 2.</b> Create a new virtual environment
<pre>
conda create -n ENVNAME python=3.7
</pre> 
<br/>
<b>Step 3.</b> Activate your virtual environment
<pre>
conda activate ENVNAME
</pre>
<br/>
<b>Step 4.</b> Install dependencies and add virtual environment to the Python Kernel
<pre>
python -m pip install --upgrade pip
pip install ipykernel
python -m ipykernel install --user --name=ENVNAME
</pre>
<br/>
<b>Step 5.</b> Collect images using the Notebook <a href="https://github.com/jiahau3/TFOD/blob/main/1.%20Image%20Collection.ipynb">1. Image Collection.ipynb</a> - ensure you change the kernel to the virtual environment as shown below
<img src="https://i.imgur.com/8yac6Xl.png"> 
<br/>
<b>Step 6.</b> Manually divide collected images into two folders train and test. For example, folders and annotations should be split between the following two folders. <br/>
\TFOD\Tensorflow\workspace\images\train<br />
\TFOD\Tensorflow\workspace\images\test
<br/><br/>
<b>Step 7.</b> Begin training process by opening <a href="https://github.com/jiahau3/TFOD/blob/main/Training_and_Detection_colab.ipynb">2. Training and Detection.ipynb</a>, this notebook will walk you through installing Tensorflow Object Detection, making detections, saving and exporting your model. 
