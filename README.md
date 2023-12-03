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

Training Accuracy: 0.646784334594765 \
Accuracy: 0.6477057710501419 \
Precision: 0.4459873934685125 \
Recall: 0.5219242645252017 \
F1 Score: 0.4277300172419794

#### Random Forest

Training Accuracy: 0.6971529091769157 \
Accuracy: 0.6841690318511511 \
Precision: 0.4359208428740078 \
Recall: 0.5175056058566144 \
F1 Score: 0.43361360863998893

#### XG Boost

Training Accuracy: 0.8597889072847682 \
Accuracy: 0.850540050457269 \
Precision: 0.47288791980781353 \
Recall: 0.39135446522908807 \
F1 Score: 0.4031200242585607

#### Neural Network

Training Accuracy: 0.8417428781667192 \
Accuracy: 0.8448964574792389 \
Precision: 0.28163215249307966 \
Recall: 0.3333333333333333 \
F1 Score: 0.3053094403768174
