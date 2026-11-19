# NLI preprocessing

[Open in Colab](https://colab.research.google.com/github/Aasta-EB/Group05-_KaggleCompetition/blob/Hamdi-Branch/preprocessing/01_NLI_Preprocessing.ipynb)

The notebook contains the executed preprocessing results and plots. Inputs are loaded from the attached Kaggle competition dataset or the original competition ZIP.

| File | Contents |
| --- | --- |
| train_clean.csv | 9,667 labeled training pairs |
| validation_clean.csv | 2,453 labeled validation pairs |
| test_clean.csv | 5,195 unlabeled test pairs |
| split_manifest.csv | Fixed training/validation IDs |
| preprocessing_summary.json | Dataset and split statistics |
| language_label_counts.csv | Class frequencies per language |
| near_duplicate_audit_sample.csv | Similarity results for 200 sampled validation rows |

Text features use `premise_clean` and `hypothesis_clean`. Raw text is retained for error analysis. The grouped split has zero normalized-premise overlap between training and validation. Learned transformations are fitted on training.

Optional classifier experiments are included with training disabled. POS features in those experiments cover English only.
