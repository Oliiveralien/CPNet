# CPNet
CPNet (CVPR'23)

* This repo will release an official **PaddlePaddle** implementation for paper: Context-aware Pretraining for Efficient Blind Image Decomposition.

## Abstract
In this paper, we study Blind Image Decomposition (BID), which is to uniformly remove multiple types of degradation at once without foreknowing the noise type. There remain two practical challenges: 
(1) Existing methods typically require massive data supervision, making them infeasible to real-world scenarios.
(2) The conventional paradigm usually focuses on mining the abnormal pattern of a superimposed image to separate the noise, which de facto conflicts with the primary image restoration task. Therefore, such a pipeline compromises repairing efficiency and authenticity. 
In an attempt to solve the two challenges in one go, we propose an efficient and simplified paradigm, called Context-aware Pretraining (CP), with two pretext tasks: mixed image separation and masked image reconstruction.
Such a paradigm reduces the annotation demands and explicitly facilitates context-aware feature learning. 
Assuming the restoration process follows a structure-to-texture manner, we also introduce a Context-aware Pretrained network (CPNet).  
In particular, CPNet contains two transformer-based parallel encoders, one information fusion module, and one multi-head prediction module. The information fusion module explicitly utilizes the mutual correlation in the spatial-channel dimension, while the multi-head prediction module facilitates texture-guided appearance flow. 
Moreover, a new sampling loss along with an attribute label constraint is also deployed to make use of the spatial context, leading to high-fidelity image restoration. 
Extensive experiments on both real and synthetic benchmarks show that our method achieves competitive performance for various BID tasks.
