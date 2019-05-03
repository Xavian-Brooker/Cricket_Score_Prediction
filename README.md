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
### Decision_Prediction_Models_v1
This notebook consists a set of Machine Learning algorithm to predict the probability of a team to either win or loose the match depending on the given input data such as the organiser team, ground, which team is playing the first and second innings etc. 

The models that were used were - 
- **XGBoost** : XGBoost is an optimized distributed gradient boosting library which is used to create an alorithm similar to parallel decision trees.
- **Logistic Regression** : Logistic Regression is a predictive modelling algorithm that is used when the Y variable is binary categorical, i.e 0 or 1
- **Support Vector Machine** : Support Vecotr Machines are supervised learning models with associated learning algorithms that analyze data used for classification and regression analysis.
- **Neural Network** : Complex Deep Learning Models that are artificial mapping of Biological Neural Architechture that are most commonly used for big and complex problems.

These were the model accuracies after training - 
- XGBoost : 61 %
- Logistic Regression - 53 %
- Neural Network - 51%
- Support Vector Machines - 52%

The accuracies of the models were unsatisfactory.
