---
layout: post
title: Machine Learning Code Challenge by SETI and IBM
subtitle: Improve classification of radio signals from cosmic sources 
gh-repo: probabilityfilter
gh-badge: [star, fork, follow]
tags: [Machine Learning, Data Analysis, Jupyter Notebooks, Python, NumPy, astronomy]
comments: true
---

## Code Challenge

The Code Challenge was whole different animal since we had to deal with a low SNR and the number of signal classes went up from 4 to 7. My Hackathon methods did not rescue me!! Many of the signals were invisible to the eye, extreme data processing was required to start seeing these signals. [Code](https://github.com/probabilityfilter/ML-SETI-IBM/blob/master/notebooks/ArunBasic_DSP_try.ipynb).

Here is one signal; top figure - hard to discern the signal, middle figure - better after adjusting amplitude and removing color, last figure - actual signal  
![Compare](/img/SETI Code Challenge/Compare.jpg "Barely visible"){: .center-block :}  

Here is a challenging one; top figure - impossible to see the signal, bottom figure - slight improvement after adjusting the color  
![Compares](/img/SETI Code Challenge/Compare2.jpg "Impossible to discern"){: .center-block :}  

I had to resort to some creative visualizations but the low SNR and higher number of classes proved to be a challenge. Here are some artistic results, each color represents a type of signal: [Code](https://github.com/probabilityfilter/ML-SETI-IBM/blob/master/notebooks/Arun_nonNN%2BPrimary_testset_preview.ipynb).
![DSP1](/img/SETI Code Challenge/PSmall_MenMedianRatio.JPG "Fountain :-)"){: .center-block :}  
![DSP2](/img/SETI Code Challenge/PSmall_pVal.JPG "Not very helpful"){: .center-block :}  
![DSP3](/img/SETI Code Challenge/PSmall_pVal_slopeLinearFit.JPG "Buttetfly from top"){: .center-block :}  
![DSP4](/img/SETI Code Challenge/PSmall_StdDevTime.JPG "Taking off"){: .center-block :}  

## Future Work

The Code Challenge that followed the Hackathon focused on bringing the powers of Supervised Learning to the task of classifying the signals into seven categories. Although the winning team attained a 95% signal classification accuracy, the Universe does not limit itself to just seven categories. Hence, I firmly believe that this is an appropriate problem for Unsupervised Learning algorithms which would not only classify previously unseen yet interesting signals but also be able to detect different types of signals within a single observation. Such research will also contribute to the pursuit of true AI (Artificial Intelligence) which does not seem to be achievable by simple variations of Deep Learning and Supervised Learning algorithms.