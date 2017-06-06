---
layout: post
title:  "Sample-level Deep Convolutional Neural Networks for Music Auto-tagging Using Raw Waveforms"
date:   2017-06-05 11:42:00
categories: Research Music Auto-Tagging
---

<p align="center">
  <img src="/assets/images/smc2017/smc1.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>
We propose sample-level deep convolutional neural networks which learn representations from very small grains of waveforms (e.g. 2 or 3 samples) beyond typical frame-level input representations. In addition, we visualize filters learned in a sample-level DCNN in each layer to identify hierarchically learned features and show that they are sensitive to log-scaled frequency along layer, such as mel-frequency spectrogram that is widely used in music classification systems.

<p align="center">
<strong>Background</strong>: Learning from raw data in the image domain.
  <img src="/assets/images/smc2017/smc2.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Background</strong>: Learning from raw data in the text domain.
  <img src="/assets/images/smc2017/smc3.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Background</strong>: Learning from raw data in the audio domain.
  <img src="/assets/images/smc2017/smc4.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Frame-level Mel-spectrogram model</strong>: Mel-spectrograms are powerful, but this process is separated from the training phase.
  <img src="/assets/images/smc2017/smc5.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Frame-level Raw waveform model</strong>: Previous studies have attempted to replace the Mel-spectrogram stage with Single Large filter CNN layer.
  <img src="/assets/images/smc2017/smc6.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Sample-level Raw waveform model</strong>: Let's use a deeper CNN with small filters.
  <img src="/assets/images/smc2017/smc7.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Comparison</strong>: Results of three comparative models.
  <img src="/assets/images/smc2017/smc8.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Trend 1</strong>: Deeper models with smaller filters increase performance.
  <img src="/assets/images/smc2017/smc9.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Trend 2</strong>:  Deeper models (about 10 layers or more).
  <img src="/assets/images/smc2017/smc10.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Trend 3</strong>: 1-5 seconds network input.
  <img src="/assets/images/smc2017/smc11.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Gradient Ascent Method</strong>: Convolution operation.
  <img src="/assets/images/smc2017/smc12.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Gradient Ascent Method</strong>: Loss is set to target filter to maximize the activation of the estimated filter shape.
  <img src="/assets/images/smc2017/smc13.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Gradient Ascent Method</strong>: Add the back-propagated value to input noise.
  <img src="/assets/images/smc2017/smc14.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Gradient Ascent Method</strong>: Repeat several steps.
  <img src="/assets/images/smc2017/smc15.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Gradient Ascent Method</strong>: Run the same steps for different filters.
  <img src="/assets/images/smc2017/smc16.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Gradient Ascent Method</strong>: The filter shape estimate is obtained at the input signal.
  <img src="/assets/images/smc2017/smc17.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Filter Visualization</strong>: To show the spectrums effectively, we use typical frame-size input (e.g. 729 samples).
  <img src="/assets/images/smc2017/smc18.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>

<p align="center">
<strong>Filter Visualization</strong>: We can see that they are sensitive to log-scaled frequency
along layer, such as mel-frequency spectrogram that is widely used in music classification systems.
  <img src="/assets/images/smc2017/smc19.jpeg" alt="Sample-level" style="max-width: 100%;">
</p>



Check out the [paper][arXiv] for more info.

[arXiv]:    https://arxiv.org/abs/1703.01789
