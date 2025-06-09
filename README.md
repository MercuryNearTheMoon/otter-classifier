# Otter classifier
## Overview
In this project, we developed an image classification model based on a convolutional neural network (CNN) to distinguish between two otter species: the Asian small-clawed otter and the sea otter. To improve performance and reduce training time, we leveraged a pre-trained ResNet model, which has been widely used for visual recognition tasks due to its residual connections and deep architecture.

Before feeding images into the model, we applied a series of data preprocessing and augmentation steps. Each input image is first resized to a fixed resolution of 224x224 pixels to match the expected input size of the ResNet architecture. The images are then converted into PyTorch tensors, and pixel values are scaled to a range of [0, 1].

To improve the model’s robustness and generalization, we applied random horizontal flipping with a probability of 50%. This helps the model learn orientation-invariant features and prevents overfitting on specific poses. Finally, we applied normalization using the standard ImageNet mean and standard deviation, ensuring that the input distribution aligns with the pre-training conditions of the ResNet model.

This preprocessing pipeline ensures consistent input format, enables effective data augmentation, and allows the model to fully leverage the benefits of transfer learning from ImageNet.
## Dataset
<https://github.com/pl2599/Image-Classification-Otters>
