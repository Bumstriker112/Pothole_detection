# Pothole_detection

## Overview
This is a <b>pothole detection project</b>, built with Yolov5. Actually, there are two different models trained with two different datasets. One contains images from a car's dashboard point of view, the other contains random pothole pictures.<br><br>
Thus there are two weights files, <i><b> dash.pt </b></i>, which was trained on images from car's dashboard point of view.<br><br>
and <i> <b>others.pt</b> </i>, which was trained on other random pothole images.

## Requirements

For requirements, see the requirements.txt file. Also, Python 3.8 or later including torch>=1.6. To install run:

```
$ pip install -r requirements.txt
```

## Working

Use this google colab notebook with free GPU: <a href="https://colab.research.google.com/drive/1PJaZn2PfdKZFH-F_9C47uAVzCbEMhyvx?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

Before showing the demo, some important things you should know:

After running the first cell in the notebook, you should get the weights downloaded and stored in a weights folder. You will see two different types of weights as mentioned in the overview section. According to the type of image or video you are running, choose the weights accordingly. If the image/video is captured from dashboard, use <b> dash.pt </b> else it is advised to use <b> others.pt </b>. <br><br>

After this you run the second cell and you should get Yolov5. <br><br>

Now for running inference,in the third and the last cell, pass the path of image/video after the <i><b> --source </i></b> flag and also in the below line in the <i> filename </i> argument. <br><br>

After running inference, your output each time will be saved in the exp folder in runs folder in yolov5 directory. The first time you run inference, output will be stored in yolov5/runs/exp0. The second time you run inference, output will be stored in yolov5/runs/exp1 and so on.

## Demo 

See the below GIF for better a understanding of how to use the colab notebook.

![](demo.gif)
