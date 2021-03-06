# Face Alignment


## Description
This repository contains a Jupyter notebook which tests and compares 3 simple face alignment Machine Learning algorithms.

The dataset used in these experiments consists of images of families collected from the web. Since most of these images are copyrighted, the dataset is going to remain private.

The face detectors used in these experiments are:
* **OpenCV Haar cascade Eyes Detector**
* **Dlib 5-point Face Landmarking Detector**
* **YOLOv5Face 5 Facial Keypoints Detector**

The detectors are evaluated based on
* **Total alignment time**
* **Total number of faces aligned**



## Instructions
### Setup and execution on Ubuntu 20.04

1. Install necessary tools
```console
sudo apt-get -y install git wget zip bzip2
```

2. Fetch repository
```console
git clone https://github.com/nbishdev/simple_face_alignment.git
```

3. Install Miniconda
```console
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
source ~/.bashrc
```

4. Create a virtual environment for the notebook experiments
```console
conda create -n face
```

5. Install all the necessary packages
```console
conda install -n face -c conda-forge dlib
conda activate face
pip install -r simple_face_alignment/requirements.txt
```

6. Execute JupyterLab
```console
jupyter-lab --notebook-dir=simple_face_alignment
```
