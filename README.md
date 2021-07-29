Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

We changed it for training our own data for vehicle detection.

we have uploaded our configuration file and dataset.

To train it,

First do: 
</br>git clone https://github.com/BuddyZhu/modified_darknet.git

</br>then:
</br>make 

</br>last: 
</br>cd ~/modfied_darknet ./modfied_darknet detector train /cfg/obj.data /cfg/yolov3-tiny.cfg ./darknet53.conv.74 > /backup/train.log

The trained weights will be saved in /backup/weights/yolov3-tiny_final.weights

For more information see the Darknet project website.

For questions or issues please use the Google Group.

./darknet detector train /path/to/snowman/darknet.data /path/to/snowman/darknet-yolov3.cfg ./darknet53.conv.74 > /path/to/snowman/train.log
