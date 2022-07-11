### Training YOLOV7 on custom dataset
# Step1: Clone the repository
```
git clone --recursive 
```


### Custom dataset structure
```log

├── custom
    ├── images
    │   ├── train
    │   │   ├── train_A.jpg
    │   │   ├── train_B.jpg
    │   │   ├── ...
    │   │   └── train_X.jpg
    │   ├── test
    │   │   ├── test_A.jpg
    │   │   ├── test_B.jpg
    │   │   ├── ...
    │   │   └── test_X.jpg
    │   └── val
    │       ├── val_A.jpg
    │       ├── val_B.jpg
    │       ├── ...
    │       └── val_X.jpg
    ├── labels
    │   ├── train
    │   │   ├── train_A.txt
    │   │   ├── train_B.txt
    │   │   ├── ...
    │   │   └── train_X.txt
    │   ├── test
    │   │   ├── test_A.txt
    │   │   ├── test_B.txt
    │   │   ├── ...
    │   │   └── test_X.txt
    │   └── val
    │       ├── val_A.txt
    │       ├── val_B.txt
    │       ├── ...
    │       └── val_X.txt
    ├── train.txt
    ├── test.txt
    └── val.txt
```


### label text file format 
Label format in yolov7 is same as yolov5



<img src="data/yolov7_label_format.png" width="1200" height="600">

[Image source](https://blog.paperspace.com/content/images/size/w1000/2021/03/image-25.png)

class_id relative_center_x relative_center_y 0.relative_center_width relative_center_height

``` log
0 0.48 0.63 0.69 0.71 
0 0.2646484375 0.505859375 0.03125 0.05078125 
```

