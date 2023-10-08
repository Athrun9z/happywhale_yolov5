# happywhale_yolov5
Problem solved: <br>
In the Awsaf's solution, the training images and labels in the yaml file of the training data are recorded in a txt file.

img1's path
img2's path
img3's path
...

In my yaml file, the path to the whole folder is used. 

train: ... /dataset/images/train # train images (relative to 'path') 128 images

This resulted in me using the full 9850 images from the competition for training, while my labels were only 1200, which greatly confused my model and resulted in a degradation in performance.



previous readme: <br>
This repository is about a competition on kaggle https://www.kaggle.com/competitions/happy-whale-and-dolphin?rvi=1
I'm trying to reproduce Awsaf's code for yolov5, but I'm running into some problems that are causing my model to not work as well as Awsaf's,
and I've been puzzling over it for a long time, so I've decided to ask about it on github.

here is the structure about this repostory:


happywhale_yolov5<br>
│<br>
├── dataset<br>
│   ├── images<br>
│   ├── labels<br>
│<br>
├── make_labels.ipynb # this notebook base on the awsaf's notebook on kaggle  https://www.kaggle.com/code/awsaf49/happywhale-boundingbox-yolov5<br>
│   ├── AnotherFile.txt<br>
│   └── Image.jpg<br>
│<br>
└── yolov5 # clone on ultralytics <br>
 
