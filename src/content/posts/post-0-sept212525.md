---
title: Stable Difusion Experiment - w1
published: 2025-09-21
description: txt2imag experiments with stable difusion automatic1111
tags: [txt2img, stable diffusion, test, automatic1111]
category: test
draft: false
---

## 1.0 Introduction


This will show some examples of the images as result of experiment with the stable difusion in Automatic 1111 google collab.

The collab used from the "stable diffusion art" page [here](https://stable-diffusion-art.com/automatic1111-colab/)

Started with all of the default configurations:

havent figure out how to test it locally yet wiht this template.. 

![AI cat](../../assets/images/post0/cat1.png)
![AI cat](../../assets/images/post0/cat2.png)
![AI cat](../../assets/images/post0/cat3.png)
![AI cat](../../assets/images/post0/cat4.png)

## 2.0 Image size and keyword strength

The next test was to with adding the different strength to the prompt such as (keyword:2) and ((keyword)). 

Found out the reason for the multiple subjects was due to using the image size 1024x1024 which was four times the trianing size of images 512x512. The better workflow is to only generate the 512x512 images, and then to use the upscaler.
Apparently if the strength of the prompt is adjusted so much their remains a lot of noise in the image as can see:

![AI water](../../assets/images/post0/water3.png)
![AI water](../../assets/images/post0/water4.png)
![AI water](../../assets/images/post0/water9.png)
![AI water](../../assets/images/post0/water10.png)

Although it can have cool effect:

![AI water](../../assets/images/post0/water5.png)
![AI water](../../assets/images/post0/water6.png)
![AI water](../../assets/images/post0/water7.png)
![AI water](../../assets/images/post0/water8.png)

The better result was from still having the strengths that were relative high (1.5 to 1.9) range to have some noisy background but it turned into pattern for the water

![AI water](../../assets/images/post0/water1.png)
![AI water](../../assets/images/post0/water2.png)

## Regional Prompter

Next experiment was to try the regional prompter, which did not work very well .. was supposed to be divided horizontally. 
But there was still some interesting result, which the best can see here:

![AI water](../../assets/images/post0/fish1.png)
![AI water](../../assets/images/post0/fish2.png)
![AI water](../../assets/images/post0/fish3.png)
![AI water](../../assets/images/post0/fish4.png)


References:

-https://stable-diffusion-art.com/how-stable-diffusion-work/
-https://stable-diffusion-art.com/automatic1111/
-https://stable-diffusion-art.com/beginners-guide/
-https://huggingface.co/learn/diffusion-course/unit0/1
-SDXL: Improving Latent Diffusion Models for High-Resolution Image Synthesis https://arxiv.org/abs/2307.01952
-SDEdit: Guided Image Synthesis and Editing with Stochastic Differential Equations https://arxiv.org/abs/2108.01073
-High-Resolution Image Synthesis with Latent Diffusion Models https://arxiv.org/pdf/2112.10752