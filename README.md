# Cellpose Hackathon on February 13, 2023
Template notebook &amp; instructions to interactively train 3D cellpose models

[Intro slides are available here](https://docs.google.com/presentation/d/1IIxVK1mCvI2eoq3HV5Ro3bzcJVO1_cM6LRWOqEPGiwY/edit#slide=id.g2072dd8912e_0_238)

Follow the instructions in the `Cellpose_3D_training_workflow` notebook.



### Installing Cellpose on M1 Macs with GPU usage
Install the dev branch from Peter Sobolewski https://github.com/psobolewskiPhD/cellpose/tree/feature/add_MPS_device 

This works for me
```
conda config --add channels conda-forge
conda config --set channel_priority strict
conda create --name cellpose-dev python=3.9 -y
conda activate cellpose-dev
conda install napari
git clone https://github.com/psobolewskiPhD/cellpose.git
cd cellpose 
git fetch
git switch feature/add_MPS_device 
conda install imagecodecs -y
conda install pyqtgraph -y
pip install -e .
```



