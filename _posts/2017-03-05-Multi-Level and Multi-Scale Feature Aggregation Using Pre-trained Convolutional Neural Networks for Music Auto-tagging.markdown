---
layout: post
title:  "Multi-Level and Multi-Scale Feature Aggregation Using Pre-trained Convolutional Neural Networks for Music Auto-tagging"
date:   2017-03-05 11:41:00
categories: Research Music Auto-Tagging
---

<p align="center">
  <img src="/assets/images/spl2017/spl1.png" alt="Multi-level" style="max-width: 100%;">
</p>
Music auto-tagging is often handled in a similar manner to image classification by regarding the 2D audio spectrogram as image data. However, music auto-tagging is distinguished from image classification in that the tags are highly diverse and have different levels of abstractions. Considering this issue, we propose a convolutional neural networks (CNN)-based Feature Aggregation Method that embraces multi-level and multi-scaled features.

<p align="center">
<strong>Motivation</strong>: Hierarchy in Music.
  <img src="/assets/images/spl2017/spl2.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Motivation</strong>: Music tags with various levels of abstraction.
  <img src="/assets/images/spl2017/spl3.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Motivation</strong>: Code music using CNN's last hidden layer?.
  <img src="/assets/images/spl2017/spl4.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Motivation</strong>: Let's use the intermediate layer Features.
  <img src="/assets/images/spl2017/spl5.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Motivation</strong>: We can also consider multi-scale Features by using several pre-trained CNN with different input sizes.
  <img src="/assets/images/spl2017/spl6.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Pre-training</strong>: Let's make Feature extractors.
  <img src="/assets/images/spl2017/spl7.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Pre-training</strong>: Let's make Feature extractors.
  <img src="/assets/images/spl2017/spl8.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Pre-training</strong>: Let's make Feature extractors.
  <img src="/assets/images/spl2017/spl9.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Feature extraction</strong>: To better capture local characteristics, frame-wise dimension is max-pooled to 1. After, average pooling is applied on whole segments of a song. Then, the feature size of each layer become equal to the number of filters on each layer.
  <img src="/assets/images/spl2017/spl10.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Feature extraction</strong>: Another Feature Aggregation.
  <img src="/assets/images/spl2017/spl11.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Feature extraction</strong>: Another Feature Aggregation in different scale.
  <img src="/assets/images/spl2017/spl12.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Rich Features</strong>: Song-level Aggregated Features are now obtained.
  <img src="/assets/images/spl2017/spl13.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Classification</strong>: Classify using DNNs.
  <img src="/assets/images/spl2017/spl14.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Transfer Learning</strong>: Since our method consist of two stages, transfer learning is easily applied.
  <img src="/assets/images/spl2017/spl15.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Datasets</strong>: MSD, Tagtraum, MTAT, GTZAN.
  <img src="/assets/images/spl2017/spl16.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Results</strong>: Comparisons.
  <img src="/assets/images/spl2017/spl17.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Analysis</strong>: We can see that some tags are indeed located at different levels and scales.
  <img src="/assets/images/spl2017/spl18.jpeg" alt="Multi-level" style="max-width: 100%;">
</p>


Check out the [paper][arXiv] for more info.

[arXiv]:    https://arxiv.org/abs/1703.01793
