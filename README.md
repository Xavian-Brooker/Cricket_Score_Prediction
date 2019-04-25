# Cricket_Score_Prediction

## INTRODUCTION
This repository contains a set of different RNN algorithms mainly **single and multi-vairiate LSTMs** to predict cricket scores. All the different algorithms are sorted into different subfolders along with:
- The training notebook (`.ipynb`)
- Weights (`.h5`)
- Dataset Used (`.csv`)
- Loss curve (`.jpg`)

## Algorithms
### Vanilla_RNN_v1
This algorithm consists of a single `LSTM` & a `Dense` layer with a single input feature that is the total runs at the current timestep and predicts the total runs at the next timestep.   
