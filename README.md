# Memorizing Autoencoders

Research on memorizing autoencoders.

## Introduction

Autoencoders are useful models for feature learning and data compression, however they typically produce poor reconstructions on out-of-distribution data. Memorizing autoencoders (MAEs) are a family of autoencoder models which excel in this task despite intentionally overfitting to a small number of training examples. In this project we aim to understand why MAEs exhibit this surprising behaviour.

## Examples

Reconstructions from an MAE trained on one 1024x1024 image. Compression ratio: 0.95.

<img src='https://github.com/oelin/memorizing-autoencoders/blob/main/images/examples.jpeg'>


## Research Questions

So far initial research has been done into MAEs showing that they're capable of significantly compressing diverse images after grossly overfitting to a single image. This observation poses a number of interesting questions.

### Which architectures mimic MAEs?

The MAE phenomenon was first observed in convolutional autoencoders, however it's possible other architectures also support similar behaviour. Of particular interest are variational autoencoders and other explicitly generative architectures. 

### Which modalities do MAEs work on?

Autoencoders are frequently used to compress images, however they can also be used with oher modalities. Does the MAE phenomenon translates over to these other contexts?

### Why Do MAEs work?

It's intuitively very surprising that models trained on a single image are able to learn a transformation for compressing images in general. We would like to understand why this phenomenon occurs.


### What are the limitations of MAEs?

How does reducing the encoder bottleneck affect reconstruction performance on unseen images?
