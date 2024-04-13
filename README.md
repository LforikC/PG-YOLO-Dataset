# PG-YOLO-Dataset: A data set for target detection of immature pomegranate fruits

 [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]
 
## Introduction
This repository is built for:

PG-YOLO-Dataset: A data set for target detection of immature pomegranate fruits

The data set is in YOLO format.

PG-YOLO-Dataset includes pomegranate young fruits in different scenes. The data set contains 13,840 pictures, including 9,798 pictures in the training set and 4,042 pictures in the validation set.

## Directory structure
    ├── images           
        ├── train           // Pictures contained in the training set
        ├── val           // Pictures contained in the validation set
    ├── labels
        ├── train           // Labels corresponding to pictures in the training set
        ├── val           // Labels corresponding to pictures in the validation set
    ├── dataset.yaml          

## How to use
To train a network on the PG-YOLO-Dataset make sure that you download the code first from [yolov8](https://github.com/ultralytics/ultralytics). And then clone this repository to yolov8 folder and  train a yolov8 network with the commands below.

```
# Clone yolov8 repo and install requirements.txt
git clone https://github.com/ultralytics/ultralytics  # clone
cd yolov8
pip install -r requirements.txt  # install
```

```
# Clone this repository to yolov8 folder
git clone https://github.com/LforikC/PG-YOLO-Dataset.
```

```
# Train yolov8
yolo detect train data=PG-YOLO-Dataset/dataset.yaml model=yolov8s.yaml epochs=100 imgsz=640
```



## License

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
