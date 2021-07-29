Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

We changed it for training our own data for vehicle detection.

we have uploaded our configuration file and dataset.

To train it,

Follow the steps: 
</br>1. git clone https://github.com/BuddyZhu/modified_darknet.git
</br>2. make
</br>3. wget https://pjreddie.com/media/files/darknet53.conv.74 
</br>4. donwload training images from https://drive.google.com/drive/folders/1uYSbwhs1I35aZQksUlZBi-aXSBRYj4Nr?usp=sharing and put them into /data/obj_train_data
</br>5. cd ~/modfied_darknet 
</br>6. ./modfied_darknet detector train /cfg/obj.data /cfg/yolov3-tiny.cfg ./darknet53.conv.74 > /backup/train.log

The trained weights will be saved in /backup/weights/yolov3-tiny_final.weights

For more information see the Darknet project website.



