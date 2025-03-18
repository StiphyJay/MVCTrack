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

<!---
### KITTI
 - Download the data for `velodyne`, `calib`, and `label_02` from KITTI Tracking.
 - Unzip the downloaded files.
 - Put the unzipped files under the same folder as follows:


```
[Parent Folder]   
    --> [calib]
    
        --> {0000-0020}.txt
        
    --> [label_02]
    
        --> {0000-0020}.txt
        
    --> [velodyne]
    
        --> [0000-0020] folders with velodynes .bin files
```
---

### Waymo Open Dataset
 - We follow the benchmark created by LiDAR-SOT based on the Waymo Open Dataset. You can download and process the Waymo dataset as guided by LiDAR-SOT, and use our code to test model performance on this benchmark.
The following processing results are necessary:

```
[waymo_sot]
     [benchmark]
         [validation]
             [vehicle]
                 bench_list.json
                 easy.json
                 medium.json
                 hard.json
             [pedestrian]
                 bench_list.json
                 easy.json
                 medium.json
                 hard.json
     [pc]
         [raw_pc]
             Here are some segment.npz files containing raw point cloud data
     [gt_info]
         Here are some segment.npz files containing tracklet and bbox data
```
-->
