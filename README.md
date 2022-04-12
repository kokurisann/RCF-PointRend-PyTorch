# RCF-PointRend-PyTorch

### RCF-PointRend-PyTorch

Thanks to Li Liang's help.
The best result of my pytorch model is 0.783 ODS F-score now.

#### My model

![](C:\Users\song\Documents\Tencent Files\492613337\FileRecv\RCF_new.jpg)

### Introduction

The result of my pytorch model will be released in the future

| Method        | ODS F-score on BSDS500 dataset |
| :------------ | :----------------------------: |
| RCF-PointRend |             0.808              |
| RCF-MS        |             0.811              |


### Installation

Install <a href="https://pytorch.org/">pytorch</a>. The code is tested under 11.6 cuda version and Python 3.9  on Ubuntu 20.04. There are also some dependencies for a few Python libraries for data processing and visualizations like `cv2` etc. It's highly recommended that you have access to GPUs.

### Usage

#### Image edge detection

To train a RCF-PointRend model on BSDS500:

        python train_RCF_PointRend.py

To resume the training on BSDS500:

```
	python train_RCF_PointRend.py --checkpoint '[.pth file]'
```

If you have multiple GPUs on your machine, you can also run the multi-GPU version training:

        CUDA_VISIBLE_DEVICES=0,1 python train_multi_gpu.py --num_gpus 2

### Source：

*  To download the pretrained model, please click https://drive.google.com/open?id=1TupHeoBKawrniDka0Hc64m3BG4OKG8nM (This pretrained model is not the best model, just for communicating)
*  To download the vgg16 pretrained model which is used for the backbone. please click https://drive.google.com/file/d/1lUhPKKj-BSOH7yQL0mOIavvrUbjydPp5/view?usp=sharing.
*  To download the HED-BSDS_PASCAL dataset. Please click https://pan.baidu.com/s/13be7JVWzbup_h-04axRrSw (Access Code: 2nzk).
*  To evaluate the model, you can learn more information in https://www.jianshu.com/p/eda277063867.
