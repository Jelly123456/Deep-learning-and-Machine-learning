1. Differences between one stage object detector and two stages object detector?

    Answer:
    
    There are mainly two types of state-of-the-art object detectors. On one hand, we have two-stage detectors, such as Faster R-CNN (Region-based Convolutional Neural Networks) or Mask R-CNN, that (i) use a Region Proposal Network to generate regions of interests in the first stage and (ii) send the region proposals down the pipeline for object classification and bounding-box regression. Such models reach the highest accuracy rates, but are typically slower. On the other hand, we have single-stage detectors, such as YOLO (You Only Look Once) and SSD (Singe Shot MultiBox Detector), that treat object detection as a simple regression problem by taking an input image and learning the class probabilities and bounding box coordinates. Such models reach lower accuracy rates, but are much faster than two-stage object detectors. (from https://arxiv.org/abs/1803.08707 )

    And see for example this figure https://www.researchgate.net/figure/Two-stage-vs-Proposed-a-The-two-stage-approach-separates-the-detection-and-pose_fig1_308320592

    https://www.youtube.com/watch?v=nDPWywWRIRo&ab_channel=StanfordUniversitySchoolofEngineering

2. Loss function

    https://ml-cheatsheet.readthedocs.io/en/latest/loss_functions.html#cross-entropy
   
    cross entroy 

3. YoLo V5 model architecture

    https://medium.com/towards-artificial-intelligence/yolo-v5-explained-and-demystified-4e4719891d69
    
4. what is batch normalization, Cross-iteration batch normalization(CBN)?
    TBA
    
5. what is residual connections, Weighted Residual Connections(WRC), Cross-Stage-Partial-connections?
    TBA

6. what is Cross mini-Batch Normalization (CmBN), Self-adversarial-training (SAT)?
    TBA

7. what is Mish-activation?
    TBA
    
8. what is Mosaic data augmentation, DropBlock regularization, CIoU loss?

9. what is Path aggregation network(PAN), Convolutional block attention module(CBAM)

9. The most accurate modern neural networks do not operate in real time and require large number of GPUs for training with a large mini-batch-size. YoLo address such problems through creating a CNN that operates in real-time on a conventional GPU, and for which training requires only one conventional GPU.

10. what is model backbone, neck, head?
    Generally, object detector consists of four parts: a backbone that extracts features from input images, a neck attached to backbone that fuses multi-level features, a region proposal network which generates prediction candidates on extracted features, and a head for classification and localization.
    https://openaccess.thecvf.com/content_CVPR_2020/papers/Guo_Hit-Detector_Hierarchical_Trinity_Architecture_Search_for_Object_Detection_CVPR_2020_paper.pdf
    
