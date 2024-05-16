该仓库旨在整理 Next-Step Location Prediction 任务的相关文献，供给自己科研学习使用

This repo aims to organize related works for the topic "Next-Step Location Prediction" for scientist research.

The repo will divide these works into three parts:

- classic assumptions/ theory/ findings
- topics (related data)
- models (mainly based on neural networks)

### Assumptions/ Theory/ Findings

| Paper                                                                                   | Journal & Year | Findings                                                | Main Method |
| --------------------------------------------------------------------------------------- | -------------- | ------------------------------------------------------- | ----------- |
| [Limits of Predictability in Human Mobility](./findings/limits_entropy/Limits_Pred.pdf) | Science, 2010  | The predictability of the general public is around 93%. | Entorpy / Π |

### Topics

| Paper                                                                                                                                                                                                   | Journal & Year                                               | Topic                     | Findings                                                  | Main Method                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ | ------------------------- | --------------------------------------------------------- | ------------------------------------------------------------------- |
| [Trajectory Data Mining: An overview](./topics/trajectory_data_mining/f89e6316-414a-4c04-a94e-221539f225d9_Trajectory_Data_Mining_An_overview.pdf)                                                      | ACM Transactions on Intelligent Systems and Technology, 2015 | Trajectory Data           | Overview on trajectory data                               | Introduction and Main methods on different trajectory-related tasks |
| [Understanding the movement predictability of international travelers using a nationwide mobile phone dataset collected in South Korea](./topics/traveler_predictability/travelers’_predictability.pdf) | CEUS, 2022                                                   | Travelers' predictability | Despite travelling, tourist movement is still predictable | 1-order Markov Chain / LSTM                                         |

### Models

| Paper                                                                                                                                       | Journal & Year | Findings | Innovation        | Main Method |
| ------------------------------------------------------------------------------------------------------------------------------------------- | -------------- | -------- | ----------------- | ----------- |
| [Context-aware multi-head self-attentional neural network model for next location prediction](./models/context-aware_mul_attent//readme.md) | TRC, 2023      | -        | 1. Adding user ID | -           |
