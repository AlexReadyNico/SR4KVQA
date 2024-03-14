

## Installation
安装

### Dependencies
依赖

The original library is build with

- python=3.8.8
- torch=1.10.2
- torchvision=0.11.3

while using decord module to read original videos (so that you don't need to make any transform on your original .mp4 input).

To get all the requirements, please run

```shell
pip install -r requirements.txt
```

### Direct Install
直接安装

You can run

```shell
git clone htps://github.com/QualityAssessment/FAST-VQA-and-FasterVQA.git
cd FAST-VQA-and-FasterVQA
pip install -e .
```

to install the full FAST-VQA with its requirements. The `-e` option allows you to import your customized version of the package.

## Usage
使用方法


### Training
训练

### Get Pretrained Weights from Recognition

You might need to download the original [Swin-T Weights](https://github.com/SwinTransformer/storage/releases/download/v1.0.4/swin_tiny_patch244_window877_kinetics400_1k.pth) to initialize the model.

### Train on the SR4KVQA database 

To train SR4KVQA, please run

```
python new_train.py -o options/fast/fast-m.yml
```


### Testing
测试

### Test on the test set of the SR4KVQA database 

To train SR4KVQA, please run

```
python new_test.py -o options/fast/fast-m-test75.yml
```






