# Deep Residual Learning for Image Recognition arXiv:1512.03385v1
**TL,DR**: The paper proposed the new architecture for building block called Residual block. Residual block is showed that it can make the model become more deeper and efficient. It resolved the problem that when the model become deep, the loss increase.
**Key notes**:
- Residual connections is y = F(x, W) + x, where F is representation of 2 or 3 layer convolution. The authors suggest it should not be 1 layer convolution.
- For the correction of demension, we have the identity shortcut y = F(x, W) + x or projection shortcut y = F(x, W) + W(x). Because the projection shortcut not show the much better than any shortcut, the authors did not use them to reduce the cost of computing.
- The bottleneck design are showed as a way to make the model efficient in compute. They use 1x1 convolution to reduce the dimensional on depth and next increase that.