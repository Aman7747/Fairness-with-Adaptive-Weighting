# Fairness-Aware Classification on COMPAS and Vehicle Insurance Datasets

This repository contains a comparative study of fairness-aware machine learning techniques applied to two sensitive datasets:

- **COMPAS**: Criminal recidivism prediction, focusing on racial fairness (African-American vs. Caucasian).
- **Vehicle Insurance**: Cross-sell prediction, focusing on gender fairness (Male vs. Female).

I have evaluated the impact of various data balancing and fairness-enhancing methods on both predictive performance and fairness metrics.


## 📊 Methods Compared

We evaluate five techniques on each dataset:

1. **Baseline** (logistic regression with class weights)
2. **Random Oversampling**
3. **Random Undersampling**
4. **SMOTE** (Synthetic Minority Oversampling Technique)
5. **Iterative Reweighting** (based on [Chai & Wang, 2022](https://proceedings.mlr.press/v162/chai22a.html))

---

## ⚖️ Fairness Metrics

We assess both predictive and fairness performance:

- **Accuracy**, **Precision**, **Recall**
- **Disparate Impact (DI)**  
- **Difference in Equal Opportunity (DEO)**
- **Difference in Predictive Equality (DPE)**

---

## 📁 Datasets

- **COMPAS Dataset**: [Kaggle Link](https://www.kaggle.com/datasets/aman7747/compas-dataset)
- **Vehicle Insurance Dataset**: [Kaggle Link](https://www.kaggle.com/datasets/anmolkumar/health-insurance-cross-sell-prediction)

Both datasets are publicly available and should be downloaded separately due to licensing.

---

## 📄 Citation

If you use this work or the iterative reweighting method, please cite:

```bibtex
@inproceedings{chai2022fairness,
  title={Fairness with Adaptive Weights},
  author={Chai, Junyi and Wang, Xiaoqian},
  booktitle={Proceedings of the 39th International Conference on Machine Learning},
  volume={162},
  pages={2924--2940},
  year={2022},
  organization={PMLR}
}
