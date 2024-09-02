# NYUv2 
This repo has a bunch of different tools and data to help you get benchmarking on NYUv2 quickly. It includes a script to download and extract data, extracted segmentation labels and a pytorch dataset class. 

Note that this repo only concerns itself with the fully labelled portion of the dataset. For the larger unlabelled version I would recommend checking out the tensorflow dataloader (https://www.tensorflow.org/datasets/catalog/nyu_depth_v2). 

## Downloading, extracting and pre-extracted data
This repository contains everything needed to download and extract data for the NYUv2 dataset in python. Using 'extract_nyu_v2.py' you can download and extract samples consisting of:
- RGB images
- Depth images
- Surface normals
- 13 class segmentation labels
- 40 class segmentation labels
The surface normals are downloaded from [here](https://dl.fbaipublicfiles.com/fair_self_supervision_benchmark/nyuv2_surfacenormal_metadata.zip) and everything else from [here](https://cs.nyu.edu/~fergus/datasets/nyu_depth_v2.html)
Additionally, you can avoid doing anything and simply download and use the pre-extracted segmentation labels found in:
- test_labels_13
- train_labels_13
- test_labels_40
- train_labels_40

## Pytorch
This repo also provides a script for a pytorch dataset class which lets you get up and running with the NYUv2 dataset very quickly ([Adapted from here](https://github.com/xapharius/pytorch-nyuv2)). Simply copy the code in 'torch_nyuv2.py', initialize the dataset using the class, give it to a dataloader and off you go!

## Thanks for checking out the repo
If you find this repo useful please consider giving it a star, so it can be more easily found by others. Also please feel free to propose changes and fixes or ask questions by creating an issue, include a @h-0-0 so that I'm notified. 

Finally, thank you very much to [ankurhanda](https://github.com/ankurhanda), [VainF](https://github.com/VainF) and [xapharius](https://github.com/xapharius) who's code I amalgamated to create this repo. 
