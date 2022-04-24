# YOLO_project
In this repository we crated object detection model that can localize and classify the culvert area in DEM images. We train Yolo v5 in our custom datset. YOLO, or You Only Look Once, is one of the most widely used deep learning based object detection algorithms out there.

# Preprocessing the dataset
Download the [dataset](https://www.dropbox.com/s/ki4a5gryx8y0n6u/Datasets.zip?dl=0)

```bash
unzip Datasets.zip
unzip Sample200by200.zip
```

follow the instructions in ``geography.ipynb ``. Eventually, you will get the folder named ``culvert-dataset`` that contains two folders ``images`` and ``annotations``.

