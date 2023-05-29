# Yolov7-light-object detection

## step1
下載yolov7
https://github.com/WongKinYiu/yolov7

## step2
下載資料籍

## step3
將yolov7_light內所有東西放到yolov7資料夾裡面
先下載pytorch GPU
安裝環境

pip install -r requirments.txt

## step3
訓練

python train.py --weights yolov7.pt --hyp data\hyp.scratch.p5.yaml --cfg yolov7-custom.yaml --data custom_data.yaml --img 640 --workers 1 --batch 4 --epochs 150 --name yolov7

## step4
預測

python detect.py --weights yolov7_light.pt --source light_dataset/validation/images --name detect_light


