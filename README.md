<h2 align="center">YoloOW: A Spatial Scale Adaptive Real-time Object Detection Neural Network for Open Water Search and Rescue from UAV Aerial Imagery</h2>
<div align="center">
  <img src="https://github.com/Xjh-UCAS/YoloOW/assets/95291196/27599265-43ff-4470-bf73-7e5b7222d4ac" width="400">
</div>

This is the Link to the paper "[YoloOW: A Spatial Scale Adaptive Real-time Object Detection Neural Network for Open Water Search and Rescue from UAV Aerial Imagery](https://ieeexplore.ieee.org/abstract/document/10517350)"

## Introduction
In this paper, we proposed a real-time object detection neural network named YoloOW that adapts to different spatial scales for improved object detection performance in open water search and rescue from UAV aerial imagery. Three new model architectures were proposed in the YoloOW model to improve scale adaptability: OaohRep block, DELAN and its enhanced variant E-DELAN, and OaohRepBi-PAN. The YoloOW model underwent quantitative evaluation in accuracy, speed, and model size. It has outperformed all other models with 37.18AP, securing the top position on the leaderboard. Additionally, it achieves a speed of 65.3 FPS, which is faster than any other model with similar accuracy. Moreover, the YoloOW model has only 2.8M more parameters than the lightest model, Yolov7, in model size.
<div align="center">
  <img src="https://github.com/Xjh-UCAS/YoloOW/assets/95291196/cfe89235-d8e5-44e9-8b7f-3082ff8df498">
</div>

## Train
python train.py --workers 8 --device 0 --batch-size 4 --data data/sea_drones_see.yaml --img 1280  --cfg cfg/training/yoloOW.yaml --weights 'yoloow.pt' --name yoloOW --hyp data/hyp.scratch.sea.yaml --epoch 300

## Implementations
"[YoloOW.pt](https://github.com/Xjh-UCAS/YoloOW/releases/download/v0.1/YoloOW.pt)"


