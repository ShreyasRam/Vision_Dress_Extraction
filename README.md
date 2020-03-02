# Vision_Dress_Extraction

I have used ChainerCV library to support the image segmentation tasks.
refer https://github.com/chainer/chainercv for more details on usage.

Pass an absolute path of the image to be extracted to the "extract" function in the notebook provided.

At first, using Faster RCNN or SSD , the main subject is detected.
Using the bounding box positions we further draw a mask highlighting only the foreground subject and remove the background noise.

Next, using the openCV grabcut algorithm we extract the dress.
This method can be applied to both 1 and 2 datasets.

Required dependencies are bundled in the requirements.txt file.
