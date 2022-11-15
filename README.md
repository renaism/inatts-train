# inatts-train

## Setup VM

1. Install nVidia driver
```
sudo /opt/deeplearning/install-driver.sh
```
Check if cuda is installed
```
sudo nvidia-smi
```
```
torch.cuda.is_available
```

2. Install dependencies
```
sudo apt-get install sox libsndfile1 ffmpeg
```
```
pip install wget unidecode
```
```
python -m pip install git+https://github.com/NVIDIA/NeMo.git@v1.4.0#egg=nemo_toolkit[tts]
```

3. Run training

Example:
```
python tacotron2.py \ 
train_dataset=data/INATTS_TelU_1k_train.json \ 
validation_datasets=data/INATTS_TelU_1k_val.json \ 
batch_size=24 \ 
trainer.max_epochs=2 \ 
trainer.check_val_every_n_epoch=1
```
