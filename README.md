# ResNext-50 Implementation

ResNeXt is a homogeneous neural network which reduces the number of hyperparameters required by conventional ResNet. This is achieved by their use of "cardinality", an additional dimension on top of the width and depth of ResNet. Cardinality defines the size of the set of transformations.

The basic architecture of ResNeXt is defined by two rules. First, if the blocks produce same-dimensional spatial maps, they share the same set of hyperparameters, and if at all the spatial map is downsampled by a factor of 2, the width of the block is multiplied by a factor of 2.

As seen in the table, ResNeXt-50 has 32 as its cardinality repeated 4 times (depth). The dimensions in
denote the residual block structures, whereas the numbers written adjacent to them refer to the number of stacked blocks. 32 precisely denotes that there are 32 groups in the grouped convolution.
