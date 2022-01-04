# FCOS_POSE

Codes for my paper **"STUDENT DANGEROUS BEHAVIOR DETECTION IN SCHOOL"**. Currently, we have only tested the effectiveness of our method on the personal collected danger behavior dataset. You can build a similar dataset by yourself, and transfer our `FCOS_POSE` framework based on FCOS (object detection) and auxiliary keypoints (pose estimation) to your human behavior detection task.

![example1](./materials/network_architecture.png)

## Installition

**Note:** Our `FCOS_POSE` is mostly based on the original [FCOS](https://github.com/tianzhi0549/FCOS). You can follow it to set the environment.

**Environment:** Anaconda, Python3.8, PyTorch1.10.0(CUDA11.2)

```bash
$ git clone https://github.com/hnuzhy/fcos_pose.git
$ pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple

# Codes are only evaluated on GTX3090+CUDA11.2+PyTorch1.10.0. You can follow the same config if needed
# [method 1][directly install from the official website][may slow]
$ pip3 install torch==1.10.0+cu111 torchvision==0.11.1+cu111 torchaudio==0.10.0+cu111 \
  -f https://download.pytorch.org/whl/cu111/torch_stable.html
  
# [method 2]download from the official website and install offline][faster]
$ wget https://download.pytorch.org/whl/cu111/torch-1.10.0%2Bcu111-cp38-cp38-linux_x86_64.whl
$ wget https://download.pytorch.org/whl/cu111/torchvision-0.11.1%2Bcu111-cp38-cp38-linux_x86_64.whl
$ wget https://download.pytorch.org/whl/cu111/torchaudio-0.10.0%2Bcu111-cp38-cp38-linux_x86_64.whl
$ pip3 install torch*.whl
```

## Dataset Preparing
