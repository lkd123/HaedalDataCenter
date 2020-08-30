# 06. 일반화 달성


{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [],
   "source": [
    "import pandas as pd\n",
    "from sklearn.datasets import load_boston\n",
    "boston=load_boston()\n",
    "dataset=pd.DataFrame(boston.data, columns=boston.feature_names)\n",
    "dataset['target'] = boston.target\n",
    "observations = len(dataset)\n",
    "variables = dataset.columns[:-1]\n",
    "X = dataset.iloc[:,:-1]\n",
    "y = dataset['target'].values"
   ]
  }
