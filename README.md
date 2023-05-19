# Project_VIBE: 
Based on Video Inference for Human Body Pose and Shape Estimation [CVPR-2020]

## Features

_**V**ideo **I**nference for **B**ody Pose and Shape **E**stimation_ (VIBE) is a video pose and shape estimation method.
Please Not: This repo is slightly modified version of the original repo (https://github.com/mkocabas/VIBE.git)


This is repository for experimenting with the demo of the origibal VIBE repository.
This version is basically modified to run on Mask-RCNN (no YOLO):

- has modified demo file
- updated to run with pretrained ResNet152 as feature extractor
- option to switch models between VIBE and baseline HMR while running demo.py using the -- model HMR

## Getting Started

Clone the repo:
```bash
git clone  https://github.com/ShrikanthX/Project_VIBE.git
```

Create a conda environment and activate it
```bash
conda create -n $CONDA_ENV_NAME python=3.7
```

```bash
# activate conda environement
conda activate $CONDA_ENV_NAME
```

```bash
# install torch and numpy
pip install numpy torch torchvision
```

## Running the Demo

Open the jupyter notebook file and run the cells in it. It has the options to run requirement files in it.

Then, running the demo is as simple as:

```bash
# Run on a local video
python demo.py --vid_file sample_video.mp4 --output_folder output/ --model HMR

```
