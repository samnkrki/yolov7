Step 1:
understand the code
python train.py --workers 8 --device 0 --batch-size 32 --data data/coco.yaml --img 640 640 --cfg cfg/training/yolov7.yaml --weights '' --name yolov7 --hyp data/hyp.scratch.p5.yaml

cfg contains anchors, backbone and head values in a list

data contains data for the particular OD project. It contains train, test and validation folder path, number of classes count and names of those classes in order of they are presented in the train.txt file.

hyp contains hyperparameters that need to be tuned like learning rate, momentum, image augmentation probablities, iou training threshold, anchor multiple threshold

weights sets the initial weights to be loaded

freeze helps freeze the layers of yolov7


- draw the exisitng network
- learn code of deformable convolution
- setup server and anydesks