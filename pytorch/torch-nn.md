# torch.nn模块

[TOC]



- [Containers](https://pytorch.org/docs/stable/nn.html#containers)
- [Convolution Layers](https://pytorch.org/docs/stable/nn.html#convolution-layers)
- [Pooling layers](https://pytorch.org/docs/stable/nn.html#pooling-layers)
- [Padding Layers](https://pytorch.org/docs/stable/nn.html#padding-layers)
- [Non-linear Activations (weighted sum, nonlinearity)](https://pytorch.org/docs/stable/nn.html#non-linear-activations-weighted-sum-nonlinearity)
- [Non-linear Activations (other)](https://pytorch.org/docs/stable/nn.html#non-linear-activations-other)
- [Normalization Layers](https://pytorch.org/docs/stable/nn.html#normalization-layers)
- [Recurrent Layers](https://pytorch.org/docs/stable/nn.html#recurrent-layers)
- [Transformer Layers](https://pytorch.org/docs/stable/nn.html#transformer-layers)
- [Linear Layers](https://pytorch.org/docs/stable/nn.html#linear-layers)
- [Dropout Layers](https://pytorch.org/docs/stable/nn.html#dropout-layers)
- [Sparse Layers](https://pytorch.org/docs/stable/nn.html#sparse-layers)
- [Distance Functions](https://pytorch.org/docs/stable/nn.html#distance-functions)
- [Loss Functions](https://pytorch.org/docs/stable/nn.html#loss-functions)
- [Vision Layers](https://pytorch.org/docs/stable/nn.html#vision-layers)
- [Shuffle Layers](https://pytorch.org/docs/stable/nn.html#shuffle-layers)
- [DataParallel Layers (multi-GPU, distributed)](https://pytorch.org/docs/stable/nn.html#module-torch.nn.parallel)
- [Utilities](https://pytorch.org/docs/stable/nn.html#module-torch.nn.utils)
- [Quantized Functions](https://pytorch.org/docs/stable/nn.html#quantized-functions)
- [Lazy Modules Initialization](https://pytorch.org/docs/stable/nn.html#lazy-modules-initialization)

# Utilities

## FLATTEN

类Flatten，负责把一个张量一维化，默认把除了第一个维度的压平。可以传参指定

> *CLASS*torch.nn.Flatten(*start_dim=1*, *end_dim=-1*)[[SOURCE\]](https://pytorch.org/docs/stable/_modules/torch/nn/modules/flatten.html#Flatten)
>
> Flattens a contiguous range of dims into a tensor. For use with `Sequential`. See [`torch.flatten()`](https://pytorch.org/docs/stable/generated/torch.flatten.html#torch.flatten) for details.

![image-20231019143504740](D:\2.git-repository\专业笔记\pytorch\assets\torch-nn.assets\image-20231019143504740-16976973087541.png)