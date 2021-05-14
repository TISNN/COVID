# Using Different Deep Learning Models to Detect COVID-19

Final Year Project

Author: Xutianhao from Macau University Of Science And Technology

----------
The code is divided into two parts:

1. Training
Including dataset, training model and generated model transfer.

2. GUI Test
An online detection system by pyqt. You can use this system to test the detction of seven models and Grad-CAM applied to models.

----------

The code partial quote:

utils.py from hysts/pytorch_mixup https://github.com/hysts/pytorch_mixup

cam.py from iz/Grad-CAM.pytorch https://github.com/yizt/Grad-CAM.pytorch

unet_parts.py from milesial/Pytorch-UNet https://github.com/milesial/Pytorch-UNet


----------

How to generate the heat map 

```
python cam.py \
--image_path ... \ # image path
--model_path
```

e.g python cam.py --image_path ./.... --model_path ./......\
        
        python cam.py --image_path ./Images-processed/CT_COVID/2020.01.24.919183-p27-135.png --model_path ./model_backup/medical_transfer/VGG.pth --method gradcam
        
----------

