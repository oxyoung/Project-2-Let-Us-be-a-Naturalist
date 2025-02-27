# iNaturalist 2019 Fine-Grained Classification Competition
## Introduction
This repository is investigating the fine-grained image classification for iNaturalist 2019 FGVC6 at CVPR 2019.

The codes is able to build three CNN models, including InceptionV3, Xception and InceptionResNetV2 using Keras and train them according to iNaturalist 2019 dataset. Additionally, the required submission CSV file can also be generated according to the fine-trained model. 

## Note
1. Before running the code, please change all paths in **iNaturalist_main.py** and **./GeneralTools/misc_fun.py** according to your folder structure.

2. In training mode, users can choose to train the three model from scratch or load pre-trained model to continue training. The base weights for InceptionV3, Xception and InceptionResNetV2 are pre-trained on ImageNet.

3. If users want to continue to train the model or get corresbonding CSV file, please make sure the desired weight is put in the ckpt_folder, whose path is define in Assignment2_main.py **ckpt_folder = FLAGS.DEFAULT_OUT + 'trial_{}_{}_{}/'.format(image_size, target_size, drop_out)**.
