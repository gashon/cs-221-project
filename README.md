# cs-221-project

https://stanford-cs221.github.io/autumn2023/project.html

## Commands

```bash
conda create -n cs-221-project python=3.9

conda cs-221-project

pip install -r requirements.txt

jupyter notebook
```

## Dataset

[dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)
Using - `diabetes_012_health_indicators_BRFSS2015.csv1`

## Results

All models account for minority in dataset by increasing cost of misclassification for minority class `compute_class_weight('balanced', classes=np.unique(y_train.numpy()), y=y_train.numpy())`

#### Logistic Regression

Accuracy: 0.6477057710501419 \
Precision: 0.4459873934685125 \
Recall: 0.5219242645252017 \
F1 Score: 0.4277300172419794

#### Random Forest

Accuracy: 0.8384973194575843 \
Precision: 0.4375527556979038 \
Recall: 0.37723050001750785 \
F1 Score: 0.38404902215644404

#### XG Boost

Accuracy: 0.850540050457269 \
Precision: 0.47288791980781353 \
Recall: 0.39135446522908807 \
F1 Score: 0.4031200242585607

#### Neural Network

TODO

- regularization/ overfitting checking
- investigate why performance better without minority class improvement (good for writeup)

Accuracy: 0.7083727530747398 \
Precision: 0.44464256168286637 \
Recall: 0.5165500825427182 \
F1 Score: 0.4465402212325172
