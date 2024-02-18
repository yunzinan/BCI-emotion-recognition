# BCI-emotion-recognition
A fundamental exploration about EEG-BCI emotion recognition using the dataset from kaggle.

# Dataset
- Emotion Recognition Dataset on Kaggle: https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-feeling-emotions

- SEED: https://bcmi.sjtu.edu.cn/home/seed/seed.html

# Models 

- GRU
- LSTM
- Transformer: EEG-conformer: https://github.com/eeyhsong/EEG-Conformer

# Results

| model     | subject-dependent | subject-independent |
| --------- | ----------------- | ------------------- |
| GRU       | 0.9934            | 0.9737              |
| Conformer | 0.9974            | 0.9998              |

note: 

● subject-dependent: train & test on subject1

● subject-independent: train & test on a mixed dataset of all subjects

