# cellpose-hackaton-liberalilab
Template notebook &amp; instructions to interactively train 3D cellpose models

Follow the instructions in the `Cellpose_3D_training_workflow` notebook.



### Installing Cellpose on M1 Macs with GPU usage
Install the dev branch from Peter Sobolewski https://github.com/psobolewskiPhD/cellpose/tree/feature/add_MPS_device 

This works for me
conda create --name cellpose-dev python=3.9 -y
conda activate cellpose-dev
conda install napari
git clone https://github.com/psobolewskiPhD/cellpose.git
cd cellpose 
git fetch
git switch feature/add_MPS_device 
conda install imagecodecs -y
pip install -e .



