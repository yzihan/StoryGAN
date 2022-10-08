# StoryGAN: A Sequential Conditional GAN for Story Visualization (Python 3.7+, Pytorch 1.6)

## Requirement:
Python 3.7+ (It seems that this repo needs Python 2)
Pytorch 1.6
Opencv-python (cv2)

## Configure File
/code/cfg/clevr.yml is the configure file for the model. This file contains the setup of the dimension of the features, maximum training epoches and etc.

## Prepare
conda create -n storygan python=3.7
conda activate storygan conda install pytorch==1.6.0 torchvision==0.7.0 cudatoolkit=10.2 -c pytorch
conda install tqdm python-dateutil scikit-learn pyyaml
conda install easydict torchfile -c conda-forge

## Check CUDA
nvidia-smi

## Run
To run the code on CLEVR-SV experiment:
```bash
python main_clevr.py
```

## Citation
```bash
@article{li2018storygan,
  title={StoryGAN: A Sequential Conditional GAN for Story Visualization},
  author={Li, Yitong and Gan, Zhe and Shen, Yelong and Liu, Jingjing and Cheng, Yu and Wu, Yuexin and Carin, Lawrence and Carlson, David and Gao, Jianfeng},
  journal={CVPR},
  year={2019}
}
```
