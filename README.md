# yolodetction2.0
training
python train.py --workers 1 --device 0 --batch-size 1 --epochs 100 --img 640  --data tanker1/custom_data.yaml --hyp tanker1/hyp.scratch.custom.yaml --cfg cfg/training/yolov7-custom.yaml --name yolov7-custom --weights yolov7.pt

detcting
python detect.py --weights best.pt --conf 0.5 --img-size 640 --source 1.jpg --view-img --no-trace
