# Generative-Adversarial-Federated-Model
This repository contains the implementation of the Generative Adversarial Federated Model (GAFM). The GAFM framework is shown in the following figure.

![截屏2023-05-15 12 22 57](https://github.com/hyj12345/Generative-Adversarial-Federated-Model/assets/49636371/f616c65a-2e44-4029-a425-9236152ed725)


## Requirements ##
The following packages are required to run the code:

- PyTorch (>=1.8.1)
- torchvision (>=0.9.1)
- numpy (>=1.19.5)
- pandas (>=1.2.4)
- sklearn (>=0.24.2)
- matplotlib (>=3.3.4)

## Data ##

We evaluate GAFM on four publicly available datasets, which can be obtained through the following sources:

- Spabmase: Download from [Spambase](https://archive.ics.uci.edu/ml/datasets/spambase).
- IMDB: Import the data using the following code (details can be found in `GAFM_IMDB/train.py`): `from keras.datasets import imdb` and the `imdb.load_data()` function.  
- Criteo: Download from [Criteo](https://www.kaggle.com/c/criteo-display-ad-challenge).
- ISIC: Download from [ISIC](https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic).

## Usage ##

To train the GAFM model, run `train.py` with the following command:

```linux
sbatch GAFM.sh
```

## Results ##

The model's training progress can be tracked by examining the logs generated during training. Several examples of GAFM training logs are provided in the `training_logs_example.txt`. For more comprehensive results, please refer to the paper.
