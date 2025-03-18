## Dataset Preparation
At present, we only support the implementation in nuScenes dataset due to the limited samples in KITTI.

### NuScenes
 - Download the dataset from the download page.
 - Extract the downloaded files and ensure the following structure:
```
[Parent Folder]
  samples	-	Sensor data for keyframes.
  sweeps	-	Sensor data for intermediate frames.
  maps	        -	Folder for all map files: rasterized .png images and vectorized .json files.
  v1.0-*	-	JSON tables that include all the meta data and annotations. Each split (trainval, test, mini) is provided in a separate folder.
Note: We use the `train_track` split to train our model and test it with the `val` split. Both splits are officially provided by NuScenes. During testing, we ignore the sequences where there is no point in the first given bbox.
```
---
