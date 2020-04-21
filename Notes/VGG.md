# VERY DEEP CONVOLUTIONAL NETWORKS FOR LARGE-SCALE IMAGE RECOGNITION
**TLDR**: The authors proposed using the very small filter in the convolution layers make the networks more depths and worked better. Beside that, by using the small filter (3x3), the total of params is decreasing.

**Key points**
- Replace the large receptive filter in the first layer (5x5, 7x7, 11x11 with big stride) by small filter (3x3)
- Stack 2 layers 3x3 convolution (without activation) is like 5x5, or 3 layer 3x3 like 7x7, but it make model has less params => efficient.
- The authors use 1x1 convolution is the way to increase the non linear of decision funtion without afecting the receptive field of convolution layers. In the paper, the 1x1 is essentially a linear projection onto the space of same dimensionality.
- The authors conjecture that the model required less epoch to converge, due to implicit regularisation imposed by greater depth and smaller conv filter sizes.
