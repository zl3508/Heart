## FGSCare: A Feature-driven Grid Search-based Machine Learning Framework for Coronary Heart Disease Prediction 

In the spirit of reproducible research, this repository includes all codes needed to reproduce the manuscript results.

### Environment Requirement
```
Python==3.12.0
torch==2.5.1
numpy==2.1.2
pandas==2.2.3
scikit-learn==1.5.2
seaborn==0.13.2
matplotlib==3.9.2
missingno==0.5.2
category-encoders==2.6.4
```

### Dataset
`framingham.csv`: It contains 4,240 records with various cardiovascular risk factors, aiming to predict the 10-year risk of Coronary Heart Disease (CHD). 
It includes demographic, lifestyle, medical history, and physiological features, with TenYearCHD as the target variable (1: CHD occurrence, 0: no CHD).

### Code Organization
The script to reproduce all the figures and tables in the paper is as follows:
- `original.ipynb`: training setting search (before feature processing) by ROC analysis.
- `healthcare.ipynb`: training setting search (after feature processing) by ROC analysis for multiple classifiers below:
   - traditional machine learning models: Decision Tree (DT), Logistic Regression (LR), Naive Bayes (NB), K-Nearest Neighbors (KNN), Gradient Boosting (GB) and ElasticNet,
   - deep learning models: Multilayer Perceptron (MLP), CNN, ResNet, RNN, Transformers, and KAN. 
- `PCA and t-sne.ipynb`: PCA analysis and t-sne analysis in feature engineering

