# Cricket_Score_Prediction

## INTRODUCTION
This repository contains a set of different RNN algorithms mainly **single and multi-vairiate LSTMs** to predict cricket scores. All the different algorithms are sorted into different subfolders along with:
- The training notebook (`.ipynb`)
- Weights (`.h5`)
- Dataset Used (`.csv`)
- Loss curve (`.jpg`)

## ALGORITHMS
### Vanilla_RNN_v1
This algorithm consists of a single `LSTM` & a `Dense` layer with a single input feature that is the total runs at the current timestep and predicts the total runs at the next timestep. It was trained on 197944 training samples and 97495 validation samples.

![Training and Test Loss](https://github.com/Xavian-Brooker/Cricket_Score_Prediction/blob/master/vanilla_RNNs/v1/loss_comparision.png)

**Hyper-Parameters**
1. Look Back = 1
2. Epochs = 5
3. Batch Size = 30

