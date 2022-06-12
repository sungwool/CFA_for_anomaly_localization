# CFA for Target-Oriented Anomaly Localization

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/cfa-coupled-hypersphere-based-feature/anomaly-detection-on-mvtec-ad)](https://paperswithcode.com/sota/anomaly-detection-on-mvtec-ad?p=cfa-coupled-hypersphere-based-feature)

PyTorch implementation of [CFA: Coupled-hypersphere-based Feature Adaptation for Target-Oriented Anomaly Localization](https://arxiv.org/abs/2206.04325) (CFA).

## Getting Started

Install packages with:

```
$ pip install -r requirements.txt
```

## Dataset 

Prepare industrial image as:

``` 
train data:
    dataset_path/class_name/train/good/any_filename.png
    [...]

test data:
    dataset_path/class_name/test/good/any_filename.png
    [...]

    dataset_path/class_name/test/defect_type/any_filename.png
    [...]
``` 

## How to train

### Example
```
python trainer_cfa.py --class_name all --data_path [/path/to/dataset/] --cnn wrn50_2 --Rd False --size 224 --gamma_c 1 --gamma_d 1
```

## Reference
[1] https://github.com/byungjae89/SPADE-pytorch

[2] https://github.com/xiahaifeng1995/PaDiM-Anomaly-Detection-Localization-master

[3] https://github.com/pytorch/vision/tree/main/torchvision/models

[4] https://github.com/lukasruff/Deep-SVDD-PyTorch
