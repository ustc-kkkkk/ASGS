# ASGS: Adaptive Sampling Gaussian Splatting for Autonomous Driving Scenes


### Installation
#### Clone this repository

```
git clone https://github.com/ustc-kkkkk/ASGS.git
```


#### Set up the python environment

```
# Set conda environment
conda create -n ASGS python=3.8
conda activate ASGS

# Install torch (corresponding to your CUDA version)
pip install torch==1.13.1+cu116 torchvision==0.14.1+cu116 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu116

# Install requirements
pip install -r requirements.txt

# Install submodules
pip install ./submodules/diff-gaussian-rasterization
pip install ./submodules/simple-knn
pip install ./submodules/simple-waymo-open-dataset-reader
python script/test_gaussian_rasterization.py
```


#### Prepare Waymo Open Dataset.
Download the training and validation set of [Waymo Open Dataset](https://console.cloud.google.com/storage/browser/waymo_open_dataset_v_1_4_1/individual_files?pageState=(%22StorageObjectListTable%22:(%22f%22:%22%255B%255D%22))). 

### 🛠️ Pipeline
<div align="center">
  <img src="assets/pipeline.png"/>
</div><br/>
