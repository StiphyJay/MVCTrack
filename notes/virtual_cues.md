## Virtual_Cues
- You can choose a segmentation model, such as CenterNet2, and generate corresponding virtual clues using the following command.

```
# nuScenes
python virtual_cues/virtual_gen.py --info_path nuScenes_DATA_ROOT/infos_train_10sweeps_withvelo_filter_True.pkl  MODEL.WEIGHTS your_segmentation_model.pth 
```
Note: The file of nuScenes_DATA_ROOT/infos_train_10sweeps_withvelo_filter_True.pkl is generated follows CenterPoint: https://github.com/tianweiy/CenterPoint/blob/master/docs/NUSC.md
