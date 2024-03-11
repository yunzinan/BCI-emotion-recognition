# BCI-emotion-recognition
A fundamental exploration about EEG-BCI emotion recognition using the SEED dataset & dataset from kaggle.

# Dataset

- Emotion Recognition Dataset on Kaggle: https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-feeling-emotions

- SEED: https://bcmi.sjtu.edu.cn/home/seed/seed.html

# Models 

- GRU
- LSTM
- Transformer: EEG-conformer: https://github.com/eeyhsong/EEG-Conformer

# Results
<!-- 
| model     | subject-dependent | subject-independent |
| --------- | ----------------- | ------------------- |
| GRU       | 0.9934            | 0.9737              |
| LSTM      | 0.9657            | 0.9665              |
| Conformer | 0.9974            | 0.9998              | -->

Thanks for [AllGGI](https://github.com/AllGGI) to point out the [bug](https://github.com/yunzinan/BCI-emotion-recognition/issues/1) in my original impl.. I fixed the bug and re-do the experiments(only the subject-dependent ones). Sadly, the results were pretty bad. Therefore, I suppose this work isn't a successful practice, and hidden bugs may remain in the codings.

note: 

- Models are trained & tested on SEED dataset

● subject-dependent: train & test on subject1, 100 epochs

● subject-independent: train & test on a mixed dataset of all subjects, 50 epochs


# File Descriptions

```
.
├── base.py # the base helper functions
├── conformer.ipynb # conformer on SEED 
├── conformer-sub1.ipynb # conformer on SEED, subject1
├── eegconformer.py # the implementation of conformer
├── emotions.csv # the Kaggle dataset
├── gru.ipynb # gru on Kaggle dataset
├── gru-seed.ipynb # GRU on SEED 
├── gru-sub1.ipynb # GRU on SEED, subject1
├── LSTM-seed.ipynb # LSTM on SEED
├── LSTM-sub1.ipynb # LSTM on SEED, subject1
├── model_gru # best model state dict 
├── model_LSTM # best model state dict
├── model_transformer # best model state dict
├── Preprocessed_EEG # the SEED dataset 
└── README.md
```
