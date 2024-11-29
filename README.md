<h1 align="center" style="color:#6C63FF; font-family:Arial;">
  🚀 MVCTrack: Boosting 3D Point Cloud Tracking 🚀
</h1>


**Authors**: Zhaofeng Hu<sup>1†</sup>, Sifan Zhou<sup>2†*</sup>, Shibo Zhao<sup>3</sup>, Zhihang Yuan<sup>4</sup>  
<sup>1</sup>Stony Brook University, <sup>2</sup>Southeast University, <sup>3</sup>Carnegie Mellon University, <sup>4</sup>Houmo AI  
† Equal contribution, *Corresponding author  

---

## Overview
<p style="background:#F7F7F7; padding:10px; border-radius:5px;">
MVCTrack is an enhanced framework for **3D single object tracking (3D SOT)** in point clouds, designed to address the limitations of sparse and incomplete LiDAR data. Our approach introduces a **Multimodal-guided Virtual Cues Projection (MVCP)** scheme to enrich sparse point clouds by integrating RGB camera data, significantly improving tracking performance, particularly in scenarios with distant or small objects.
</p>

![framework](https://github.com/WindyHu001/MVCtrack/blob/master/figures/backbone.png)

This repository provides the code for **MVCTrack**, which achieves state-of-the-art performance on the **NuScenes dataset**.

---
## Video
 - Please watch this video to know more about our work.
[![Watch the video](https://img.youtube.com/vi/c-OPJ0PvvbA/maxresdefault.jpg)](https://www.youtube.com/watch?v=c-OPJ0PvvbA)


## Key Features
### **Multimodal-guided Virtual Cues Projection (MVCP)**
A novel, lightweight, and plug-and-play scheme that:
1. Utilizes **2D object detection** to generate virtual cues from RGB images.
2. Projects dense 2D semantic information into **3D space** to balance point cloud density.
3. Enhances the **sparsity and completeness** of point clouds.

### **MVCTrack Framework**
An end-to-end 3D SOT tracker that:
1. Seamlessly integrates the MVCP scheme to improve tracking accuracy.
2. Effectively balances point density distribution across different distances.
3. Achieves competitive performance with minimal computational overhead.

### **State-of-the-Art Performance**
- Evaluated on the large-scale **NuScenes dataset**.
- Significantly surpasses existing multi-modal 3D trackers.
- Demonstrates exceptional performance in sparse and occluded scenarios.

![framework](https://github.com/WindyHu001/MVCtrack/blob/master/figures/nuScenes.png)


---

## Acknowledgement

Our implementation is based on [Open3DSOT](https://github.com/Ghostish/Open3DSOT), [BEVTrack](https://github.com/xmm-prio/BEVTrack), [P2P](https://github.com/haooozi/P2P), [MMDetection3D](https://github.com/open-mmlab/mmdetection3d), and [MVP](https://github.com/tianweiy/MVP). Thanks for the great open-source work!

## Citation
If any parts of our paper and code help your research, please consider citing us and giving a star to our repository.


