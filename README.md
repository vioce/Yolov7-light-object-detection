# Yolov7-light-object detection

## step1
* 下載yolov7 https://github.com/WongKinYiu/yolov7

## step2
* 下載資料集(需要暨大學生信箱)

## step3
* 將所有檔案放到yolov7資料夾裡面
* 先去Pytorch官網下載Pytorch GPU
* https://pytorch.org/get-started/previous-versions/
* 安裝環境
```py
pip install -r requirments.txt
```
## step4
* 訓練
```py
python train.py --weights yolov7.pt --hyp data\hyp.scratch.p5.yaml --cfg yolov7-custom.yaml --data custom_data.yaml --img 640 --workers 1 --batch 4 --epochs 150 --name yolov7
```
## step5
* 預測
```py
python detect.py --weights yolov7_light.pt --source light_dataset/validation/images --name detect_light
```

