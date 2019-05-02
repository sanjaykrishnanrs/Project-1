# Channel and Kernels



*  **Kernels**
> 1. Kernels applied on an image give Channels.
> 2. Other names of Kernels are *Feature Extractors*, *Filter*
> 3. Kernel convolves on an image which results in an extracted feature -> channel

* **Channels**
> 1. Feature Maps or Channels are the outcome of Feature extractor convolving on the image
> 2. Number of Channels = Number of Kernels applied on the image
> 3. Each channel carries each features. RGB image has 3 channels where each channel carries the respective color values



# 3*3 Kernels

> 1. ODD squared matrix always uplifts the concept of having an anchor pixel in centre and symmetrically considering the neghbour pixels. Even squared matrix won't have anchor pixel and thus resulting in distortion.

> 2. `3*3` kernel is the matrix which consumes less computational power compared to other matrixes during convolution.
`5*5` image --applying `3*3` kernel --> `3*3` image--applying `3*3` kernel -->`1*1` image

>>Here, no: of parameters used = 9 + 9 = 18


>>`5*5` image --applying `5*5` kernel --> `1*1` image
>>Here, no: of parameters used = 25

>>Hence, `3*3` matrix uses less computational power

> 3. Due to above advantage of 3*3 kernel, most of the GPUs are tuned/architected to perform well for 3*3 filter.

# 3x3 convolution operation to reach 1x1 from 199x199 image

99 times we have to apply 3*3 convolution operation to reach `1*1` image from `199*199` image

<img src="https://github.com/sanjaykrishnanrs/Project-1/blob/master/199*199-kernel.png">
