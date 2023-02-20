# Memorizing Autoencoders

Research on memorizing autoencoders.


## Introduction

Autoencoders are useful models for feature learning and data compression, however they typically produce poor reconstructions of out-of-distribution data (ODD). Memorizing autoencoders (MAEs) are a family of autoencoder models which excel in this regard despite intentionally overfitting to a small number of training examples. In this research, we aim to understand why this extrapolation occurs and whether it translates to generative tasks.


## Background

Autoencoders are neural networks which are trained to encode and decode data, typically with a bottleneck layer in the middle. The encoder learns a compact representation of the input data, while the decoder learns to reconstruct the input from the encoded representation. This allows for data compression and feature learning, as well as reconstruction and denoising of the input.

Memorizing autoencoders, on the other hand, intentionally overfit to a small number of training examples. This means that the model is essentially memorizing the input data, rather than generalizing to new, unseen data. Despite this, MAEs have been shown to perform well in extrapolation tasks, where the model is asked to generate data that is outside of the training distribution.


## Examples

Some examples of images compressed by 92% and then decompressed using an MAE trained on a single 1024x1024 image.

<img src='https://github.com/oelin/memorizing-autoencoders/blob/main/images/examples.png'>
