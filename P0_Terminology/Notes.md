1. Differences between one stage object detector and two stages object detector?
  
  Answer:
    
    There are mainly two types of state-of-the-art object detectors. On one hand, we have two-stage detectors, such as Faster R-CNN (Region-based Convolutional Neural Networks) or Mask R-CNN, that (i) use a Region Proposal Network to generate regions of interests in the first stage and (ii) send the region proposals down the pipeline for object classification and bounding-box regression. Such models reach the highest accuracy rates, but are typically slower. On the other hand, we have single-stage detectors, such as YOLO (You Only Look Once) and SSD (Singe Shot MultiBox Detector), that treat object detection as a simple regression problem by taking an input image and learning the class probabilities and bounding box coordinates. Such models reach lower accuracy rates, but are much faster than two-stage object detectors. (from https://arxiv.org/abs/1803.08707 )

    And see for example this figure https://www.researchgate.net/figure/Two-stage-vs-Proposed-a-The-two-stage-approach-separates-the-detection-and-pose_fig1_308320592

    https://www.youtube.com/watch?v=nDPWywWRIRo&ab_channel=StanfordUniversitySchoolofEngineering

2. Loss function

   https://ml-cheatsheet.readthedocs.io/en/latest/loss_functions.html#cross-entropy
   
   cross entroy 
