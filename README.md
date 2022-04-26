# 4995-DL-Project
Nathaniel Thomas Jenkins (ntj2109)

Nikhil Nanda (nn2522)

Padmanabhan Krishnamurthy (pk2705)

### Submodule for Rain-Removal-Specific Data Augmentation
[VRGNet](https://github.com/hongwang01/VRGNet/tree/834c2c64be363797fe3741f4f8e8d17657f9b614)

### Data
* [Data_Augmentation_Restormer.ipynb](Data_Augmentation_Restormer.ipynb)
* [Data_Augmentation_Restormer_Crop_Rain_Streak.ipynb](Data_Augmentation_Restormer_Crop_Rain_Streak.ipynb)
* [Data_Augmentation_Restormer_ISR.ipynb](Data_Augmentation_Restormer_ISR.ipynb)

### Models
https://drive.google.com/drive/folders/1ajTTQ6uQwl_rcnim7hANO49yO-ERFx7l?usp=sharing

### Instructions
Clone this repository and download the desired model configuration's weights from the above link

`cd DAD`

`python eval_derain.py --dataset rain100h --ckptdir <folder name of downloaded checkpoint> --net_G unet_512 --in_size 512 --save_output`

For example, to run evaluation using configuration 1.(b)'s weights (with rain streak maps supplied during training), run

`python eval_derain.py --dataset rain100h --ckptdir 1_b/rainstreak --net_G unet_512 --in_size 512 --save_output`
