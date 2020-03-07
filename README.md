# Automated-Seismic-Phase-Recognition-Using-Neural-Networks
This repository contains both the .ipynb file containing the generated graphs and code, as well as the .py file conatinaing only the code. The code is written in Python 3.x, and it's dependencies are: Tensorflow, Keras, Numpy, Matplotlib, and h5py.
To view the file in Google Colaboratory, please download the .zip file using the clone or download button in the top right of this page, extract it to a location on your device, and then upload the .ipynb file to Google Colaboratory to view the code along with the graphs. A link to Google Colaboratory can be found here: https://colab.research.google.com/notebooks/intro.ipynb. To upload the downloaded .ipynb file for viewing, click on the 'File' button in the top left, select 'upload notebook', and then 'Upload' followed by selecting the file.

## Running the script
### Google Colaboratory Tensor Processing Unit (TPU) Runtimes
The code was written in Google Colaboratory, and it was trained using the Tensor-Processing-Unit, or TPU so that RAM and disk space requirements were not exceeded in the environment. The dataset file is downloaded using the shell command "wget" in the first cell and is saved in the hosted runtime in Colaboratory to prevent the large dataset file of approximately 21 GB taking up lots of disk space in a local machine. Using the TPU hosted runtime in Colaboratory is highly recommended, since it reduces computation time signifigantly and does not run into RAM restrictions. To change the runtime to the TPU, click on 'runtime' in the top left and select 'Change runtime type' to change the 'Hardware Accelerator' to 'TPU'.

### Google Colaboratory GPU and Standard Runtimes
If the TPU runtime is not responding or not available, then the GPU or standard runtime can be used with some changes. In code cell 9 in the .ipynb file, there is a variable called "extracted_data", which defines the subset of the dataset which is extracted and used. Changing the "0.1" which signifies 10% of the dataset to "0.05", signifying 5% of the data, will allow the data to be run in hosted runtimes beside the TPU environment in Google Colaboratory.

### Local Runtimes
If you wish to run the code in a local environment, please be advised that the 21 GB dataset file which downloads using the wget tool is quite large and may take several hours to download. Alternatively, there is a link to downloading the dataset here:
https://service.scedc.caltech.edu/ftp/ross_etal_2018_bssa/scsn_ps_2000_2017_shuf.hdf5

In addition, in the third code cell please change the local path of the file to wherever the file is stored on your local machine to ensure that the code runs.
