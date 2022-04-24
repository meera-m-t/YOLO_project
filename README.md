# YOLO_project
In this repository we crated object detection model that can localize and classify the culvert area in DEM images. We train Yolo v5 in our custom datset. YOLO, or You Only Look Once, is one of the most widely used deep learning based object detection algorithms out there.

## Preprocessing the dataset
Download the [dataset](https://www.dropbox.com/s/ki4a5gryx8y0n6u/Datasets.zip?dl=0)

```bash
unzip Datasets.zip
unzip Sample200by200.zip
```

follow the instructions in ``geography.ipynb ``. Eventually, you will get the folder named ``culvert-dataset`` that contains two folders ``images`` and ``annotations``, as follows 

```bash
unzip culvert-dataset.zip
```


## Convert the Annotations into the YOLO v5 Format
 We convert annotations into the format expected by YOLO v5. There are a variety of formats when it comes to annotations for object detection datasets. Annotations for our dataset follow the PASCAL VOC XML format, which is a very popular format. 
 
 ```bash
 python convert.py
 ```
## Partition the Dataset
We partition the dataset into train, validation, and test sets containing 80%, 10%, and 10% of the data, respectively. You can change the split values according to your convenience. See ``Partition.ipynb``.  You can download this data from [here](https://www.dropbox.com/s/a5n8z2qi1bsa8g4/TRAIN-VAL-TEST.zip?dl=0). 

```bash
unzip TRAIN-VAL-TEST.zip
```

## Set up the yolov5 code
Recommend you create a new conda  environment to run your YOLO v5 experiments as to not mess up dependencies of any existing project. 
```bash
git clone https://github.com/ultralytics/yolov5
cd yolov5
pip install -r requirements.txt
```



