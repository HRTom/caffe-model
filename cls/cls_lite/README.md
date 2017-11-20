## CLS Lite (Classification lite)

Please install [py-RFCN-priv](https://github.com/soeaver/py-RFCN-priv) for evaluating and finetuning.


### Performance of lite models on imagenet validation.
**1. Top-1/5 error and CPU/GPU speed of lite models in this repository.**

 Network|Top-1/5 error|F/B on GPU|F/B on CPU|Source
 :---:|:---:|:---:|:---:|:---:
 resnet18-priv | 29.11/10.07 | 4.48/5.07ms | 213.2/193.3ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)
 resnet18-1x96d | 26.11/8.31 | 6.16/9.94ms | 443.2/419.0ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)
 resnet18-1x128d | 24.81/7.61 | 9.75/16.94ms | 729.1/695.4ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)
 vgg13-pytorch | 31.07/11.13 | 5.70/9.35ms | 1318/1279ms | [vision](https://github.com/pytorch/vision/tree/master/torchvision/models)
 vgg13bn-pytorch | 29.50/10.18 | 8.35/13.49ms | 1443/1336ms | [vision](https://github.com/pytorch/vision/tree/master/torchvision/models)
 vgg16-pytorch | 29.14/10.00 | 6.79/11.78ms | 1684/1643ms | [vision](https://github.com/pytorch/vision/tree/master/torchvision/models)
 vgg16-tf | 29.03/10.12 | 13.04/48.90ms | 1787/1647ms | [tf-slim](https://github.com/tensorflow/models/tree/master/research/slim)
 vgg16-dsd | 27.62/9.02 | 6.81/11.80ms | 1753/1660ms | [dsd](https://github.com/songhan/DSD)
 vgg16-5x | 31.67/11.60 | 4.46/7.15ms | 580.5/593.0ms | [channel-pruning](https://github.com/yihui-he/channel-pruning)
 vgg16-3c4x | 28.79/9.78 | 7.53/9.77ms | 753.4/772.4ms | [channel-pruning](https://github.com/yihui-he/channel-pruning)
 vgg16bn-pytorch | 27.53/8.99 | 9.14/15.83ms | 1783/1695ms | [vision](https://github.com/pytorch/vision/tree/master/torchvision/models)
 vgg19-pytorch | 28.23/9.60 | 8.03/14.26ms | 2076/2012ms | [vision](https://github.com/pytorch/vision/tree/master/torchvision/models)
 vgg19bn-pytorch | 26.58/8.45 | 10.75/18.77ms | 2224/2081ms | [vision](https://github.com/pytorch/vision/tree/master/torchvision/models)
 air14-1x16d  | -- | 5.13/3.56ms | 45.5/6.4ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)
 air26-1x16d  | -- | 7.32/4.70ms | 62.0/8.5ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)
 air26-1x32d  | 28.71/9.59 | 8.77/5.05ms | 170.7/19.25ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)
 air50-1x16d  | 31.19/11.26 | 14.73/8.31ms | 91.65/16.06ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)
 air50-1x32d  | -- | 15.39/7.64ms | 229.6/22.81ms | [pytorch-classification](https://github.com/soeaver/pytorch-classification)