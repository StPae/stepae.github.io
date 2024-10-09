# stepae.github.io

## Install napari with noise 2 void (n2v) on windows (09.Oct.2024) in anaconda/miniconda

Accoirding to https://juglab.github.io/napari-n2v/installation.html<br>
`conda create -n napari-n2v python=3.9`<br>
`conda activate napari-n2v`<br>
`conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0`<br>
`python -m pip install "tensorflow<2.11"`<br>
`pip install "napari[all]" napari-n2v`<br>
test tensorflow using:<br>
`python -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"`<br>
Output should look something like:<br>
`[PhysicalDevice(name='/physical_device:GPU:0', device_type='GPU')]`<br>
run napari using<br>
`napari`
