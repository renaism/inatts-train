# inatts-train

## Setup VM

1. Install nVidia driver
```
sudo /opt/deeplearning/install-driver.sh
```
```
sudo nvidia-smi
```

2. Install dependencies
```
sudo apt-get install sox libsndfile1 ffmpeg
```
```
pip install wget undecode
```
```
python -m pip install git+https://github.com/NVIDIA/NeMo.git@v1.4.0#egg=nemo_toolkit[tts]
Collecting nemo_toolkit[tts]
```
