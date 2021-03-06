# cil-road-segmentation

## Useful papers & thesis
- [Road Structure Refined CNN for Road Extraction in Aerial Image - May 2017](http://ieeexplore.ieee.org/document/7876793/#full-text-section)
- [pix2pix](https://arxiv.org/abs/1611.07004)
- [Machine Learning for Aerial Image Labeling](https://www.cs.toronto.edu/~vmnih/docs/Mnih_Volodymyr_PhD_Thesis.pdf)
- [SEMANTIC SEGMENTATION OF AERIAL IMAGES WITH AN ENSEMBLE OF CNNS](https://www.ethz.ch/content/dam/ethz/special-interest/baug/igp/photogrammetry-remote-sensing-dam/documents/pdf/marmanis-isprs16.pdf)
- [Learning to Detect Roads in High-Resolution Aerial Images](http://www.cs.toronto.edu/~fritz/absps/road_detection.pdf)
- [CycleGAN](https://junyanz.github.io/CycleGAN/)
- [Fully Convolutional Networks for Semantic Segmentation (CVPR)](https://people.eecs.berkeley.edu/~jonlong/long_shelhamer_fcn.pdf)
- [SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation (2016)](https://arxiv.org/pdf/1511.00561.pdf)
- [Kaggle Satellite Image Segmentation Competition]
(https://deepsense.io/deep-learning-for-satellite-imagery-via-image-segmentation/)
(http://blog.kaggle.com/2017/04/26/dstl-satellite-imagery-competition-1st-place-winners-interview-kyle-lee/?utm_source=Mailing%20list&utm_campaign=f1be30eedd-Kaggle_Newsletter_05-04-2017&utm_medium=email&utm_term=0_f42f9df1e1-f1be30eedd-400419961)


## Possible extra datasets
- [Road and Building Detection Datasets](https://www.cs.toronto.edu/~vmnih/data/)
- [Maps dataset from pix2pix work](https://people.eecs.berkeley.edu/~tinghuiz/projects/pix2pix/datasets/)
- [Maps dataset from CycleGAN work](https://people.eecs.berkeley.edu/~taesung_park/CycleGAN/datasets/)
- [Vlodmir Mnih Dataset](https://www.cs.toronto.edu/~vmnih/data/)

## TODO / Next Step
1. Fix the dataset
options
a. pix2pix dataset + rotation
b. CIL dataset + rotation
c. Mnih dataset (if we figure out how to remove the white patches in some of the images)
2. Decide on the input size of the image (next step depends on this)
3. Get the distance map (see the loss function part of the paper)
4. If we're using the pix2pix dataset, how to convert google map images to road segmentation maps (white for road, black for non-road)
5. Get the deconv according to the paper efficiently (use the conv2d_transpose and upsample right now)

After the above, we will be able to run the network and get numbers