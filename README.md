# Reference Twice: A Simple and Unified Baseline for Few-Shot Instance Segmentation

Yue Han, [Jiangning Zhang](https://zhangzjn.github.io/), [Zhucun Xue](http://www.captain-whu.com/xuezhucun.html), [Chao Xu](https://scholar.google.com/citations?hl=zh-CN&user=zlq2S_0AAAAJ), [Xintian Shen](https://april.zju.edu.cn/team/xintian-shen/), [Yabiao Wang](https://scholar.google.com.hk/citations?hl=zh-CN&user=xiK4nFUAAAAJ), [Chengjie Wang](https://scholar.google.com/citations?hl=zh-CN&user=fqte5H4AAAAJ), [Yong Liu](https://april.zju.edu.cn/our-team/), [Xiangtai Li](https://lxtgh.github.io/)

## Abstract
**Few Shot Instance Segmentation (FSIS)** requires models to detect and segment novel classes with limited several support examples. In this work, we explore a simple yet unified solution for FSIS as well as its incremental variants, and introduce a new framework named **Ref**erence **T**wice (RefT) to fully explore the relationship between support/query features based on a Transformer-like framework. Our key insights are two folds: Firstly, with the aid of support masks, we can generate dynamic class centers more appropriately to re-weight query features. Secondly, we find that support object queries have already encoded key factors after base training. In this way, the query features can be **enhanced twice** from two aspects, i.e., feature-level and instance-level. In particular, we firstly design a mask-based dynamic weighting module to enhance support features and then propose to link object queries for better calibration via cross-attention. After the above steps, the novel classes can be improved significantly over our strong baseline. Additionally, our new framework can be easily extended to incremental FSIS with minor modification. When benchmarking results on the COCO dataset for FSIS, gFSIS, and iFSIS settings, our method achieves a competitive performance compared to existing approaches across different shots, e.g., we boost nAP by noticeable +8.2 $\uparrow$ /+9.4 $\uparrow$ over the current state-of-the-art FSIS method for 10/30-shot. We further demonstrate the superiority of our approach on Few Shot Object Detection.


![Figure](./fig/teaser.png)

## Results
#### gFSIS 
![Figure](./fig/gfsis_res.png)
#### FSIS and iFSIS  results
![Figure](./fig/fsis_res.png)


