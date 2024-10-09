# stepae.github.io

## Install napari with noise 2 void (n2v) on windows (09.Oct.2024) in anaconda/miniconda

Accoirding to https://juglab.github.io/napari-n2v/installation.html
`conda create -n napari-n2v python=3.9`
`conda activate napari-n2v`
`conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0`
`python -m pip install "tensorflow<2.11"`
`pip install "napari[all]" napari-n2v`
test tensorflow using:
`python -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"`
Output should look something like:
`[PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')]`
run napari using
`napari`
