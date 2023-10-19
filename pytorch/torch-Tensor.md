# torch.Tensor.detach

# Tensor.detach()

> 返回新的tensor，从计算图中剥离。反向传播时，在此截断，不会接着向前传播。
>
> 常用于冻结前一个网络的参数。

> Returns a new Tensor, detached from the current graph.
>
> The result will never require gradient.
>
> This method also affects forward mode AD gradients and the result will never have forward mode AD gradients.

NOTE

Returned Tensor shares the same storage with the original one. In-place modifications on either of them will be seen, and may trigger errors in correctness checks. IMPORTANT NOTE: Previously, in-place size / stride / storage changes (such as resize_ / resize_as_ / set_ / transpose_) to the returned tensor also update the original tensor. Now, these in-place changes will not update the original tensor anymore, and will instead trigger an error. For sparse tensors: In-place indices / values changes (such as zero_ / copy_ / add_) to the returned tensor will not update the original tensor anymore, and will instead trigger an error.