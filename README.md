# Whoop ML Project

This project was a personal exercise in implementing the EDA, preprocessing, training, and optimization steps of an ML pipeline or research project. The project scope was two-fold, including the training and evaluation of multiple models on each of a classification task and a regression task.

To learn more, please read through the [full report](./Reconstructing%20Secrets%20-%20Using%20Machine%20Learning%20Models%20to%20Approximate%20Proprietary%20Whoop%20Algorithms.pdf), from which the abstract is displayed below. For even more detail, I've also included .pdf exports of each of the three (admittedly messy) notebooks in which this project was completed: [whoop_eda.pdf](whoop_eda.pdf), [whoop_process.pdf](whoop_process.pdf), and [whoop_train_v2.pdf](whoop_train_v2.pdf).

## Abstract

Wearable fitness devices, such as the Whoop device, are now widely-used products for monitoring health and optimizing athletic performance. This project focuses on leveraging personal Whoop data collected over 21 months to achieve two objectives. First, I aim to accurately predict the labels of various activities recorded within the Whoop app. Second, I seek to approximate Whoop’s proprietary Recovery scores and obtain insights into the key features and relative complexity of Whoop’s algorithm.

The dataset for this project was generated from an export of my personal data from the Whoop app and contains metrics for logged activities, daily aggregate physiological data, and self-reported behaviors. The activity classification task was performed on the set of logged activities and involved the training of multiple classifiers on two uniquely-labeled subsets of the data. The recovery score regression task utilized the set of daily aggregate physiological data and included feature selection to identify the metrics essential to Whoop’s proprietary algorithm.

The results demonstrate that the simple neural network outperformed traditional models in activity classification, especially on the subset with a larger variety of class labels. In the regression task, the simple neural network underperformed, while the
Lasso and Ridge models performed the best, both out of the box and after feature selection. This indicates the potentially simple nature of Whoop’s Recovery score algorithm, and highlights the small subset of this algorithm’s likely critical features.