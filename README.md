# Coral Density Analysis using Deep Learning

This repository contains the LaTeX source code for my MEng Computer Science thesis at the University of Bristol. The full PDF is available [here](https://github.com/ainsleyrutterford/Thesis/blob/master/Thesis.pdf) and the accompanying code written throughout is available in [this repository](https://github.com/ainsleyrutterford/DeepC).

<p align="center">
  <img src="https://raw.githubusercontent.com/ainsleyrutterford/Thesis/master/images/real-coral.png" height=300>
  <img src="https://raw.githubusercontent.com/ainsleyrutterford/Thesis/master/images/3D-scan.png" height=300>
</p>

### Abstract

This project uses deep learning to automate the estimation of the amount of skeletal matter produced
annually by corals. In particular, the U-Net architecture is successfully modified to automatically label
the density bands present in two dimensional slices of coral. This is the first time that deep learning
techniques have been used to process coral density data of any kind. To train the U-Net based network, a
dataset containing ∼400 images is curated using slices extracted from four different three dimensional CT
scans of coral skeletons. Various data augmentation techniques are used to artificially expand the dataset
and improve the performance achieved. In order to effectively measure performance, an accuracy metric
based off the average Euclidean distance between predicted and ground truth boundaries is conceived.
Various ablation studies and rigorous quantitative and qualitative evaluation are applied to pinpoint
performance and limitations. An ablated version of the U-Net architecture was found to perform better
in this task and ultimately achieved a cross-validated accuracy of 77.8%.

The automatic labelling of the banding present in three dimensions is also explored. To this end, the
U-Net architecture is modified to process three dimensional data, and a custom three dimensional data
loader capable of online augmentation is implemented. In order to train this network, a larger dataset
of manually labelled adjacent slices is curated, containing over 3,400 images extracted from four coral
samples.

The densities of the coral skeletons and the distances between the density bands extracted by the network
are automatically estimated using various classical image processing techniques. These estimates are
used to automatically calculate the amount of skeletal matter produced annually and the final automated
calculations are similar to the manual calculations reported in the literature.
