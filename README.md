# Drug Classification

Practice notebooks that predict which of five drugs (A, B, C, X or Y) suits a patient, from age, sex, blood pressure, cholesterol and sodium-to-potassium ratio. The notebooks compare tree-based models, KNN, SVM and a small TensorFlow network on a small tabular dataset.

## Data

[`drug200.csv`](drug200.csv): 200 patients, five features (`Age`, `Sex`, `BP`, `Cholesterol`, `Na_to_K`) and the target `Drug`. The classes are imbalanced: DrugY 91, drugX 54, drugA 23, drugB 16, drugC 16.

## Notebooks

| Notebook | Contents |
|---|---|
| `01. .ipynb` | Univariate and bivariate EDA, encoding, Random Forest, KNN and SVM |
| `02 .ipynb` | Random Forest versus a Keras neural network |
| `03. .ipynb` | Data checks (nulls, duplicates), feature engineering, KNN and ensemble models |
| `04_decision_tree.ipynb` | Decision tree with Gini and entropy criteria (`category_encoders` for encoding) |

In the saved output of `04_decision_tree.ipynb`, both criteria reach **84.85% test accuracy** on a 67/33 split. Results for the other notebooks are in their cell outputs.

## Running

```bash
git clone https://github.com/hasansust32/Drug_classification.git
cd Drug_classification
pip install jupyter pandas numpy scikit-learn seaborn matplotlib category_encoders tensorflow
jupyter notebook
```

The notebooks were written in Google Colab; replace the Drive paths with `drug200.csv`.

## Notes

- Learning exercise on a 200-row dataset; results are not meant to generalise.
- `hello.html` is an unrelated test file.

## Author

**S M Mahamudul Hasan** · [GitHub](https://github.com/hasansust32) · [Portfolio](https://www.hasansm.com/)
