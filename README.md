# Deep-Attention-Network
DAN: Deep-Attention Network for 3D Shape Recognition

## _Introduction_

We proposed a Deep-Attention neural network called DAN for 3D shape recognition and retrieval. You can check our paper for more details.

In this repository, our code and data are released for training our DAN on ModelNet40 dataset.

## _Citation_

if you find our work useful in your research, please cite our paper.


## _configuration_
Code is tested under the environment of Pytorch 0.4.1, Python 3.6 and CUDA 9.0 on Ubuntu 16.04.

Dataset: multi-view(12-view) data from ModelNet40 dataset.
Pretrained Model: VGGNet.

## _Usage_
* Download data and pretrained ckpt from above links. Create dir for data as well as result, and place them under corresponding dirs(./data adn ./result/ckpt).

```python
  mkdir -p data result/ckpt
```

* Train DAN. This would use pretrained VGGNet model saved in ./result/ckpt:

```python
  python train_DAN.py
```
* Test DAN. 
```python
  python test_DAN.py
```

## License

Ou code is released under MIT License (see LICENSE file for details).
