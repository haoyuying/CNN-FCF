# CNN-FCF
This is a Pytorch implementation of our paper "Compressing Convolutional Neural Networks via Factorized Convolutional Filters" published in CVPR 2019.

## Requirements
- Python 3.6
- PyTorch 0.3.1
- TorchVision 0.2.0

## Models and log files
The trained models with log files can be found in [Google Drive](https://drive.google.com/drive/folders/1VGqpOhAGe9YQcyZTGbzitsLuELjQdsXW).

## reproduce the CIFAR-10 results in our paper
```
python inference_cifar.py --model 'resnet20' -n 6 -reference-model 'resnet20_cifar_full.pkl' -finetune-model 'finetune_model_checkpoint' 

python inference_cifar.py --model 'resnet32' -n 10 -reference-model 'resnet32_cifar_full.pkl' -finetune-model 'finetune_model_checkpoint' 

python inference_cifar.py --model 'resnet56' -n 18 -reference-model 'resnet56_cifar_full.pkl' -finetune-model 'finetune_model_checkpoint' 

python inference_cifar.py --model 'resnet110' -n 36 -reference-model 'resnet110_cifar_full.pkl' -finetune-model 'finetune_model_checkpoint'
```

## reproduce the ImageNet results in our paper
```
python inference_imagenet_resnet34.py --model 'resnet34' -reference-model 'resnet34-333f7ec4.pth' -finetune-model 'finetune_model_checkpoint' 

python inference_imagenet_resnet50.py --model 'resnet50' -reference-model 'resnet50-19c8e357.pth' -finetune-model 'finetune_model_checkpoint' 

```
