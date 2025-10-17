## Virtual_Cues
- You can choose a segmentation model, such as CenterNet2, and generate corresponding virtual clues using the following command. Here, we follow the centernet2, use this [config](https://github.com/xingyizhou/CenterNet2/blob/master/configs/nuImages_CenterNet2_DLA_640_8x.yaml) and the corresponding [model weights](https://drive.google.com/file/d/1v43riMzWx9Bydha4u3z69nLrMrhtlNBR/view?usp=sharing).

Download the model weights in here: [model weights](https://drive.google.com/file/d/1v43riMzWx9Bydha4u3z69nLrMrhtlNBR/view?usp=sharing)
Run the following command:
```
# nuScenes
python virtual_cues/virtual_gen.py --info_path nuScenes_DATA_ROOT/infos_train_10sweeps_withvelo_filter_True.pkl  MODEL.WEIGHTS centernet2_checkpoint.pth
```
Note: The file of nuScenes_DATA_ROOT/infos_train_10sweeps_withvelo_filter_True.pkl is generated follows CenterPoint: https://github.com/tianweiy/CenterPoint/blob/master/docs/NUSC.md
