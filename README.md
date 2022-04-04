# Salient objects in clutter (TPAMI2022-Minor)

> Authors:
> [Deng-Ping Fan](https://dengpingfan.github.io/), 
> [Jing Zhang](https://jingzhang617.github.io/), 
> [Gang Xu](https://github.com/CS-GangXu/), 
> [Ming-Ming Cheng](https://mmcheng.net/), 
> [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=zh-CN&oi=sra).

## 1. Preface

- This repository provides benchamrk for "_**Salient objects in clutter**_". 
([paper](https://arxiv.org/abs/2105.03053) | [中文版](https://dengpingfan.github.io/papers/[2022][TPAMI]SOC_Chinese.pdf))

- If you have any questions about our paper, feel free to contact me. And if you are using SOCbenchamrk results 
or evaluation toolbox for your research, please cite this paper ([BibTeX](#4-citation)).

## 2. Scope
Salient object detection originated from the task of fixation prediction (FP), switching attention regions for accurate object-level regions. 
Current algorithms have been developed for 2D images of limited resolution (width or height $<$ 500 pixels), high-resolution (i.e., 1080p, 4K) and 
even remote sensing data. According to the supervision strategy, there are five types of SOD models: fully supervised, 
semi-supervised, weakly supervised, unsupervised, and self-supervised.

Recently, several interesting extensions of SOD have also been introduced, such as salient instance detection (SID), 
salient object subitizing (SOS), and saliency ranking. 
A taxonomy of the saliency detection task is shown below. 
Different from previous SOD reviews, we mainly focus on 2D salient object detection in a fully supervised manner. We highlight the scope of this study in gray.
For other closely related 3D/4D SOD tasks, we refer readers to
recent survey and benchmarking works such as RGB-D SOD, Event-RGB SOD [(ERSOD)](https://github.com/jxr326/ERSOD-Net), Light Field SOD,  
Co-SOD, 360° Video SOD, and Video SOD.
 
![avatar](Imgs/Scope.png)
