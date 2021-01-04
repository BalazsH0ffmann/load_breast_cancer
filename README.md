# load_breast_cancer

import sklearn
import sklearn

import pandas as pd
import numpy as np
from sklearn.datasets import load_breast_cancer
from sklearn.datasets import load_breast_cancer
cancer=load_breast_cancer()
print("cancer.keys():\n", cancer.keys())
cancer.keys():
 dict_keys(['data', 'target', 'frame', 'target_names', 'DESCR', 'feature_names', 'filename'])
print("Shape of cancerdata:", cancer.data.shape)
Shape of cancerdata: (569, 30)
)
print("Sample counts per class:\n",
    {n: v for n, v in zip(cancer.target_names, np.bincount(cancer.target))})
Sample counts per class:
 {'malignant': 212, 'benign': 357}
, cancer.feature_names
print("Feature names:\n", cancer.feature_names)
Feature names:
 ['mean radius' 'mean texture' 'mean perimeter' 'mean area'
 'mean smoothness' 'mean compactness' 'mean concavity'
 'mean concave points' 'mean symmetry' 'mean fractal dimension'
 'radius error' 'texture error' 'perimeter error' 'area error'
 'smoothness error' 'compactness error' 'concavity error'
 'concave points error' 'symmetry error' 'fractal dimension error'
 'worst radius' 'worst texture' 'worst perimeter' 'worst area'
 'worst smoothness' 'worst compactness' 'worst concavity'
 'worst concave points' 'worst symmetry' 'worst fractal dimension']
