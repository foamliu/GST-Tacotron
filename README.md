# Tacotron 2

A PyTorch implementation of [Style Tokens: Unsupervised Style Modeling, Control and Transfer in End-to-End Speech Synthesis](https://arxiv.org/abs/1803.09017).

## Dataset

[THCHS-30 Dataset](http://www.openslr.org/18/).

## Dependency

- Python 3.5.2
- PyTorch 1.0.0

## Usage
### Data Pre-processing
Extract data_thchs30.tgz and generate features:
```bash
$ python extract.py
$ python pre_process.py
```

### Train
```bash
$ python train.py
```

If you want to visualize during training, run in your terminal:
```bash
$ tensorboard --logdir runs
```

### Demo
Generate mel-spectrogram for text "Waveglow is really awesome!"
```bash
$ python demo.py
```
![image](https://github.com/foamliu/Tacotron2-CN/raw/master/images/mel_spec.jpg)
