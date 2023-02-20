# Memorizing Autoencoders

Research on memorizing autoencoders.

## About

Autoencoders are useful models for feature learning and data compression, however they typically produce poor reconstructions of out-of-distribution data (ODD). Memorizing autoencoders (MAEs) are a family of autoencoder models which excel in this regard despite intentionally overfitting to a small number of training examples. In this research, we aim to understand why this extrapolation occurs and whether it translates to generative tasks.

## Examples

Reconstructions from an MAE trained on one 1024x1024 image. The compression ratio was set to 95%.

<img src='https://github.com/oelin/memorizing-autoencoders/blob/main/images/examples.jpeg'>
