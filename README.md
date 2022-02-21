# Tensorflow Object Detection
These notebooks demonstrate how to leverage models from TensorFlow Model Zoo to do object detection. It's based on this <a href="https://github.com/nicknochnack/TFODCourse">repo</a>.

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
<b>Step 6.</b> Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the following two folders. <br/>
\TFODCourse\Tensorflow\workspace\images\train<br />
\TFODCourse\Tensorflow\workspace\images\test
<br/><br/>
<b>Step 7.</b> Begin training process by opening <a href="https://github.com/jiahau3/TFOD/blob/main/Training_and_Detection_colab.ipynb">2. Training and Detection.ipynb</a>, this notebook will walk you through installing Tensorflow Object Detection, making detections, saving and exporting your model. 
