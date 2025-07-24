<div align="center">

<h1> Attack to Defense: Adversarial Agents for Point Prompt Optimization Empowering Segment Anything </h1>

[Xueyu Liu]([https://scholar.google.com/citations?user=9JcQ2hwAAAAJ&hl=en](https://scholar.google.com.hk/citations?user=jeatLqIAAAAJ&hl=zh-CN))<sup>1</sup>, &nbsp; 
Guangze Shi<sup>1</sup>, &nbsp; 
Rui Wang<sup>2</sup>, &nbsp; 
Yexin Lai<sup>1</sup>, &nbsp; 
Jianan Zhang<sup>1</sup>, &nbsp; 
Yonfei Wu<sup>1*</sup>, &nbsp;


<sup>1</sup>[Taiyuan University of Technology](https://www.tyut.edu.cn/), &nbsp;
<sup>2</sup>[University of Science and Technology of China](https://www.ustc.edu.cn/), &nbsp;

</div>

## Overview
<p align="center">
<img width="800" alt="eg" src="img/Display.png">
</p>

##  Description
\begin{abstract}
	Prompt quality plays a critical role in the Segment Anything Model (SAM), yet existing methods rely heavily on heuristic or manual prompt design, limiting scalability and generalization. In this paper, we propose an adversarial reinforcement learning framework for automatic prompt optimization via competitive interaction between two agents. Specifically, we construct a task-agnostic prompt environment by modeling image patches as nodes in a dual-space graph, where edges encode physical and semantic distances. Within this environment, an attacker agent learns to activate a subset of prompts that maximally degrade SAM’s segmentation performance, while a defender agent learns to remove disruptive prompts and restore accuracy. Both agents are trained with Deep Q-Networks (DQNs) using segmentation quality variation as reward. During inference, only the defender is used to refine arbitrary coarse prompt sets, enabling improved segmentation across diverse tasks without retraining. Extensive experiments demonstrate that our method consistently enhances SAM’s robustness and generalization, establishing a flexible and plug-and-play framework for prompt-based segmentation.
 
## Setup 
- Cuda 12.0
- Python 3.9.18
- PyTorch 2.0.0

## TODO
- [ ] Release code


## Acknowledgement
Thanks [DINOv2](https://github.com/facebookresearch/dinov2), [SAM](https://github.com/facebookresearch/segment-anything), [GBMSeg](https://github.com/SnowRain510/GBMSeg). for serving as building blocks of SAT.
