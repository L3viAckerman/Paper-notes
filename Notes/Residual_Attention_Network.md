# Residual Attention Network for Image Classification 
**TL,DR**: The paper presented new architecture callel Residual Attention Network. The Residual Attention Network is builded by stacking multi block called Residual Module which generate attention-aware features. Inside each attention module, the bottom-up top-down structure is used to calculated the features. The model also use residual connection to make model more deeper. 

**Key points**:
- The model is constructed by stacking multiply Attention Modules. Each Attention Module is divided into two branch, mask branch and trunk branch. Trunk branch is convolutional layer and mask branch is the bottom-up top-down structures to generate the features.
- H(x) = M(x) * T(x).
- Residual attention module : H(x) = (1 + M(x)) * T(x).
- Spatial Attention and Channel Attention.