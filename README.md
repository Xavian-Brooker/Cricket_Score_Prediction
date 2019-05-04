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
- Look Back = 1
- Epochs = 5
- Batch Size = 30
### Decision_Prediction_Models
This notebook consists a Machine Learning algorithm to predict the probability of a team to either win or loose the match depending on the given input data such as the organiser team, ground, which team is playing the first and second innings etc. 

The Neural Network Trained well and with nearly 71% accuracy, its able to predict the outcome of the match by just the match's metadata.

Other models were also used for the same but didn't prove to be satisfactory - 

These were the model accuracies after training - 
- XGBoost : 61 %
- Logistic Regression - 53 %
- Support Vector Machines - 52%

