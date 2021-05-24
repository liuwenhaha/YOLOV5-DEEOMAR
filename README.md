本项目是行人轨迹和属性分析的解决方案，检测采用的是[yolov5](https://github.com/ultralytics/yolov5), 跟踪采用的是[deepsort](https://github.com/ZQPei/deep_sort_pytorch)，属性分析采用的是[deepmar](https://github.com/dangweili/pedestrian-attribute-recognition-pytorch),效果[demo](https://www.youtube.com/watch?v=Cu3ERM0Zk4s)

## Requirements

Python 3.7 or later with all `requirements.txt` dependencies installed, including `torch >= 1.5`. To install run:
```bash
$ pip install -U -r requirements.txt
```

## weights
Google drive link:

https://drive.google.com/drive/folders/11qr6Y2c62NzM3BN_011oXLHietiw5tbi?usp=sharing
https://drive.google.com/drive/folders/1r08uwmB3QeOnwkhOupZ0UCC1TIaGybOK?usp=sharing
https://drive.google.com/drive/folders/1KRoWa-VJwgOxWXgywuzwFaq95wDd0QnJ?usp=sharing


## Inference

Inference can be run on most common media formats. Results are saved to `./inference/output`.To run inference on examples in the `./inference/images` folder
```bash

python detect.py --weights "/content/drive/My Drive/yolo weight/yolov5x.pt" 
                 --img 416 
                 --conf 0.4 
                 --source ./inference/images/ 
                 --deepsort ./config/deep_sort.yaml

```
