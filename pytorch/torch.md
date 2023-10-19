# torch

[TOC]

# torch.argmax

> 返回最大值对应的索引，默认把所有维度压缩，返回一个值。
>
> dim参数（int）表示要规约的维度
>
> keepdim：是否保持原始tensor维度，默认false

```
torch.argmax(*input*, *dim*, *keepdim=False*) → LongTensor
```

Returns the indices of the maximum values of a tensor across a dimension.

This is the second value returned by [`torch.max()`](https://pytorch.org/docs/stable/generated/torch.max.html#torch.max). See its documentation for the exact semantics of this method.

- Parameters

  **input** ([*Tensor*](https://pytorch.org/docs/stable/tensors.html#torch.Tensor)) – the input tensor.**dim** ([*int*](https://docs.python.org/3/library/functions.html#int)) – the dimension to reduce. If `None`, the argmax of the flattened input is returned.**keepdim** ([*bool*](https://docs.python.org/3/library/functions.html#bool)) – whether the output tensor has `dim` retained or not. Ignored if `dim=None`.

Example:

```
>>> a = torch.randn(4, 4)
>>> a
tensor([[ 1.3398,  0.2663, -0.2686,  0.2450],
        [-0.7401, -0.8805, -0.3402, -1.1936],
        [ 0.4907, -1.3948, -1.0691, -0.3132],
        [-1.6092,  0.5419, -0.2993,  0.3195]])
>>> torch.argmax(a, dim=1)
tensor([ 0,  2,  0,  1])
```